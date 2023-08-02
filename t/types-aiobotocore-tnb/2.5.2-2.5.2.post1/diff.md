# Comparing `tmp/types-aiobotocore-tnb-2.5.2.tar.gz` & `tmp/types-aiobotocore-tnb-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-tnb-2.5.2.tar", last modified: Sat Jul  8 01:44:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-tnb-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:07 2023, max compression
```

## Comparing `types-aiobotocore-tnb-2.5.2.tar` & `types-aiobotocore-tnb-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.903006 types-aiobotocore-tnb-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-08 01:44:25.903006 types-aiobotocore-tnb-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:25.903006 types-aiobotocore-tnb-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.895006 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27273 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34773 2023-07-08 01:42:02.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-08 01:42:02.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:01.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.903006 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-08 01:44:25.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:25.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:25.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:25.000000 types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26984 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-08-02 14:50:37.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34594 2023-08-02 14:50:37.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-08-02 14:50:37.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-tnb-2.5.2/LICENSE` & `types-aiobotocore-tnb-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2/PKG-INFO` & `types-aiobotocore-tnb-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-tnb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore tnb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore tnb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-tnb"></a>
 
 # types-aiobotocore-tnb
 
 [![PyPI - types-aiobotocore-tnb](https://img.shields.io/pypi/v/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-tnb?color=blue)](https://pypistats.org/packages/types-aiobotocore-tnb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-tnb)](https://pepy.tech/project/types-aiobotocore-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TelcoNetworkBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [types-aiobotocore-tnb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/).
 
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
@@ -342,97 +341,98 @@
 )
 
 
 def check_value(value: DescriptorContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_tnb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_tnb.type_defs import (
+    BlobTypeDef,
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
-    PutSolFunctionPackageContentInputRequestTypeDef,
-    PutSolNetworkPackageContentInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
+    PutSolFunctionPackageContentInputRequestTypeDef,
+    PutSolNetworkPackageContentInputRequestTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
@@ -453,15 +453,15 @@
     GetSolNetworkPackageOutputTypeDef,
     PutSolNetworkPackageContentOutputTypeDef,
     ValidateSolNetworkPackageContentOutputTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
 )
 
 
-def get_structure() -> CancelSolNetworkOperationInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-tnb-2.5.2/README.md` & `types-aiobotocore-tnb-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-tnb"></a>
 
 # types-aiobotocore-tnb
 
 [![PyPI - types-aiobotocore-tnb](https://img.shields.io/pypi/v/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-tnb?color=blue)](https://pypistats.org/packages/types-aiobotocore-tnb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-tnb)](https://pepy.tech/project/types-aiobotocore-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TelcoNetworkBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [types-aiobotocore-tnb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/).
 
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
@@ -309,97 +309,98 @@
 )
 
 
 def check_value(value: DescriptorContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_tnb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_tnb.type_defs import (
+    BlobTypeDef,
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
-    PutSolFunctionPackageContentInputRequestTypeDef,
-    PutSolNetworkPackageContentInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
+    PutSolFunctionPackageContentInputRequestTypeDef,
+    PutSolNetworkPackageContentInputRequestTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
@@ -420,15 +421,15 @@
     GetSolNetworkPackageOutputTypeDef,
     PutSolNetworkPackageContentOutputTypeDef,
     ValidateSolNetworkPackageContentOutputTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
 )
 
 
-def get_structure() -> CancelSolNetworkOperationInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-tnb-2.5.2/setup.py` & `types-aiobotocore-tnb-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-tnb",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_tnb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2 service generated with"
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
-    keywords="aiobotocore tnb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore tnb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_tnb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/__init__.py` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/__init__.pyi` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/__main__.py` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder\nOther"
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

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/client.py` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
     session = get_session()
     async with session.create_client("tnb") as client:
         client: TelcoNetworkBuilderClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import NsdOperationalStateType, OperationalStateType
 from .paginator import (
     ListSolFunctionInstancesPaginator,
     ListSolFunctionPackagesPaginator,
     ListSolNetworkInstancesPaginator,
     ListSolNetworkOperationsPaginator,
     ListSolNetworkPackagesPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorOutputTypeDef,
@@ -369,33 +369,25 @@
         Lists tags for AWS TNB resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#list_tags_for_resource)
         """
 
     async def put_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolFunctionPackageContentOutputTypeDef:
         """
         Uploads the contents of a function package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_function_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#put_sol_function_package_content)
         """
 
     async def put_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolNetworkPackageContentOutputTypeDef:
         """
         Uploads the contents of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_network_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#put_sol_network_package_content)
         """
@@ -458,33 +450,25 @@
         Updates the operational state of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.update_sol_network_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#update_sol_network_package)
         """
 
     async def validate_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolFunctionPackageContentOutputTypeDef:
         """
         Validates function package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_function_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#validate_sol_function_package_content)
         """
 
     async def validate_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolNetworkPackageContentOutputTypeDef:
         """
         Validates network package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_network_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#validate_sol_network_package_content)
         """
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/client.pyi` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
     session = get_session()
     async with session.create_client("tnb") as client:
         client: TelcoNetworkBuilderClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import NsdOperationalStateType, OperationalStateType
 from .paginator import (
     ListSolFunctionInstancesPaginator,
     ListSolFunctionPackagesPaginator,
     ListSolNetworkInstancesPaginator,
     ListSolNetworkOperationsPaginator,
     ListSolNetworkPackagesPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CreateSolFunctionPackageOutputTypeDef,
     CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
     GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorOutputTypeDef,
@@ -338,32 +338,24 @@
         """
         Lists tags for AWS TNB resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#list_tags_for_resource)
         """
     async def put_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolFunctionPackageContentOutputTypeDef:
         """
         Uploads the contents of a function package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_function_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#put_sol_function_package_content)
         """
     async def put_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> PutSolNetworkPackageContentOutputTypeDef:
         """
         Uploads the contents of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.put_sol_network_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#put_sol_network_package_content)
         """
@@ -419,32 +411,24 @@
         """
         Updates the operational state of a network package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.update_sol_network_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#update_sol_network_package)
         """
     async def validate_sol_function_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        vnfPkgId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, vnfPkgId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolFunctionPackageContentOutputTypeDef:
         """
         Validates function package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_function_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#validate_sol_function_package_content)
         """
     async def validate_sol_network_package_content(
-        self,
-        *,
-        file: Union[str, bytes, IO[Any], StreamingBody],
-        nsdInfoId: str,
-        contentType: Literal["application/zip"] = ...
+        self, *, file: BlobTypeDef, nsdInfoId: str, contentType: Literal["application/zip"] = ...
     ) -> ValidateSolNetworkPackageContentOutputTypeDef:
         """
         Validates network package content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Client.validate_sol_network_package_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/client/#validate_sol_network_package_content)
         """
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/literals.py` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/literals.pyi` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/paginator.py` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -46,91 +46,84 @@
     "ListSolFunctionInstancesPaginator",
     "ListSolFunctionPackagesPaginator",
     "ListSolNetworkInstancesPaginator",
     "ListSolNetworkOperationsPaginator",
     "ListSolNetworkPackagesPaginator",
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
 class ListSolFunctionInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctioninstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolFunctionInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctioninstancespaginator)
         """
 
-
 class ListSolFunctionPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctionpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolFunctionPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctionpackagespaginator)
         """
 
-
 class ListSolNetworkInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolNetworkInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkinstancespaginator)
         """
 
-
 class ListSolNetworkOperationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolNetworkOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkoperationspaginator)
         """
 
-
 class ListSolNetworkPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolNetworkPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkpackagespaginator)
         """
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/paginator.pyi` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,84 +46,91 @@
     "ListSolFunctionInstancesPaginator",
     "ListSolFunctionPackagesPaginator",
     "ListSolNetworkInstancesPaginator",
     "ListSolNetworkOperationsPaginator",
     "ListSolNetworkPackagesPaginator",
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
 class ListSolFunctionInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctioninstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolFunctionInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctioninstancespaginator)
         """
 
+
 class ListSolFunctionPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctionpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolFunctionPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolFunctionPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolfunctionpackagespaginator)
         """
 
+
 class ListSolNetworkInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolNetworkInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkinstancespaginator)
         """
 
+
 class ListSolNetworkOperationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolNetworkOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkoperationspaginator)
         """
 
+
 class ListSolNetworkPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSolNetworkPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder.Paginator.ListSolNetworkPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/paginators/#listsolnetworkpackagespaginator)
         """
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/type_defs.py` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for tnb service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_tnb.type_defs import CancelSolNetworkOperationInputRequestTypeDef
+    from types_aiobotocore_tnb.type_defs import BlobTypeDef
 
-    data: CancelSolNetworkOperationInputRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,88 +39,89 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
-    "CreateSolFunctionPackageOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
-    "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
-    "CreateSolNetworkPackageOutputTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
     "DeleteSolNetworkPackageInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "ToscaOverrideTypeDef",
     "GetSolFunctionInstanceInputRequestTypeDef",
     "GetSolFunctionInstanceMetadataTypeDef",
     "GetSolFunctionPackageContentInputRequestTypeDef",
-    "GetSolFunctionPackageContentOutputTypeDef",
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
     "GetSolFunctionPackageInputRequestTypeDef",
     "GetSolInstantiatedVnfInfoTypeDef",
     "GetSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkInstanceMetadataTypeDef",
     "LcmOperationInfoTypeDef",
     "GetSolNetworkOperationInputRequestTypeDef",
     "GetSolNetworkOperationMetadataTypeDef",
     "ProblemDetailsTypeDef",
     "GetSolNetworkPackageContentInputRequestTypeDef",
-    "GetSolNetworkPackageContentOutputTypeDef",
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
     "GetSolNetworkPackageInputRequestTypeDef",
     "GetSolVnfcResourceInfoMetadataTypeDef",
     "InstantiateSolNetworkInstanceInputRequestTypeDef",
-    "InstantiateSolNetworkInstanceOutputTypeDef",
     "ListSolFunctionInstanceMetadataTypeDef",
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSolFunctionInstancesInputRequestTypeDef",
     "ListSolFunctionPackageMetadataTypeDef",
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
     "ListSolFunctionPackagesInputRequestTypeDef",
     "ListSolNetworkInstanceMetadataTypeDef",
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutSolFunctionPackageContentInputRequestTypeDef",
-    "PutSolNetworkPackageContentInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
-    "TerminateSolNetworkInstanceOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
-    "UpdateSolFunctionPackageOutputTypeDef",
     "UpdateSolNetworkModifyTypeDef",
-    "UpdateSolNetworkInstanceOutputTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
-    "UpdateSolNetworkPackageOutputTypeDef",
+    "PutSolFunctionPackageContentInputRequestTypeDef",
+    "PutSolNetworkPackageContentInputRequestTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
+    "CreateSolFunctionPackageOutputTypeDef",
+    "CreateSolNetworkInstanceOutputTypeDef",
+    "CreateSolNetworkPackageOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetSolFunctionPackageContentOutputTypeDef",
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    "GetSolNetworkPackageContentOutputTypeDef",
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolFunctionPackageOutputTypeDef",
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolNetworkPackageOutputTypeDef",
     "GetSolNetworkOperationTaskDetailsTypeDef",
     "FunctionArtifactMetaTypeDef",
     "NetworkArtifactMetaTypeDef",
     "GetSolNetworkInstanceOutputTypeDef",
     "GetSolVnfcResourceInfoTypeDef",
     "ListSolFunctionInstanceInfoTypeDef",
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolFunctionPackageInfoTypeDef",
     "ListSolNetworkInstanceInfoTypeDef",
     "ListSolNetworkOperationsInfoTypeDef",
     "ListSolNetworkPackageInfoTypeDef",
     "UpdateSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkOperationOutputTypeDef",
     "GetSolFunctionPackageMetadataTypeDef",
@@ -140,14 +141,15 @@
     "ValidateSolFunctionPackageContentOutputTypeDef",
     "GetSolNetworkPackageOutputTypeDef",
     "PutSolNetworkPackageContentOutputTypeDef",
     "ValidateSolNetworkPackageContentOutputTypeDef",
     "GetSolFunctionInstanceOutputTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSolNetworkOperationInputRequestTypeDef = TypedDict(
     "CancelSolNetworkOperationInputRequestTypeDef",
     {
         "nsLcmOpOccId": str,
     },
 )
 
@@ -155,24 +157,22 @@
     "CreateSolFunctionPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolFunctionPackageOutputTypeDef = TypedDict(
-    "CreateSolFunctionPackageOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "onboardingState": OnboardingStateType,
-        "operationalState": OperationalStateType,
-        "tags": Dict[str, str],
-        "usageState": UsageStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSolNetworkInstanceInputRequestTypeDef = TypedDict(
     "_RequiredCreateSolNetworkInstanceInputRequestTypeDef",
     {
         "nsName": str,
@@ -192,47 +192,22 @@
 class CreateSolNetworkInstanceInputRequestTypeDef(
     _RequiredCreateSolNetworkInstanceInputRequestTypeDef,
     _OptionalCreateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
-CreateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "CreateSolNetworkInstanceOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsInstanceName": str,
-        "nsdInfoId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "CreateSolNetworkPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolNetworkPackageOutputTypeDef = TypedDict(
-    "CreateSolNetworkPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsdOnboardingState": NsdOnboardingStateType,
-        "nsdOperationalState": NsdOperationalStateType,
-        "nsdUsageState": NsdUsageStateType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSolFunctionPackageInputRequestTypeDef = TypedDict(
     "DeleteSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -246,21 +221,14 @@
 DeleteSolNetworkPackageInputRequestTypeDef = TypedDict(
     "DeleteSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "cause": str,
         "details": str,
     },
     total=False,
@@ -294,40 +262,22 @@
     "GetSolFunctionPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageContentOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "packageContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
     {
         "accept": Literal["text/plain"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "vnfd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -399,39 +349,21 @@
     "GetSolNetworkPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageContentOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "nsdContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "nsd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
@@ -465,35 +397,28 @@
 class InstantiateSolNetworkInstanceInputRequestTypeDef(
     _RequiredInstantiateSolNetworkInstanceInputRequestTypeDef,
     _OptionalInstantiateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
 
-InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListSolFunctionInstanceMetadataTypeDef = TypedDict(
     "ListSolFunctionInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
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
 
 ListSolFunctionInstancesInputRequestTypeDef = TypedDict(
     "ListSolFunctionInstancesInputRequestTypeDef",
     {
@@ -507,22 +432,14 @@
     "ListSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolFunctionPackagesInputRequestTypeDef = TypedDict(
     "ListSolFunctionPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -532,22 +449,14 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkInstancesInputRequestTypeDef = TypedDict(
     "ListSolNetworkInstancesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -557,22 +466,14 @@
     "ListSolNetworkOperationsMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkOperationsInputRequestTypeDef = TypedDict(
     "ListSolNetworkOperationsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -582,22 +483,14 @@
     "ListSolNetworkPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkPackagesInputRequestTypeDef = TypedDict(
     "ListSolNetworkPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -606,36 +499,80 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
+    "_RequiredTerminateSolNetworkInstanceInputRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "nsInstanceId": str,
+    },
+)
+_OptionalTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
+    "_OptionalTerminateSolNetworkInstanceInputRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class TerminateSolNetworkInstanceInputRequestTypeDef(
+    _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
+    _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
+):
+    pass
+
+
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
+UpdateSolFunctionPackageInputRequestTypeDef = TypedDict(
+    "UpdateSolFunctionPackageInputRequestTypeDef",
+    {
+        "operationalState": OperationalStateType,
+        "vnfPkgId": str,
+    },
+)
+
+UpdateSolNetworkModifyTypeDef = TypedDict(
+    "UpdateSolNetworkModifyTypeDef",
+    {
+        "vnfConfigurableProperties": Mapping[str, Any],
+        "vnfInstanceId": str,
+    },
+)
+
+UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
+    "UpdateSolNetworkPackageInputRequestTypeDef",
+    {
+        "nsdInfoId": str,
+        "nsdOperationalState": NsdOperationalStateType,
+    },
+)
+
 _RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "vnfPkgId": str,
     },
 )
 _OptionalPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalPutSolFunctionPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
@@ -650,15 +587,15 @@
 ):
     pass
 
 
 _RequiredPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolNetworkPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "nsdInfoId": str,
     },
 )
 _OptionalPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalPutSolNetworkPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
@@ -670,166 +607,191 @@
 class PutSolNetworkPackageContentInputRequestTypeDef(
     _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
     _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "file": BlobTypeDef,
+        "vnfPkgId": str,
     },
 )
-
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+_OptionalValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalValidateSolFunctionPackageContentInputRequestTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "contentType": Literal["application/zip"],
     },
+    total=False,
 )
 
-_RequiredTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
-    "_RequiredTerminateSolNetworkInstanceInputRequestTypeDef",
+
+class ValidateSolFunctionPackageContentInputRequestTypeDef(
+    _RequiredValidateSolFunctionPackageContentInputRequestTypeDef,
+    _OptionalValidateSolFunctionPackageContentInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredValidateSolNetworkPackageContentInputRequestTypeDef",
     {
-        "nsInstanceId": str,
+        "file": BlobTypeDef,
+        "nsdInfoId": str,
     },
 )
-_OptionalTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
-    "_OptionalTerminateSolNetworkInstanceInputRequestTypeDef",
+_OptionalValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalValidateSolNetworkPackageContentInputRequestTypeDef",
     {
-        "tags": Mapping[str, str],
+        "contentType": Literal["application/zip"],
     },
     total=False,
 )
 
 
-class TerminateSolNetworkInstanceInputRequestTypeDef(
-    _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
-    _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
+class ValidateSolNetworkPackageContentInputRequestTypeDef(
+    _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
+    _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
 
-TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "TerminateSolNetworkInstanceOutputTypeDef",
+CreateSolFunctionPackageOutputTypeDef = TypedDict(
+    "CreateSolFunctionPackageOutputTypeDef",
     {
-        "nsLcmOpOccId": str,
+        "arn": str,
+        "id": str,
+        "onboardingState": OnboardingStateType,
+        "operationalState": OperationalStateType,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "usageState": UsageStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
+CreateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "CreateSolNetworkInstanceOutputTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "arn": str,
+        "id": str,
+        "nsInstanceName": str,
+        "nsdInfoId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolFunctionPackageInputRequestTypeDef = TypedDict(
-    "UpdateSolFunctionPackageInputRequestTypeDef",
+CreateSolNetworkPackageOutputTypeDef = TypedDict(
+    "CreateSolNetworkPackageOutputTypeDef",
     {
-        "operationalState": OperationalStateType,
-        "vnfPkgId": str,
+        "arn": str,
+        "id": str,
+        "nsdOnboardingState": NsdOnboardingStateType,
+        "nsdOperationalState": NsdOperationalStateType,
+        "nsdUsageState": NsdUsageStateType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolFunctionPackageOutputTypeDef = TypedDict(
-    "UpdateSolFunctionPackageOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "operationalState": OperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkModifyTypeDef = TypedDict(
-    "UpdateSolNetworkModifyTypeDef",
+GetSolFunctionPackageContentOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageContentOutputTypeDef",
     {
-        "vnfConfigurableProperties": Mapping[str, Any],
-        "vnfInstanceId": str,
+        "contentType": Literal["application/zip"],
+        "packageContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "UpdateSolNetworkInstanceOutputTypeDef",
+GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
     {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "contentType": Literal["text/plain"],
+        "vnfd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
-    "UpdateSolNetworkPackageInputRequestTypeDef",
+GetSolNetworkPackageContentOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageContentOutputTypeDef",
     {
-        "nsdInfoId": str,
-        "nsdOperationalState": NsdOperationalStateType,
+        "contentType": Literal["application/zip"],
+        "nsdContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkPackageOutputTypeDef = TypedDict(
-    "UpdateSolNetworkPackageOutputTypeDef",
+GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
     {
-        "nsdOperationalState": NsdOperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "contentType": Literal["text/plain"],
+        "nsd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
+InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "InstantiateSolNetworkInstanceOutputTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "vnfPkgId": str,
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalValidateSolFunctionPackageContentInputRequestTypeDef",
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
-        "contentType": Literal["application/zip"],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ValidateSolFunctionPackageContentInputRequestTypeDef(
-    _RequiredValidateSolFunctionPackageContentInputRequestTypeDef,
-    _OptionalValidateSolFunctionPackageContentInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredValidateSolNetworkPackageContentInputRequestTypeDef",
+TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "TerminateSolNetworkInstanceOutputTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "nsdInfoId": str,
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalValidateSolNetworkPackageContentInputRequestTypeDef",
+
+UpdateSolFunctionPackageOutputTypeDef = TypedDict(
+    "UpdateSolFunctionPackageOutputTypeDef",
     {
-        "contentType": Literal["application/zip"],
+        "operationalState": OperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ValidateSolNetworkPackageContentInputRequestTypeDef(
-    _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
-    _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
-):
-    pass
-
+UpdateSolNetworkPackageOutputTypeDef = TypedDict(
+    "UpdateSolNetworkPackageOutputTypeDef",
+    {
+        "nsdOperationalState": NsdOperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetSolNetworkOperationTaskDetailsTypeDef = TypedDict(
     "GetSolNetworkOperationTaskDetailsTypeDef",
     {
         "taskContext": Dict[str, str],
         "taskEndTime": datetime,
         "taskErrorDetails": ErrorInfoTypeDef,
@@ -865,15 +827,15 @@
         "metadata": GetSolNetworkInstanceMetadataTypeDef,
         "nsInstanceDescription": str,
         "nsInstanceName": str,
         "nsState": NsStateType,
         "nsdId": str,
         "nsdInfoId": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolVnfcResourceInfoTypeDef = TypedDict(
     "GetSolVnfcResourceInfoTypeDef",
     {
         "metadata": GetSolVnfcResourceInfoMetadataTypeDef,
@@ -904,14 +866,54 @@
 
 class ListSolFunctionInstanceInfoTypeDef(
     _RequiredListSolFunctionInstanceInfoTypeDef, _OptionalListSolFunctionInstanceInfoTypeDef
 ):
     pass
 
 
+ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListSolFunctionPackageInfoTypeDef = TypedDict(
     "_RequiredListSolFunctionPackageInfoTypeDef",
     {
         "arn": str,
         "id": str,
         "onboardingState": OnboardingStateType,
         "operationalState": OperationalStateType,
@@ -1040,15 +1042,15 @@
         "id": str,
         "lcmOperationType": LcmOperationTypeType,
         "metadata": GetSolNetworkOperationMetadataTypeDef,
         "nsInstanceId": str,
         "operationState": NsLcmOperationStateType,
         "tags": Dict[str, str],
         "tasks": List[GetSolNetworkOperationTaskDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSolFunctionPackageMetadataTypeDef = TypedDict(
     "_RequiredGetSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
@@ -1134,51 +1136,51 @@
 )
 
 ListSolFunctionInstancesOutputTypeDef = TypedDict(
     "ListSolFunctionInstancesOutputTypeDef",
     {
         "functionInstances": List[ListSolFunctionInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolFunctionPackagesOutputTypeDef = TypedDict(
     "ListSolFunctionPackagesOutputTypeDef",
     {
         "functionPackages": List[ListSolFunctionPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkInstancesOutputTypeDef = TypedDict(
     "ListSolNetworkInstancesOutputTypeDef",
     {
         "networkInstances": List[ListSolNetworkInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkOperationsOutputTypeDef = TypedDict(
     "ListSolNetworkOperationsOutputTypeDef",
     {
         "networkOperations": List[ListSolNetworkOperationsInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkPackagesOutputTypeDef = TypedDict(
     "ListSolNetworkPackagesOutputTypeDef",
     {
         "networkPackages": List[ListSolNetworkPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionPackageOutputTypeDef = TypedDict(
     "GetSolFunctionPackageOutputTypeDef",
     {
         "arn": str,
@@ -1188,41 +1190,41 @@
         "operationalState": OperationalStateType,
         "tags": Dict[str, str],
         "usageState": UsageStateType,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolFunctionPackageContentOutputTypeDef = TypedDict(
     "PutSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": PutSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolFunctionPackageContentOutputTypeDef = TypedDict(
     "ValidateSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": ValidateSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolNetworkPackageOutputTypeDef = TypedDict(
     "GetSolNetworkPackageOutputTypeDef",
     {
         "arn": str,
@@ -1232,43 +1234,43 @@
         "nsdName": str,
         "nsdOnboardingState": NsdOnboardingStateType,
         "nsdOperationalState": NsdOperationalStateType,
         "nsdUsageState": NsdUsageStateType,
         "nsdVersion": str,
         "tags": Dict[str, str],
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolNetworkPackageContentOutputTypeDef = TypedDict(
     "PutSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": PutSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolNetworkPackageContentOutputTypeDef = TypedDict(
     "ValidateSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": ValidateSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionInstanceOutputTypeDef = TypedDict(
     "GetSolFunctionInstanceOutputTypeDef",
     {
         "arn": str,
@@ -1279,10 +1281,10 @@
         "nsInstanceId": str,
         "tags": Dict[str, str],
         "vnfPkgId": str,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb/type_defs.pyi` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for tnb service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_tnb.type_defs import CancelSolNetworkOperationInputRequestTypeDef
+    from types_aiobotocore_tnb.type_defs import BlobTypeDef
 
-    data: CancelSolNetworkOperationInputRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -38,88 +38,89 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "CancelSolNetworkOperationInputRequestTypeDef",
     "CreateSolFunctionPackageInputRequestTypeDef",
-    "CreateSolFunctionPackageOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSolNetworkInstanceInputRequestTypeDef",
-    "CreateSolNetworkInstanceOutputTypeDef",
     "CreateSolNetworkPackageInputRequestTypeDef",
-    "CreateSolNetworkPackageOutputTypeDef",
     "DeleteSolFunctionPackageInputRequestTypeDef",
     "DeleteSolNetworkInstanceInputRequestTypeDef",
     "DeleteSolNetworkPackageInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "ToscaOverrideTypeDef",
     "GetSolFunctionInstanceInputRequestTypeDef",
     "GetSolFunctionInstanceMetadataTypeDef",
     "GetSolFunctionPackageContentInputRequestTypeDef",
-    "GetSolFunctionPackageContentOutputTypeDef",
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
     "GetSolFunctionPackageInputRequestTypeDef",
     "GetSolInstantiatedVnfInfoTypeDef",
     "GetSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkInstanceMetadataTypeDef",
     "LcmOperationInfoTypeDef",
     "GetSolNetworkOperationInputRequestTypeDef",
     "GetSolNetworkOperationMetadataTypeDef",
     "ProblemDetailsTypeDef",
     "GetSolNetworkPackageContentInputRequestTypeDef",
-    "GetSolNetworkPackageContentOutputTypeDef",
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
     "GetSolNetworkPackageInputRequestTypeDef",
     "GetSolVnfcResourceInfoMetadataTypeDef",
     "InstantiateSolNetworkInstanceInputRequestTypeDef",
-    "InstantiateSolNetworkInstanceOutputTypeDef",
     "ListSolFunctionInstanceMetadataTypeDef",
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSolFunctionInstancesInputRequestTypeDef",
     "ListSolFunctionPackageMetadataTypeDef",
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
     "ListSolFunctionPackagesInputRequestTypeDef",
     "ListSolNetworkInstanceMetadataTypeDef",
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
     "ListSolNetworkInstancesInputRequestTypeDef",
     "ListSolNetworkOperationsMetadataTypeDef",
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
     "ListSolNetworkOperationsInputRequestTypeDef",
     "ListSolNetworkPackageMetadataTypeDef",
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolNetworkPackagesInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutSolFunctionPackageContentInputRequestTypeDef",
-    "PutSolNetworkPackageContentInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "TerminateSolNetworkInstanceInputRequestTypeDef",
-    "TerminateSolNetworkInstanceOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateSolFunctionPackageInputRequestTypeDef",
-    "UpdateSolFunctionPackageOutputTypeDef",
     "UpdateSolNetworkModifyTypeDef",
-    "UpdateSolNetworkInstanceOutputTypeDef",
     "UpdateSolNetworkPackageInputRequestTypeDef",
-    "UpdateSolNetworkPackageOutputTypeDef",
+    "PutSolFunctionPackageContentInputRequestTypeDef",
+    "PutSolNetworkPackageContentInputRequestTypeDef",
     "ValidateSolFunctionPackageContentInputRequestTypeDef",
     "ValidateSolNetworkPackageContentInputRequestTypeDef",
+    "CreateSolFunctionPackageOutputTypeDef",
+    "CreateSolNetworkInstanceOutputTypeDef",
+    "CreateSolNetworkPackageOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetSolFunctionPackageContentOutputTypeDef",
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
+    "GetSolNetworkPackageContentOutputTypeDef",
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
+    "InstantiateSolNetworkInstanceOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolFunctionPackageOutputTypeDef",
+    "UpdateSolNetworkInstanceOutputTypeDef",
+    "UpdateSolNetworkPackageOutputTypeDef",
     "GetSolNetworkOperationTaskDetailsTypeDef",
     "FunctionArtifactMetaTypeDef",
     "NetworkArtifactMetaTypeDef",
     "GetSolNetworkInstanceOutputTypeDef",
     "GetSolVnfcResourceInfoTypeDef",
     "ListSolFunctionInstanceInfoTypeDef",
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
     "ListSolFunctionPackageInfoTypeDef",
     "ListSolNetworkInstanceInfoTypeDef",
     "ListSolNetworkOperationsInfoTypeDef",
     "ListSolNetworkPackageInfoTypeDef",
     "UpdateSolNetworkInstanceInputRequestTypeDef",
     "GetSolNetworkOperationOutputTypeDef",
     "GetSolFunctionPackageMetadataTypeDef",
@@ -139,14 +140,15 @@
     "ValidateSolFunctionPackageContentOutputTypeDef",
     "GetSolNetworkPackageOutputTypeDef",
     "PutSolNetworkPackageContentOutputTypeDef",
     "ValidateSolNetworkPackageContentOutputTypeDef",
     "GetSolFunctionInstanceOutputTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSolNetworkOperationInputRequestTypeDef = TypedDict(
     "CancelSolNetworkOperationInputRequestTypeDef",
     {
         "nsLcmOpOccId": str,
     },
 )
 
@@ -154,24 +156,22 @@
     "CreateSolFunctionPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolFunctionPackageOutputTypeDef = TypedDict(
-    "CreateSolFunctionPackageOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "onboardingState": OnboardingStateType,
-        "operationalState": OperationalStateType,
-        "tags": Dict[str, str],
-        "usageState": UsageStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSolNetworkInstanceInputRequestTypeDef = TypedDict(
     "_RequiredCreateSolNetworkInstanceInputRequestTypeDef",
     {
         "nsName": str,
@@ -189,47 +189,22 @@
 
 class CreateSolNetworkInstanceInputRequestTypeDef(
     _RequiredCreateSolNetworkInstanceInputRequestTypeDef,
     _OptionalCreateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
-CreateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "CreateSolNetworkInstanceOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsInstanceName": str,
-        "nsdInfoId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSolNetworkPackageInputRequestTypeDef = TypedDict(
     "CreateSolNetworkPackageInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateSolNetworkPackageOutputTypeDef = TypedDict(
-    "CreateSolNetworkPackageOutputTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "nsdOnboardingState": NsdOnboardingStateType,
-        "nsdOperationalState": NsdOperationalStateType,
-        "nsdUsageState": NsdUsageStateType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSolFunctionPackageInputRequestTypeDef = TypedDict(
     "DeleteSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -243,21 +218,14 @@
 DeleteSolNetworkPackageInputRequestTypeDef = TypedDict(
     "DeleteSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "cause": str,
         "details": str,
     },
     total=False,
@@ -291,40 +259,22 @@
     "GetSolFunctionPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageContentOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "packageContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageDescriptorInputRequestTypeDef",
     {
         "accept": Literal["text/plain"],
         "vnfPkgId": str,
     },
 )
 
-GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolFunctionPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "vnfd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolFunctionPackageInputRequestTypeDef = TypedDict(
     "GetSolFunctionPackageInputRequestTypeDef",
     {
         "vnfPkgId": str,
     },
 )
 
@@ -394,39 +344,21 @@
     "GetSolNetworkPackageContentInputRequestTypeDef",
     {
         "accept": Literal["application/zip"],
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageContentOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageContentOutputTypeDef",
-    {
-        "contentType": Literal["application/zip"],
-        "nsdContent": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageDescriptorInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageDescriptorInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
-GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
-    "GetSolNetworkPackageDescriptorOutputTypeDef",
-    {
-        "contentType": Literal["text/plain"],
-        "nsd": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSolNetworkPackageInputRequestTypeDef = TypedDict(
     "GetSolNetworkPackageInputRequestTypeDef",
     {
         "nsdInfoId": str,
     },
 )
 
@@ -458,35 +390,28 @@
 
 class InstantiateSolNetworkInstanceInputRequestTypeDef(
     _RequiredInstantiateSolNetworkInstanceInputRequestTypeDef,
     _OptionalInstantiateSolNetworkInstanceInputRequestTypeDef,
 ):
     pass
 
-InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "InstantiateSolNetworkInstanceOutputTypeDef",
-    {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListSolFunctionInstanceMetadataTypeDef = TypedDict(
     "ListSolFunctionInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
-    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
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
 
 ListSolFunctionInstancesInputRequestTypeDef = TypedDict(
     "ListSolFunctionInstancesInputRequestTypeDef",
     {
@@ -500,22 +425,14 @@
     "ListSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
-    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolFunctionPackagesInputRequestTypeDef = TypedDict(
     "ListSolFunctionPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -525,22 +442,14 @@
     "ListSolNetworkInstanceMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
-    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkInstancesInputRequestTypeDef = TypedDict(
     "ListSolNetworkInstancesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -550,22 +459,14 @@
     "ListSolNetworkOperationsMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
-    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkOperationsInputRequestTypeDef = TypedDict(
     "ListSolNetworkOperationsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -575,22 +476,14 @@
     "ListSolNetworkPackageMetadataTypeDef",
     {
         "createdAt": datetime,
         "lastModified": datetime,
     },
 )
 
-ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
-    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSolNetworkPackagesInputRequestTypeDef = TypedDict(
     "ListSolNetworkPackagesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -599,36 +492,78 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
+    "_RequiredTerminateSolNetworkInstanceInputRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "nsInstanceId": str,
+    },
+)
+_OptionalTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
+    "_OptionalTerminateSolNetworkInstanceInputRequestTypeDef",
+    {
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class TerminateSolNetworkInstanceInputRequestTypeDef(
+    _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
+    _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
+):
+    pass
+
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
+UpdateSolFunctionPackageInputRequestTypeDef = TypedDict(
+    "UpdateSolFunctionPackageInputRequestTypeDef",
+    {
+        "operationalState": OperationalStateType,
+        "vnfPkgId": str,
+    },
+)
+
+UpdateSolNetworkModifyTypeDef = TypedDict(
+    "UpdateSolNetworkModifyTypeDef",
+    {
+        "vnfConfigurableProperties": Mapping[str, Any],
+        "vnfInstanceId": str,
+    },
+)
+
+UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
+    "UpdateSolNetworkPackageInputRequestTypeDef",
+    {
+        "nsdInfoId": str,
+        "nsdOperationalState": NsdOperationalStateType,
+    },
+)
+
 _RequiredPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolFunctionPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "vnfPkgId": str,
     },
 )
 _OptionalPutSolFunctionPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalPutSolFunctionPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
@@ -641,15 +576,15 @@
     _OptionalPutSolFunctionPackageContentInputRequestTypeDef,
 ):
     pass
 
 _RequiredPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_RequiredPutSolNetworkPackageContentInputRequestTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
+        "file": BlobTypeDef,
         "nsdInfoId": str,
     },
 )
 _OptionalPutSolNetworkPackageContentInputRequestTypeDef = TypedDict(
     "_OptionalPutSolNetworkPackageContentInputRequestTypeDef",
     {
         "contentType": Literal["application/zip"],
@@ -659,160 +594,187 @@
 
 class PutSolNetworkPackageContentInputRequestTypeDef(
     _RequiredPutSolNetworkPackageContentInputRequestTypeDef,
     _OptionalPutSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "file": BlobTypeDef,
+        "vnfPkgId": str,
     },
 )
-
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+_OptionalValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalValidateSolFunctionPackageContentInputRequestTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "contentType": Literal["application/zip"],
     },
+    total=False,
 )
 
-_RequiredTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
-    "_RequiredTerminateSolNetworkInstanceInputRequestTypeDef",
+class ValidateSolFunctionPackageContentInputRequestTypeDef(
+    _RequiredValidateSolFunctionPackageContentInputRequestTypeDef,
+    _OptionalValidateSolFunctionPackageContentInputRequestTypeDef,
+):
+    pass
+
+_RequiredValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_RequiredValidateSolNetworkPackageContentInputRequestTypeDef",
     {
-        "nsInstanceId": str,
+        "file": BlobTypeDef,
+        "nsdInfoId": str,
     },
 )
-_OptionalTerminateSolNetworkInstanceInputRequestTypeDef = TypedDict(
-    "_OptionalTerminateSolNetworkInstanceInputRequestTypeDef",
+_OptionalValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
+    "_OptionalValidateSolNetworkPackageContentInputRequestTypeDef",
     {
-        "tags": Mapping[str, str],
+        "contentType": Literal["application/zip"],
     },
     total=False,
 )
 
-class TerminateSolNetworkInstanceInputRequestTypeDef(
-    _RequiredTerminateSolNetworkInstanceInputRequestTypeDef,
-    _OptionalTerminateSolNetworkInstanceInputRequestTypeDef,
+class ValidateSolNetworkPackageContentInputRequestTypeDef(
+    _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
+    _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
 ):
     pass
 
-TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "TerminateSolNetworkInstanceOutputTypeDef",
+CreateSolFunctionPackageOutputTypeDef = TypedDict(
+    "CreateSolFunctionPackageOutputTypeDef",
     {
-        "nsLcmOpOccId": str,
+        "arn": str,
+        "id": str,
+        "onboardingState": OnboardingStateType,
+        "operationalState": OperationalStateType,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "usageState": UsageStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
+CreateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "CreateSolNetworkInstanceOutputTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "arn": str,
+        "id": str,
+        "nsInstanceName": str,
+        "nsdInfoId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolFunctionPackageInputRequestTypeDef = TypedDict(
-    "UpdateSolFunctionPackageInputRequestTypeDef",
+CreateSolNetworkPackageOutputTypeDef = TypedDict(
+    "CreateSolNetworkPackageOutputTypeDef",
     {
-        "operationalState": OperationalStateType,
-        "vnfPkgId": str,
+        "arn": str,
+        "id": str,
+        "nsdOnboardingState": NsdOnboardingStateType,
+        "nsdOperationalState": NsdOperationalStateType,
+        "nsdUsageState": NsdUsageStateType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolFunctionPackageOutputTypeDef = TypedDict(
-    "UpdateSolFunctionPackageOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "operationalState": OperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkModifyTypeDef = TypedDict(
-    "UpdateSolNetworkModifyTypeDef",
+GetSolFunctionPackageContentOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageContentOutputTypeDef",
     {
-        "vnfConfigurableProperties": Mapping[str, Any],
-        "vnfInstanceId": str,
+        "contentType": Literal["application/zip"],
+        "packageContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
-    "UpdateSolNetworkInstanceOutputTypeDef",
+GetSolFunctionPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolFunctionPackageDescriptorOutputTypeDef",
     {
-        "nsLcmOpOccId": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "contentType": Literal["text/plain"],
+        "vnfd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkPackageInputRequestTypeDef = TypedDict(
-    "UpdateSolNetworkPackageInputRequestTypeDef",
+GetSolNetworkPackageContentOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageContentOutputTypeDef",
     {
-        "nsdInfoId": str,
-        "nsdOperationalState": NsdOperationalStateType,
+        "contentType": Literal["application/zip"],
+        "nsdContent": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSolNetworkPackageOutputTypeDef = TypedDict(
-    "UpdateSolNetworkPackageOutputTypeDef",
+GetSolNetworkPackageDescriptorOutputTypeDef = TypedDict(
+    "GetSolNetworkPackageDescriptorOutputTypeDef",
     {
-        "nsdOperationalState": NsdOperationalStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "contentType": Literal["text/plain"],
+        "nsd": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredValidateSolFunctionPackageContentInputRequestTypeDef",
+InstantiateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "InstantiateSolNetworkInstanceOutputTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "vnfPkgId": str,
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValidateSolFunctionPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalValidateSolFunctionPackageContentInputRequestTypeDef",
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
     {
-        "contentType": Literal["application/zip"],
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ValidateSolFunctionPackageContentInputRequestTypeDef(
-    _RequiredValidateSolFunctionPackageContentInputRequestTypeDef,
-    _OptionalValidateSolFunctionPackageContentInputRequestTypeDef,
-):
-    pass
+TerminateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "TerminateSolNetworkInstanceOutputTypeDef",
+    {
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_RequiredValidateSolNetworkPackageContentInputRequestTypeDef",
+UpdateSolFunctionPackageOutputTypeDef = TypedDict(
+    "UpdateSolFunctionPackageOutputTypeDef",
     {
-        "file": Union[str, bytes, IO[Any], StreamingBody],
-        "nsdInfoId": str,
+        "operationalState": OperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValidateSolNetworkPackageContentInputRequestTypeDef = TypedDict(
-    "_OptionalValidateSolNetworkPackageContentInputRequestTypeDef",
+
+UpdateSolNetworkInstanceOutputTypeDef = TypedDict(
+    "UpdateSolNetworkInstanceOutputTypeDef",
     {
-        "contentType": Literal["application/zip"],
+        "nsLcmOpOccId": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ValidateSolNetworkPackageContentInputRequestTypeDef(
-    _RequiredValidateSolNetworkPackageContentInputRequestTypeDef,
-    _OptionalValidateSolNetworkPackageContentInputRequestTypeDef,
-):
-    pass
+UpdateSolNetworkPackageOutputTypeDef = TypedDict(
+    "UpdateSolNetworkPackageOutputTypeDef",
+    {
+        "nsdOperationalState": NsdOperationalStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetSolNetworkOperationTaskDetailsTypeDef = TypedDict(
     "GetSolNetworkOperationTaskDetailsTypeDef",
     {
         "taskContext": Dict[str, str],
         "taskEndTime": datetime,
         "taskErrorDetails": ErrorInfoTypeDef,
@@ -848,15 +810,15 @@
         "metadata": GetSolNetworkInstanceMetadataTypeDef,
         "nsInstanceDescription": str,
         "nsInstanceName": str,
         "nsState": NsStateType,
         "nsdId": str,
         "nsdInfoId": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolVnfcResourceInfoTypeDef = TypedDict(
     "GetSolVnfcResourceInfoTypeDef",
     {
         "metadata": GetSolVnfcResourceInfoMetadataTypeDef,
@@ -885,14 +847,54 @@
 )
 
 class ListSolFunctionInstanceInfoTypeDef(
     _RequiredListSolFunctionInstanceInfoTypeDef, _OptionalListSolFunctionInstanceInfoTypeDef
 ):
     pass
 
+ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef = TypedDict(
+    "ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef = TypedDict(
+    "ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef = TypedDict(
+    "ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef = TypedDict(
+    "ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef = TypedDict(
+    "ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredListSolFunctionPackageInfoTypeDef = TypedDict(
     "_RequiredListSolFunctionPackageInfoTypeDef",
     {
         "arn": str,
         "id": str,
         "onboardingState": OnboardingStateType,
         "operationalState": OperationalStateType,
@@ -1013,15 +1015,15 @@
         "id": str,
         "lcmOperationType": LcmOperationTypeType,
         "metadata": GetSolNetworkOperationMetadataTypeDef,
         "nsInstanceId": str,
         "operationState": NsLcmOperationStateType,
         "tags": Dict[str, str],
         "tasks": List[GetSolNetworkOperationTaskDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSolFunctionPackageMetadataTypeDef = TypedDict(
     "_RequiredGetSolFunctionPackageMetadataTypeDef",
     {
         "createdAt": datetime,
@@ -1103,51 +1105,51 @@
 )
 
 ListSolFunctionInstancesOutputTypeDef = TypedDict(
     "ListSolFunctionInstancesOutputTypeDef",
     {
         "functionInstances": List[ListSolFunctionInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolFunctionPackagesOutputTypeDef = TypedDict(
     "ListSolFunctionPackagesOutputTypeDef",
     {
         "functionPackages": List[ListSolFunctionPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkInstancesOutputTypeDef = TypedDict(
     "ListSolNetworkInstancesOutputTypeDef",
     {
         "networkInstances": List[ListSolNetworkInstanceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkOperationsOutputTypeDef = TypedDict(
     "ListSolNetworkOperationsOutputTypeDef",
     {
         "networkOperations": List[ListSolNetworkOperationsInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSolNetworkPackagesOutputTypeDef = TypedDict(
     "ListSolNetworkPackagesOutputTypeDef",
     {
         "networkPackages": List[ListSolNetworkPackageInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionPackageOutputTypeDef = TypedDict(
     "GetSolFunctionPackageOutputTypeDef",
     {
         "arn": str,
@@ -1157,41 +1159,41 @@
         "operationalState": OperationalStateType,
         "tags": Dict[str, str],
         "usageState": UsageStateType,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolFunctionPackageContentOutputTypeDef = TypedDict(
     "PutSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": PutSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolFunctionPackageContentOutputTypeDef = TypedDict(
     "ValidateSolFunctionPackageContentOutputTypeDef",
     {
         "id": str,
         "metadata": ValidateSolFunctionPackageContentMetadataTypeDef,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolNetworkPackageOutputTypeDef = TypedDict(
     "GetSolNetworkPackageOutputTypeDef",
     {
         "arn": str,
@@ -1201,43 +1203,43 @@
         "nsdName": str,
         "nsdOnboardingState": NsdOnboardingStateType,
         "nsdOperationalState": NsdOperationalStateType,
         "nsdUsageState": NsdUsageStateType,
         "nsdVersion": str,
         "tags": Dict[str, str],
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSolNetworkPackageContentOutputTypeDef = TypedDict(
     "PutSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": PutSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateSolNetworkPackageContentOutputTypeDef = TypedDict(
     "ValidateSolNetworkPackageContentOutputTypeDef",
     {
         "arn": str,
         "id": str,
         "metadata": ValidateSolNetworkPackageContentMetadataTypeDef,
         "nsdId": str,
         "nsdName": str,
         "nsdVersion": str,
         "vnfPkgIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSolFunctionInstanceOutputTypeDef = TypedDict(
     "GetSolFunctionInstanceOutputTypeDef",
     {
         "arn": str,
@@ -1248,10 +1250,10 @@
         "nsInstanceId": str,
         "tags": Dict[str, str],
         "vnfPkgId": str,
         "vnfProductName": str,
         "vnfProvider": str,
         "vnfdId": str,
         "vnfdVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/PKG-INFO` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-tnb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore tnb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore tnb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-tnb"></a>
 
 # types-aiobotocore-tnb
 
 [![PyPI - types-aiobotocore-tnb](https://img.shields.io/pypi/v/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-tnb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-tnb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-tnb?color=blue)](https://pypistats.org/packages/types-aiobotocore-tnb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-tnb)](https://pepy.tech/project/types-aiobotocore-tnb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TelcoNetworkBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder)
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
 [types-aiobotocore-tnb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb/).
 
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
@@ -342,97 +341,98 @@
 )
 
 
 def check_value(value: DescriptorContentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_tnb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_tnb.type_defs import (
+    BlobTypeDef,
     CancelSolNetworkOperationInputRequestTypeDef,
     CreateSolFunctionPackageInputRequestTypeDef,
-    CreateSolFunctionPackageOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSolNetworkInstanceInputRequestTypeDef,
-    CreateSolNetworkInstanceOutputTypeDef,
     CreateSolNetworkPackageInputRequestTypeDef,
-    CreateSolNetworkPackageOutputTypeDef,
     DeleteSolFunctionPackageInputRequestTypeDef,
     DeleteSolNetworkInstanceInputRequestTypeDef,
     DeleteSolNetworkPackageInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     ToscaOverrideTypeDef,
     GetSolFunctionInstanceInputRequestTypeDef,
     GetSolFunctionInstanceMetadataTypeDef,
     GetSolFunctionPackageContentInputRequestTypeDef,
-    GetSolFunctionPackageContentOutputTypeDef,
     GetSolFunctionPackageDescriptorInputRequestTypeDef,
-    GetSolFunctionPackageDescriptorOutputTypeDef,
     GetSolFunctionPackageInputRequestTypeDef,
     GetSolInstantiatedVnfInfoTypeDef,
     GetSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkInstanceMetadataTypeDef,
     LcmOperationInfoTypeDef,
     GetSolNetworkOperationInputRequestTypeDef,
     GetSolNetworkOperationMetadataTypeDef,
     ProblemDetailsTypeDef,
     GetSolNetworkPackageContentInputRequestTypeDef,
-    GetSolNetworkPackageContentOutputTypeDef,
     GetSolNetworkPackageDescriptorInputRequestTypeDef,
-    GetSolNetworkPackageDescriptorOutputTypeDef,
     GetSolNetworkPackageInputRequestTypeDef,
     GetSolVnfcResourceInfoMetadataTypeDef,
     InstantiateSolNetworkInstanceInputRequestTypeDef,
-    InstantiateSolNetworkInstanceOutputTypeDef,
     ListSolFunctionInstanceMetadataTypeDef,
-    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSolFunctionInstancesInputRequestTypeDef,
     ListSolFunctionPackageMetadataTypeDef,
-    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
     ListSolFunctionPackagesInputRequestTypeDef,
     ListSolNetworkInstanceMetadataTypeDef,
-    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
     ListSolNetworkInstancesInputRequestTypeDef,
     ListSolNetworkOperationsMetadataTypeDef,
-    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
     ListSolNetworkOperationsInputRequestTypeDef,
     ListSolNetworkPackageMetadataTypeDef,
-    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolNetworkPackagesInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
-    PutSolFunctionPackageContentInputRequestTypeDef,
-    PutSolNetworkPackageContentInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     TerminateSolNetworkInstanceInputRequestTypeDef,
-    TerminateSolNetworkInstanceOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateSolFunctionPackageInputRequestTypeDef,
-    UpdateSolFunctionPackageOutputTypeDef,
     UpdateSolNetworkModifyTypeDef,
-    UpdateSolNetworkInstanceOutputTypeDef,
     UpdateSolNetworkPackageInputRequestTypeDef,
-    UpdateSolNetworkPackageOutputTypeDef,
+    PutSolFunctionPackageContentInputRequestTypeDef,
+    PutSolNetworkPackageContentInputRequestTypeDef,
     ValidateSolFunctionPackageContentInputRequestTypeDef,
     ValidateSolNetworkPackageContentInputRequestTypeDef,
+    CreateSolFunctionPackageOutputTypeDef,
+    CreateSolNetworkInstanceOutputTypeDef,
+    CreateSolNetworkPackageOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetSolFunctionPackageContentOutputTypeDef,
+    GetSolFunctionPackageDescriptorOutputTypeDef,
+    GetSolNetworkPackageContentOutputTypeDef,
+    GetSolNetworkPackageDescriptorOutputTypeDef,
+    InstantiateSolNetworkInstanceOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    TerminateSolNetworkInstanceOutputTypeDef,
+    UpdateSolFunctionPackageOutputTypeDef,
+    UpdateSolNetworkInstanceOutputTypeDef,
+    UpdateSolNetworkPackageOutputTypeDef,
     GetSolNetworkOperationTaskDetailsTypeDef,
     FunctionArtifactMetaTypeDef,
     NetworkArtifactMetaTypeDef,
     GetSolNetworkInstanceOutputTypeDef,
     GetSolVnfcResourceInfoTypeDef,
     ListSolFunctionInstanceInfoTypeDef,
+    ListSolFunctionInstancesInputListSolFunctionInstancesPaginateTypeDef,
+    ListSolFunctionPackagesInputListSolFunctionPackagesPaginateTypeDef,
+    ListSolNetworkInstancesInputListSolNetworkInstancesPaginateTypeDef,
+    ListSolNetworkOperationsInputListSolNetworkOperationsPaginateTypeDef,
+    ListSolNetworkPackagesInputListSolNetworkPackagesPaginateTypeDef,
     ListSolFunctionPackageInfoTypeDef,
     ListSolNetworkInstanceInfoTypeDef,
     ListSolNetworkOperationsInfoTypeDef,
     ListSolNetworkPackageInfoTypeDef,
     UpdateSolNetworkInstanceInputRequestTypeDef,
     GetSolNetworkOperationOutputTypeDef,
     GetSolFunctionPackageMetadataTypeDef,
@@ -453,15 +453,15 @@
     GetSolNetworkPackageOutputTypeDef,
     PutSolNetworkPackageContentOutputTypeDef,
     ValidateSolNetworkPackageContentOutputTypeDef,
     GetSolFunctionInstanceOutputTypeDef,
 )
 
 
-def get_structure() -> CancelSolNetworkOperationInputRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-tnb-2.5.2/types_aiobotocore_tnb.egg-info/SOURCES.txt` & `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


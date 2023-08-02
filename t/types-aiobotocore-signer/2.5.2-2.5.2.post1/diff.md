# Comparing `tmp/types-aiobotocore-signer-2.5.2.tar.gz` & `tmp/types-aiobotocore-signer-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-signer-2.5.2.tar", last modified: Sat Jul  8 01:44:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-signer-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
```

## Comparing `types-aiobotocore-signer-2.5.2.tar` & `types-aiobotocore-signer-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.366908 types-aiobotocore-signer-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-08 01:44:20.362908 types-aiobotocore-signer-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:20.366908 types-aiobotocore-signer-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.362908 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-07-08 01:41:10.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21566 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-08 01:41:09.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.362908 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-08 01:44:20.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 01:44:20.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:20.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:44:20.000000 types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.729455 types-aiobotocore-signer-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-02 14:53:01.725455 types-aiobotocore-signer-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.729455 types-aiobotocore-signer-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.721455 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18592 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-08-02 14:49:47.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.725455 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-signer-2.5.2/LICENSE` & `types-aiobotocore-signer-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/PKG-INFO` & `types-aiobotocore-signer-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-signer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore signer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore signer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-signer"></a>
 
 # types-aiobotocore-signer
 
 [![PyPI - types-aiobotocore-signer](https://img.shields.io/pypi/v/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-signer?color=blue)](https://pypistats.org/packages/types-aiobotocore-signer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.signer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -352,71 +351,73 @@
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_signer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
-    GetRevocationStatusResponseTypeDef,
+    TimestampTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
-    SignPayloadRequestRequestTypeDef,
-    SignPayloadResponseTypeDef,
     SigningConfigurationOverridesTypeDef,
-    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AddProfilePermissionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutSigningProfileResponseTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    SignPayloadResponseTypeDef,
+    StartSigningJobResponseTypeDef,
+    SignPayloadRequestRequestTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    ListSigningJobsRequestRequestTypeDef,
+    RevokeSigningProfileRequestRequestTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
     SourceTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
@@ -425,15 +426,15 @@
     GetSigningProfileResponseTypeDef,
     PutSigningProfileRequestRequestTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
 )
 
 
-def get_structure() -> AddProfilePermissionRequestRequestTypeDef:
+def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-signer-2.5.2/README.md` & `types-aiobotocore-signer-2.5.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-signer"></a>
 
 # types-aiobotocore-signer
 
 [![PyPI - types-aiobotocore-signer](https://img.shields.io/pypi/v/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-signer?color=blue)](https://pypistats.org/packages/types-aiobotocore-signer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.signer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -319,71 +319,73 @@
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_signer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
-    GetRevocationStatusResponseTypeDef,
+    TimestampTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
-    SignPayloadRequestRequestTypeDef,
-    SignPayloadResponseTypeDef,
     SigningConfigurationOverridesTypeDef,
-    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AddProfilePermissionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutSigningProfileResponseTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    SignPayloadResponseTypeDef,
+    StartSigningJobResponseTypeDef,
+    SignPayloadRequestRequestTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    ListSigningJobsRequestRequestTypeDef,
+    RevokeSigningProfileRequestRequestTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
     SourceTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
@@ -392,15 +394,15 @@
     GetSigningProfileResponseTypeDef,
     PutSigningProfileRequestRequestTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
 )
 
 
-def get_structure() -> AddProfilePermissionRequestRequestTypeDef:
+def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-signer-2.5.2/setup.py` & `types-aiobotocore-signer-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-signer",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore signer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore signer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_signer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/"
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/__init__.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/__init__.pyi` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/__main__.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.signer 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.signer 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/client.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 
     session = get_session()
     async with session.create_client("signer") as client:
         client: signerClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .type_defs import (
     AddProfilePermissionResponseTypeDef,
+    BlobTypeDef,
     DescribeSigningJobResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     GetSigningProfileResponseTypeDef,
     ListProfilePermissionsResponseTypeDef,
@@ -45,48 +44,45 @@
     RemoveProfilePermissionResponseTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningMaterialTypeDef,
     SigningPlatformOverridesTypeDef,
     SignPayloadResponseTypeDef,
     SourceTypeDef,
     StartSigningJobResponseTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("signerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class signerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/)
     """
 
     meta: ClientMeta
@@ -95,15 +91,14 @@
     def exceptions(self) -> Exceptions:
         """
         signerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#exceptions)
         """
-
     async def add_profile_permission(
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
@@ -112,126 +107,115 @@
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#add_profile_permission)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#can_paginate)
         """
-
     async def cancel_signing_profile(self, *, profileName: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of an `ACTIVE` signing profile to `CANCELED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#cancel_signing_profile)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#close)
         """
-
     async def describe_signing_job(self, *, jobId: str) -> DescribeSigningJobResponseTypeDef:
         """
         Returns information about a specific code signing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#describe_signing_job)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#generate_presigned_url)
         """
-
     async def get_revocation_status(
         self,
         *,
-        signatureTimestamp: Union[datetime, str],
+        signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
         certificateHashes: Sequence[str]
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_revocation_status)
         """
-
     async def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_signing_platform)
         """
-
     async def get_signing_profile(
         self, *, profileName: str, profileOwner: str = ...
     ) -> GetSigningProfileResponseTypeDef:
         """
         Returns information on a specific signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_signing_profile)
         """
-
     async def list_profile_permissions(
         self, *, profileName: str, nextToken: str = ...
     ) -> ListProfilePermissionsResponseTypeDef:
         """
         Lists the cross-account permissions associated with a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_profile_permissions)
         """
-
     async def list_signing_jobs(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_jobs)
         """
-
     async def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
@@ -240,15 +224,14 @@
         """
         Lists all signing platforms available in code signing that match the request
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_platforms)
         """
-
     async def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
@@ -256,25 +239,23 @@
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_profiles)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with a signing profile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_tags_for_resource)
         """
-
     async def put_signing_profile(
         self,
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
@@ -284,65 +265,50 @@
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#put_signing_profile)
         """
-
     async def remove_profile_permission(
         self, *, profileName: str, revisionId: str, statementId: str
     ) -> RemoveProfilePermissionResponseTypeDef:
         """
         Removes cross-account permissions from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#remove_profile_permission)
         """
-
     async def revoke_signature(
         self, *, jobId: str, reason: str, jobOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing job to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#revoke_signature)
         """
-
     async def revoke_signing_profile(
-        self,
-        *,
-        profileName: str,
-        profileVersion: str,
-        reason: str,
-        effectiveTime: Union[datetime, str]
+        self, *, profileName: str, profileVersion: str, reason: str, effectiveTime: TimestampTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#revoke_signing_profile)
         """
-
     async def sign_payload(
-        self,
-        *,
-        profileName: str,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
-        payloadFormat: str,
-        profileOwner: str = ...
+        self, *, profileName: str, payload: BlobTypeDef, payloadFormat: str, profileOwner: str = ...
     ) -> SignPayloadResponseTypeDef:
         """
         Signs a binary payload and returns a signature envelope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#sign_payload)
         """
-
     async def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
@@ -350,70 +316,62 @@
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#start_signing_job)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#untag_resource)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_jobs"]
     ) -> ListSigningJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_platforms"]
     ) -> ListSigningPlatformsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_profiles"]
     ) -> ListSigningProfilesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_paginator)
         """
-
     def get_waiter(
         self, waiter_name: Literal["successful_signing_job"]
     ) -> SuccessfulSigningJobWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "signerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/)
         """
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/client.pyi` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 
     session = get_session()
     async with session.create_client("signer") as client:
         client: signerClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .type_defs import (
     AddProfilePermissionResponseTypeDef,
+    BlobTypeDef,
     DescribeSigningJobResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     GetSigningProfileResponseTypeDef,
     ListProfilePermissionsResponseTypeDef,
@@ -45,44 +44,49 @@
     RemoveProfilePermissionResponseTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningMaterialTypeDef,
     SigningPlatformOverridesTypeDef,
     SignPayloadResponseTypeDef,
     SourceTypeDef,
     StartSigningJobResponseTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("signerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServiceErrorException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceLimitExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class signerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/)
     """
 
     meta: ClientMeta
@@ -91,14 +95,15 @@
     def exceptions(self) -> Exceptions:
         """
         signerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#exceptions)
         """
+
     async def add_profile_permission(
         self,
         *,
         profileName: str,
         action: str,
         principal: str,
         statementId: str,
@@ -107,115 +112,126 @@
     ) -> AddProfilePermissionResponseTypeDef:
         """
         Adds cross-account permissions to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.add_profile_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#add_profile_permission)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#can_paginate)
         """
+
     async def cancel_signing_profile(self, *, profileName: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of an `ACTIVE` signing profile to `CANCELED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.cancel_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#cancel_signing_profile)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#close)
         """
+
     async def describe_signing_job(self, *, jobId: str) -> DescribeSigningJobResponseTypeDef:
         """
         Returns information about a specific code signing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.describe_signing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#describe_signing_job)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#generate_presigned_url)
         """
+
     async def get_revocation_status(
         self,
         *,
-        signatureTimestamp: Union[datetime, str],
+        signatureTimestamp: TimestampTypeDef,
         platformId: str,
         profileVersionArn: str,
         jobArn: str,
         certificateHashes: Sequence[str]
     ) -> GetRevocationStatusResponseTypeDef:
         """
         Retrieves the revocation status of one or more of the signing profile, signing
         job, and signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_revocation_status)
         """
+
     async def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_signing_platform)
         """
+
     async def get_signing_profile(
         self, *, profileName: str, profileOwner: str = ...
     ) -> GetSigningProfileResponseTypeDef:
         """
         Returns information on a specific signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_signing_profile)
         """
+
     async def list_profile_permissions(
         self, *, profileName: str, nextToken: str = ...
     ) -> ListProfilePermissionsResponseTypeDef:
         """
         Lists the cross-account permissions associated with a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_profile_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_profile_permissions)
         """
+
     async def list_signing_jobs(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...
     ) -> ListSigningJobsResponseTypeDef:
         """
         Lists all your signing jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_jobs)
         """
+
     async def list_signing_platforms(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
         maxResults: int = ...,
@@ -224,14 +240,15 @@
         """
         Lists all signing platforms available in code signing that match the request
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_platforms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_platforms)
         """
+
     async def list_signing_profiles(
         self,
         *,
         includeCanceled: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         platformId: str = ...,
@@ -239,23 +256,25 @@
     ) -> ListSigningProfilesResponseTypeDef:
         """
         Lists all available signing profiles in your AWS account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_signing_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_signing_profiles)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Returns a list of the tags associated with a signing profile resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#list_tags_for_resource)
         """
+
     async def put_signing_profile(
         self,
         *,
         profileName: str,
         platformId: str,
         signingMaterial: SigningMaterialTypeDef = ...,
         signatureValidityPeriod: SignatureValidityPeriodTypeDef = ...,
@@ -265,60 +284,55 @@
     ) -> PutSigningProfileResponseTypeDef:
         """
         Creates a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.put_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#put_signing_profile)
         """
+
     async def remove_profile_permission(
         self, *, profileName: str, revisionId: str, statementId: str
     ) -> RemoveProfilePermissionResponseTypeDef:
         """
         Removes cross-account permissions from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.remove_profile_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#remove_profile_permission)
         """
+
     async def revoke_signature(
         self, *, jobId: str, reason: str, jobOwner: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing job to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signature)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#revoke_signature)
         """
+
     async def revoke_signing_profile(
-        self,
-        *,
-        profileName: str,
-        profileVersion: str,
-        reason: str,
-        effectiveTime: Union[datetime, str]
+        self, *, profileName: str, profileVersion: str, reason: str, effectiveTime: TimestampTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#revoke_signing_profile)
         """
+
     async def sign_payload(
-        self,
-        *,
-        profileName: str,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
-        payloadFormat: str,
-        profileOwner: str = ...
+        self, *, profileName: str, payload: BlobTypeDef, payloadFormat: str, profileOwner: str = ...
     ) -> SignPayloadResponseTypeDef:
         """
         Signs a binary payload and returns a signature envelope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#sign_payload)
         """
+
     async def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
@@ -326,62 +340,70 @@
     ) -> StartSigningJobResponseTypeDef:
         """
         Initiates a signing job to be performed on the code provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.start_signing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#start_signing_job)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from a signing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#untag_resource)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_jobs"]
     ) -> ListSigningJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_platforms"]
     ) -> ListSigningPlatformsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_signing_profiles"]
     ) -> ListSigningProfilesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_paginator)
         """
+
     def get_waiter(
         self, waiter_name: Literal["successful_signing_job"]
     ) -> SuccessfulSigningJobWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "signerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/client/)
         """
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/literals.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/literals.pyi` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/paginator.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,26 @@
         client: signerClient
 
         list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
         list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
         list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .type_defs import (
     ListSigningJobsResponseTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningProfilesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
@@ -64,18 +64,18 @@
     def paginate(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningjobspaginator)
         """
 
 
@@ -87,15 +87,15 @@
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningplatformspaginator)
         """
 
 
@@ -107,13 +107,13 @@
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/paginator.pyi` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -20,26 +20,26 @@
         client: signerClient
 
         list_signing_jobs_paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
         list_signing_platforms_paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
         list_signing_profiles_paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .type_defs import (
     ListSigningJobsResponseTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningProfilesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListSigningJobsPaginator",
     "ListSigningPlatformsPaginator",
     "ListSigningProfilesPaginator",
 )
@@ -61,18 +61,18 @@
     def paginate(
         self,
         *,
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
-        signatureExpiresBefore: Union[datetime, str] = ...,
-        signatureExpiresAfter: Union[datetime, str] = ...,
+        signatureExpiresBefore: TimestampTypeDef = ...,
+        signatureExpiresAfter: TimestampTypeDef = ...,
         jobInvoker: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningjobspaginator)
         """
 
 class ListSigningPlatformsPaginator(AioPaginator):
@@ -83,15 +83,15 @@
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningplatformspaginator)
         """
 
 class ListSigningProfilesPaginator(AioPaginator):
@@ -102,13 +102,13 @@
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/type_defs.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
-    data: AddProfilePermissionRequestRequestTypeDef = {...}
+    data: AddProfilePermissionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -34,61 +34,63 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
-    "AddProfilePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
     "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
-    "GetRevocationStatusRequestRequestTypeDef",
-    "GetRevocationStatusResponseTypeDef",
+    "TimestampTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
     "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    "ListSigningJobsRequestRequestTypeDef",
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutSigningProfileResponseTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
-    "RemoveProfilePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
-    "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
     "S3SourceTypeDef",
-    "SignPayloadRequestRequestTypeDef",
-    "SignPayloadResponseTypeDef",
     "SigningConfigurationOverridesTypeDef",
-    "StartSigningJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AddProfilePermissionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetRevocationStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutSigningProfileResponseTypeDef",
+    "RemoveProfilePermissionResponseTypeDef",
+    "SignPayloadResponseTypeDef",
+    "StartSigningJobResponseTypeDef",
+    "SignPayloadRequestRequestTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
+    "GetRevocationStatusRequestRequestTypeDef",
+    "ListSigningJobsRequestRequestTypeDef",
+    "RevokeSigningProfileRequestRequestTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
     "SourceTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
@@ -122,22 +124,26 @@
 class AddProfilePermissionRequestRequestTypeDef(
     _RequiredAddProfilePermissionRequestRequestTypeDef,
     _OptionalAddProfilePermissionRequestRequestTypeDef,
 ):
     pass
 
 
-AddProfilePermissionResponseTypeDef = TypedDict(
-    "AddProfilePermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
     },
 )
 
@@ -179,48 +185,23 @@
     {
         "bucketName": str,
         "prefix": str,
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
 EncryptionAlgorithmOptionsTypeDef = TypedDict(
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
 
-GetRevocationStatusRequestRequestTypeDef = TypedDict(
-    "GetRevocationStatusRequestRequestTypeDef",
-    {
-        "signatureTimestamp": Union[datetime, str],
-        "platformId": str,
-        "profileVersionArn": str,
-        "jobArn": str,
-        "certificateHashes": Sequence[str],
-    },
-)
-
-GetRevocationStatusResponseTypeDef = TypedDict(
-    "GetRevocationStatusResponseTypeDef",
-    {
-        "revokedEntities": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -309,52 +290,20 @@
         "principal": str,
         "statementId": str,
         "profileVersion": str,
     },
     total=False,
 )
 
-ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSigningJobsRequestRequestTypeDef = TypedDict(
-    "ListSigningJobsRequestRequestTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "maxResults": int,
-        "nextToken": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-    },
-    total=False,
-)
-
-ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "category": str,
-        "partner": str,
-        "target": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
@@ -363,25 +312,14 @@
         "target": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
-    {
-        "includeCanceled": bool,
-        "platformId": str,
-        "statuses": Sequence[SigningProfileStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningProfilesRequestRequestTypeDef = TypedDict(
     "ListSigningProfilesRequestRequestTypeDef",
     {
         "includeCanceled": bool,
         "maxResults": int,
         "nextToken": str,
         "platformId": str,
@@ -393,70 +331,23 @@
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
-PutSigningProfileResponseTypeDef = TypedDict(
-    "PutSigningProfileResponseTypeDef",
-    {
-        "arn": str,
-        "profileVersion": str,
-        "profileVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
 )
 
-RemoveProfilePermissionResponseTypeDef = TypedDict(
-    "RemoveProfilePermissionResponseTypeDef",
-    {
-        "revisionId": str,
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
 _RequiredRevokeSignatureRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeSignatureRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
@@ -471,24 +362,14 @@
 
 class RevokeSignatureRequestRequestTypeDef(
     _RequiredRevokeSignatureRequestRequestTypeDef, _OptionalRevokeSignatureRequestRequestTypeDef
 ):
     pass
 
 
-RevokeSigningProfileRequestRequestTypeDef = TypedDict(
-    "RevokeSigningProfileRequestRequestTypeDef",
-    {
-        "profileName": str,
-        "profileVersion": str,
-        "reason": str,
-        "effectiveTime": Union[datetime, str],
-    },
-)
-
 S3SignedObjectTypeDef = TypedDict(
     "S3SignedObjectTypeDef",
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
@@ -499,82 +380,131 @@
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
 )
 
-_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
-    "_RequiredSignPayloadRequestRequestTypeDef",
+SigningConfigurationOverridesTypeDef = TypedDict(
+    "SigningConfigurationOverridesTypeDef",
     {
-        "profileName": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-        "payloadFormat": str,
+        "encryptionAlgorithm": EncryptionAlgorithmType,
+        "hashAlgorithm": HashAlgorithmType,
     },
+    total=False,
 )
-_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
-    "_OptionalSignPayloadRequestRequestTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "profileOwner": str,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
-    total=False,
 )
 
+AddProfilePermissionResponseTypeDef = TypedDict(
+    "AddProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class SignPayloadRequestRequestTypeDef(
-    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
-):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRevocationStatusResponseTypeDef = TypedDict(
+    "GetRevocationStatusResponseTypeDef",
+    {
+        "revokedEntities": List[str],
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
+PutSigningProfileResponseTypeDef = TypedDict(
+    "PutSigningProfileResponseTypeDef",
+    {
+        "arn": str,
+        "profileVersion": str,
+        "profileVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+RemoveProfilePermissionResponseTypeDef = TypedDict(
+    "RemoveProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 SignPayloadResponseTypeDef = TypedDict(
     "SignPayloadResponseTypeDef",
     {
         "jobId": str,
         "jobOwner": str,
         "metadata": Dict[str, str],
         "signature": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SigningConfigurationOverridesTypeDef = TypedDict(
-    "SigningConfigurationOverridesTypeDef",
-    {
-        "encryptionAlgorithm": EncryptionAlgorithmType,
-        "hashAlgorithm": HashAlgorithmType,
-    },
-    total=False,
-)
-
 StartSigningJobResponseTypeDef = TypedDict(
     "StartSigningJobResponseTypeDef",
     {
         "jobId": str,
         "jobOwner": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
+    "_RequiredSignPayloadRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "profileName": str,
+        "payload": BlobTypeDef,
+        "payloadFormat": str,
     },
 )
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
+    "_OptionalSignPayloadRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "profileOwner": str,
     },
+    total=False,
 )
 
+
+class SignPayloadRequestRequestTypeDef(
+    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
@@ -597,14 +527,51 @@
     "DestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
     },
     total=False,
 )
 
+GetRevocationStatusRequestRequestTypeDef = TypedDict(
+    "GetRevocationStatusRequestRequestTypeDef",
+    {
+        "signatureTimestamp": TimestampTypeDef,
+        "platformId": str,
+        "profileVersionArn": str,
+        "jobArn": str,
+        "certificateHashes": Sequence[str],
+    },
+)
+
+ListSigningJobsRequestRequestTypeDef = TypedDict(
+    "ListSigningJobsRequestRequestTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "maxResults": int,
+        "nextToken": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
+        "jobInvoker": str,
+    },
+    total=False,
+)
+
+RevokeSigningProfileRequestRequestTypeDef = TypedDict(
+    "RevokeSigningProfileRequestRequestTypeDef",
+    {
+        "profileName": str,
+        "profileVersion": str,
+        "reason": str,
+        "effectiveTime": TimestampTypeDef,
+    },
+)
+
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "signingMaterial": SigningMaterialTypeDef,
@@ -630,18 +597,55 @@
 ListProfilePermissionsResponseTypeDef = TypedDict(
     "ListProfilePermissionsResponseTypeDef",
     {
         "revisionId": str,
         "policySizeBytes": int,
         "permissions": List[PermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
+        "jobInvoker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    {
+        "category": str,
+        "partner": str,
+        "target": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
+    {
+        "includeCanceled": bool,
+        "platformId": str,
+        "statuses": Sequence[SigningProfileStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 SignedObjectTypeDef = TypedDict(
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
     total=False,
 )
@@ -664,15 +668,15 @@
 )
 
 ListSigningProfilesResponseTypeDef = TypedDict(
     "ListSigningProfilesResponseTypeDef",
     {
         "profiles": List[SigningProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningPlatformResponseTypeDef = TypedDict(
     "GetSigningPlatformResponseTypeDef",
     {
         "platformId": str,
@@ -680,15 +684,15 @@
         "partner": str,
         "target": str,
         "category": Literal["AWSIoT"],
         "signingConfiguration": SigningConfigurationTypeDef,
         "signingImageFormat": SigningImageFormatTypeDef,
         "maxSizeInMB": int,
         "revocationSupported": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SigningPlatformTypeDef = TypedDict(
     "SigningPlatformTypeDef",
     {
         "platformId": str,
@@ -767,15 +771,15 @@
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
         "revocationRecord": SigningJobRevocationRecordTypeDef,
         "signedObject": SignedObjectTypeDef,
         "jobOwner": str,
         "jobInvoker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
@@ -788,15 +792,15 @@
         "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
         "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSigningProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPutSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -823,19 +827,19 @@
 
 
 ListSigningPlatformsResponseTypeDef = TypedDict(
     "ListSigningPlatformsResponseTypeDef",
     {
         "platforms": List[SigningPlatformTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSigningJobsResponseTypeDef = TypedDict(
     "ListSigningJobsResponseTypeDef",
     {
         "jobs": List[SigningJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/type_defs.pyi` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
-    data: AddProfilePermissionRequestRequestTypeDef = {...}
+    data: AddProfilePermissionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,61 +33,63 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
-    "AddProfilePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
     "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
-    "GetRevocationStatusRequestRequestTypeDef",
-    "GetRevocationStatusResponseTypeDef",
+    "TimestampTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
     "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    "ListSigningJobsRequestRequestTypeDef",
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutSigningProfileResponseTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
-    "RemoveProfilePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
-    "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
     "S3SourceTypeDef",
-    "SignPayloadRequestRequestTypeDef",
-    "SignPayloadResponseTypeDef",
     "SigningConfigurationOverridesTypeDef",
-    "StartSigningJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AddProfilePermissionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetRevocationStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutSigningProfileResponseTypeDef",
+    "RemoveProfilePermissionResponseTypeDef",
+    "SignPayloadResponseTypeDef",
+    "StartSigningJobResponseTypeDef",
+    "SignPayloadRequestRequestTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
+    "GetRevocationStatusRequestRequestTypeDef",
+    "ListSigningJobsRequestRequestTypeDef",
+    "RevokeSigningProfileRequestRequestTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
     "SourceTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
@@ -119,22 +121,26 @@
 
 class AddProfilePermissionRequestRequestTypeDef(
     _RequiredAddProfilePermissionRequestRequestTypeDef,
     _OptionalAddProfilePermissionRequestRequestTypeDef,
 ):
     pass
 
-AddProfilePermissionResponseTypeDef = TypedDict(
-    "AddProfilePermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
     },
 )
 
@@ -176,48 +182,23 @@
     {
         "bucketName": str,
         "prefix": str,
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
 EncryptionAlgorithmOptionsTypeDef = TypedDict(
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
 
-GetRevocationStatusRequestRequestTypeDef = TypedDict(
-    "GetRevocationStatusRequestRequestTypeDef",
-    {
-        "signatureTimestamp": Union[datetime, str],
-        "platformId": str,
-        "profileVersionArn": str,
-        "jobArn": str,
-        "certificateHashes": Sequence[str],
-    },
-)
-
-GetRevocationStatusResponseTypeDef = TypedDict(
-    "GetRevocationStatusResponseTypeDef",
-    {
-        "revokedEntities": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -302,52 +283,20 @@
         "principal": str,
         "statementId": str,
         "profileVersion": str,
     },
     total=False,
 )
 
-ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListSigningJobsRequestRequestTypeDef = TypedDict(
-    "ListSigningJobsRequestRequestTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "maxResults": int,
-        "nextToken": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-    },
-    total=False,
-)
-
-ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "category": str,
-        "partner": str,
-        "target": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
@@ -356,25 +305,14 @@
         "target": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
-    {
-        "includeCanceled": bool,
-        "platformId": str,
-        "statuses": Sequence[SigningProfileStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningProfilesRequestRequestTypeDef = TypedDict(
     "ListSigningProfilesRequestRequestTypeDef",
     {
         "includeCanceled": bool,
         "maxResults": int,
         "nextToken": str,
         "platformId": str,
@@ -386,70 +324,23 @@
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
-PutSigningProfileResponseTypeDef = TypedDict(
-    "PutSigningProfileResponseTypeDef",
-    {
-        "arn": str,
-        "profileVersion": str,
-        "profileVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
 )
 
-RemoveProfilePermissionResponseTypeDef = TypedDict(
-    "RemoveProfilePermissionResponseTypeDef",
-    {
-        "revisionId": str,
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
 _RequiredRevokeSignatureRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeSignatureRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
@@ -462,24 +353,14 @@
 )
 
 class RevokeSignatureRequestRequestTypeDef(
     _RequiredRevokeSignatureRequestRequestTypeDef, _OptionalRevokeSignatureRequestRequestTypeDef
 ):
     pass
 
-RevokeSigningProfileRequestRequestTypeDef = TypedDict(
-    "RevokeSigningProfileRequestRequestTypeDef",
-    {
-        "profileName": str,
-        "profileVersion": str,
-        "reason": str,
-        "effectiveTime": Union[datetime, str],
-    },
-)
-
 S3SignedObjectTypeDef = TypedDict(
     "S3SignedObjectTypeDef",
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
@@ -490,80 +371,129 @@
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
 )
 
-_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
-    "_RequiredSignPayloadRequestRequestTypeDef",
+SigningConfigurationOverridesTypeDef = TypedDict(
+    "SigningConfigurationOverridesTypeDef",
     {
-        "profileName": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-        "payloadFormat": str,
+        "encryptionAlgorithm": EncryptionAlgorithmType,
+        "hashAlgorithm": HashAlgorithmType,
     },
+    total=False,
 )
-_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
-    "_OptionalSignPayloadRequestRequestTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "profileOwner": str,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
-    total=False,
 )
 
-class SignPayloadRequestRequestTypeDef(
-    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
-):
-    pass
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
+AddProfilePermissionResponseTypeDef = TypedDict(
+    "AddProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
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
+GetRevocationStatusResponseTypeDef = TypedDict(
+    "GetRevocationStatusResponseTypeDef",
+    {
+        "revokedEntities": List[str],
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
+PutSigningProfileResponseTypeDef = TypedDict(
+    "PutSigningProfileResponseTypeDef",
+    {
+        "arn": str,
+        "profileVersion": str,
+        "profileVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveProfilePermissionResponseTypeDef = TypedDict(
+    "RemoveProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 SignPayloadResponseTypeDef = TypedDict(
     "SignPayloadResponseTypeDef",
     {
         "jobId": str,
         "jobOwner": str,
         "metadata": Dict[str, str],
         "signature": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SigningConfigurationOverridesTypeDef = TypedDict(
-    "SigningConfigurationOverridesTypeDef",
-    {
-        "encryptionAlgorithm": EncryptionAlgorithmType,
-        "hashAlgorithm": HashAlgorithmType,
-    },
-    total=False,
-)
-
 StartSigningJobResponseTypeDef = TypedDict(
     "StartSigningJobResponseTypeDef",
     {
         "jobId": str,
         "jobOwner": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
+    "_RequiredSignPayloadRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "profileName": str,
+        "payload": BlobTypeDef,
+        "payloadFormat": str,
     },
 )
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
+    "_OptionalSignPayloadRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "profileOwner": str,
     },
+    total=False,
 )
 
+class SignPayloadRequestRequestTypeDef(
+    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
+):
+    pass
+
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
@@ -584,14 +514,51 @@
     "DestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
     },
     total=False,
 )
 
+GetRevocationStatusRequestRequestTypeDef = TypedDict(
+    "GetRevocationStatusRequestRequestTypeDef",
+    {
+        "signatureTimestamp": TimestampTypeDef,
+        "platformId": str,
+        "profileVersionArn": str,
+        "jobArn": str,
+        "certificateHashes": Sequence[str],
+    },
+)
+
+ListSigningJobsRequestRequestTypeDef = TypedDict(
+    "ListSigningJobsRequestRequestTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "maxResults": int,
+        "nextToken": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
+        "jobInvoker": str,
+    },
+    total=False,
+)
+
+RevokeSigningProfileRequestRequestTypeDef = TypedDict(
+    "RevokeSigningProfileRequestRequestTypeDef",
+    {
+        "profileName": str,
+        "profileVersion": str,
+        "reason": str,
+        "effectiveTime": TimestampTypeDef,
+    },
+)
+
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "signingMaterial": SigningMaterialTypeDef,
@@ -617,18 +584,55 @@
 ListProfilePermissionsResponseTypeDef = TypedDict(
     "ListProfilePermissionsResponseTypeDef",
     {
         "revisionId": str,
         "policySizeBytes": int,
         "permissions": List[PermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": TimestampTypeDef,
+        "signatureExpiresAfter": TimestampTypeDef,
+        "jobInvoker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    {
+        "category": str,
+        "partner": str,
+        "target": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
+    {
+        "includeCanceled": bool,
+        "platformId": str,
+        "statuses": Sequence[SigningProfileStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 SignedObjectTypeDef = TypedDict(
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
     total=False,
 )
@@ -651,15 +655,15 @@
 )
 
 ListSigningProfilesResponseTypeDef = TypedDict(
     "ListSigningProfilesResponseTypeDef",
     {
         "profiles": List[SigningProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningPlatformResponseTypeDef = TypedDict(
     "GetSigningPlatformResponseTypeDef",
     {
         "platformId": str,
@@ -667,15 +671,15 @@
         "partner": str,
         "target": str,
         "category": Literal["AWSIoT"],
         "signingConfiguration": SigningConfigurationTypeDef,
         "signingImageFormat": SigningImageFormatTypeDef,
         "maxSizeInMB": int,
         "revocationSupported": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SigningPlatformTypeDef = TypedDict(
     "SigningPlatformTypeDef",
     {
         "platformId": str,
@@ -752,15 +756,15 @@
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
         "revocationRecord": SigningJobRevocationRecordTypeDef,
         "signedObject": SignedObjectTypeDef,
         "jobOwner": str,
         "jobInvoker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
@@ -773,15 +777,15 @@
         "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
         "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSigningProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPutSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -806,19 +810,19 @@
     pass
 
 ListSigningPlatformsResponseTypeDef = TypedDict(
     "ListSigningPlatformsResponseTypeDef",
     {
         "platforms": List[SigningPlatformTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSigningJobsResponseTypeDef = TypedDict(
     "ListSigningJobsResponseTypeDef",
     {
         "jobs": List[SigningJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/waiter.py` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer/waiter.pyi` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/PKG-INFO` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-signer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore signer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore signer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-signer"></a>
 
 # types-aiobotocore-signer
 
 [![PyPI - types-aiobotocore-signer](https://img.shields.io/pypi/v/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-signer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-signer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-signer?color=blue)](https://pypistats.org/packages/types-aiobotocore-signer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-signer)](https://pepy.tech/project/types-aiobotocore-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.signer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -352,71 +351,73 @@
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_signer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
-    GetRevocationStatusResponseTypeDef,
+    TimestampTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
-    SignPayloadRequestRequestTypeDef,
-    SignPayloadResponseTypeDef,
     SigningConfigurationOverridesTypeDef,
-    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AddProfilePermissionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutSigningProfileResponseTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    SignPayloadResponseTypeDef,
+    StartSigningJobResponseTypeDef,
+    SignPayloadRequestRequestTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    ListSigningJobsRequestRequestTypeDef,
+    RevokeSigningProfileRequestRequestTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
     SourceTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
@@ -425,15 +426,15 @@
     GetSigningProfileResponseTypeDef,
     PutSigningProfileRequestRequestTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
 )
 
 
-def get_structure() -> AddProfilePermissionRequestRequestTypeDef:
+def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-signer-2.5.2/types_aiobotocore_signer.egg-info/SOURCES.txt` & `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


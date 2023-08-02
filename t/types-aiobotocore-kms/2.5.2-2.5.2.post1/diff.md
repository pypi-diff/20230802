# Comparing `tmp/types-aiobotocore-kms-2.5.2.tar.gz` & `tmp/types-aiobotocore-kms-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kms-2.5.2.tar", last modified: Sat Jul  8 01:43:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-kms-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-kms-2.5.2.tar` & `types-aiobotocore-kms-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:52.514412 types-aiobotocore-kms-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-07-08 01:43:52.510412 types-aiobotocore-kms-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:52.514412 types-aiobotocore-kms-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:52.510412 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43136 2023-07-08 01:33:34.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43070 2023-07-08 01:33:34.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-07-08 01:33:34.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-08 01:33:34.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-08 01:33:34.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-08 01:33:34.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40403 2023-07-08 01:33:35.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40344 2023-07-08 01:33:35.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:32.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:52.510412 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-07-08 01:43:52.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:52.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:52.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:52.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:52.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:52.000000 types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42763 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42697 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40489 2023-08-02 14:41:40.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40430 2023-08-02 14:41:40.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kms-2.5.2/LICENSE` & `types-aiobotocore-kms-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2/PKG-INFO` & `types-aiobotocore-kms-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KMS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kms"></a>
 
 # types-aiobotocore-kms
 
 [![PyPI - types-aiobotocore-kms](https://img.shields.io/pypi/v/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kms?color=blue)](https://pypistats.org/packages/types-aiobotocore-kms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kms)](https://pepy.tech/project/types-aiobotocore-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [types-aiobotocore-kms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/).
 
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
@@ -353,129 +352,133 @@
 )
 
 
 def check_value(value: AlgorithmSpecType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kms.type_defs import (
     AliasListEntryTypeDef,
+    BlobTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
-    CancelKeyDeletionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
-    CreateCustomKeyStoreResponseTypeDef,
     GrantConstraintsTypeDef,
-    CreateGrantResponseTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
-    RecipientInfoTypeDef,
-    DecryptResponseTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
-    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
-    EncryptRequestRequestTypeDef,
-    EncryptResponseTypeDef,
-    GenerateDataKeyPairResponseTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
-    GenerateDataKeyResponseTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyWithoutPlaintextResponseTypeDef,
-    GenerateMacRequestRequestTypeDef,
-    GenerateMacResponseTypeDef,
-    GenerateRandomResponseTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
-    GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
-    GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
-    GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
-    GetPublicKeyResponseTypeDef,
-    ImportKeyMaterialRequestRequestTypeDef,
+    GrantConstraintsOutputTypeDef,
+    TimestampTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
-    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
-    ListKeyPoliciesResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
-    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
-    PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
-    ReEncryptRequestRequestTypeDef,
-    ReEncryptResponseTypeDef,
-    ResponseMetadataTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    ScheduleKeyDeletionResponseTypeDef,
-    SignRequestRequestTypeDef,
-    SignResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
+    EncryptRequestRequestTypeDef,
+    GenerateMacRequestRequestTypeDef,
+    ReEncryptRequestRequestTypeDef,
+    RecipientInfoTypeDef,
+    SignRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
-    VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
-    VerifyResponseTypeDef,
+    CancelKeyDeletionResponseTypeDef,
+    CreateCustomKeyStoreResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    DecryptResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptResponseTypeDef,
+    GenerateDataKeyPairResponseTypeDef,
+    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
+    GenerateDataKeyResponseTypeDef,
+    GenerateDataKeyWithoutPlaintextResponseTypeDef,
+    GenerateMacResponseTypeDef,
+    GenerateRandomResponseTypeDef,
+    GetKeyPolicyResponseTypeDef,
+    GetKeyRotationStatusResponseTypeDef,
+    GetParametersForImportResponseTypeDef,
+    GetPublicKeyResponseTypeDef,
     ListAliasesResponseTypeDef,
+    ListKeyPoliciesResponseTypeDef,
+    ReEncryptResponseTypeDef,
+    ScheduleKeyDeletionResponseTypeDef,
+    SignResponseTypeDef,
+    VerifyMacResponseTypeDef,
+    VerifyResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
-    GrantListEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
     ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
+    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListGrantsRequestListGrantsPaginateTypeDef,
+    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    GrantConstraintsUnionTypeDef,
+    GrantListEntryTypeDef,
+    ImportKeyMaterialRequestRequestTypeDef,
+    ListKeysResponseTypeDef,
+    MultiRegionConfigurationTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
-    ListKeysResponseTypeDef,
-    MultiRegionConfigurationTypeDef,
-    ListGrantsResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
+    ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
 
 
-def get_structure() -> AliasListEntryTypeDef:
+def get_value() -> AliasListEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kms-2.5.2/README.md` & `types-aiobotocore-kms-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kms"></a>
 
 # types-aiobotocore-kms
 
 [![PyPI - types-aiobotocore-kms](https://img.shields.io/pypi/v/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kms?color=blue)](https://pypistats.org/packages/types-aiobotocore-kms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kms)](https://pepy.tech/project/types-aiobotocore-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [types-aiobotocore-kms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/).
 
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
@@ -320,129 +320,133 @@
 )
 
 
 def check_value(value: AlgorithmSpecType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kms.type_defs import (
     AliasListEntryTypeDef,
+    BlobTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
-    CancelKeyDeletionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
-    CreateCustomKeyStoreResponseTypeDef,
     GrantConstraintsTypeDef,
-    CreateGrantResponseTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
-    RecipientInfoTypeDef,
-    DecryptResponseTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
-    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
-    EncryptRequestRequestTypeDef,
-    EncryptResponseTypeDef,
-    GenerateDataKeyPairResponseTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
-    GenerateDataKeyResponseTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyWithoutPlaintextResponseTypeDef,
-    GenerateMacRequestRequestTypeDef,
-    GenerateMacResponseTypeDef,
-    GenerateRandomResponseTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
-    GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
-    GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
-    GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
-    GetPublicKeyResponseTypeDef,
-    ImportKeyMaterialRequestRequestTypeDef,
+    GrantConstraintsOutputTypeDef,
+    TimestampTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
-    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
-    ListKeyPoliciesResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
-    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
-    PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
-    ReEncryptRequestRequestTypeDef,
-    ReEncryptResponseTypeDef,
-    ResponseMetadataTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    ScheduleKeyDeletionResponseTypeDef,
-    SignRequestRequestTypeDef,
-    SignResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
+    EncryptRequestRequestTypeDef,
+    GenerateMacRequestRequestTypeDef,
+    ReEncryptRequestRequestTypeDef,
+    RecipientInfoTypeDef,
+    SignRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
-    VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
-    VerifyResponseTypeDef,
+    CancelKeyDeletionResponseTypeDef,
+    CreateCustomKeyStoreResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    DecryptResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptResponseTypeDef,
+    GenerateDataKeyPairResponseTypeDef,
+    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
+    GenerateDataKeyResponseTypeDef,
+    GenerateDataKeyWithoutPlaintextResponseTypeDef,
+    GenerateMacResponseTypeDef,
+    GenerateRandomResponseTypeDef,
+    GetKeyPolicyResponseTypeDef,
+    GetKeyRotationStatusResponseTypeDef,
+    GetParametersForImportResponseTypeDef,
+    GetPublicKeyResponseTypeDef,
     ListAliasesResponseTypeDef,
+    ListKeyPoliciesResponseTypeDef,
+    ReEncryptResponseTypeDef,
+    ScheduleKeyDeletionResponseTypeDef,
+    SignResponseTypeDef,
+    VerifyMacResponseTypeDef,
+    VerifyResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
-    GrantListEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
     ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
+    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListGrantsRequestListGrantsPaginateTypeDef,
+    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    GrantConstraintsUnionTypeDef,
+    GrantListEntryTypeDef,
+    ImportKeyMaterialRequestRequestTypeDef,
+    ListKeysResponseTypeDef,
+    MultiRegionConfigurationTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
-    ListKeysResponseTypeDef,
-    MultiRegionConfigurationTypeDef,
-    ListGrantsResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
+    ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
 
 
-def get_structure() -> AliasListEntryTypeDef:
+def get_value() -> AliasListEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kms-2.5.2/setup.py` & `types-aiobotocore-kms-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kms",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KMS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore kms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore kms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/__init__.py` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/__init__.pyi` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/__main__.py` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KMS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.KMS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/client.py` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 
     session = get_session()
     async with session.create_client("kms") as client:
         client: KMSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AlgorithmSpecType,
     CustomerMasterKeySpecType,
     CustomKeyStoreTypeType,
     DataKeyPairSpecType,
@@ -46,14 +44,15 @@
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     CreateKeyResponseTypeDef,
     DecryptResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     DescribeKeyResponseTypeDef,
@@ -65,26 +64,27 @@
     GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacResponseTypeDef,
     GenerateRandomResponseTypeDef,
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
-    GrantConstraintsTypeDef,
+    GrantConstraintsUnionTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
     ReplicateKeyResponseTypeDef,
     ScheduleKeyDeletionResponseTypeDef,
     SignResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VerifyMacResponseTypeDef,
     VerifyResponseTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -240,15 +240,15 @@
     async def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
-        Constraints: GrantConstraintsTypeDef = ...,
+        Constraints: GrantConstraintsUnionTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
         Name: str = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
@@ -278,15 +278,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_key)
         """
 
     async def decrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         Recipient: RecipientInfoTypeDef = ...
     ) -> DecryptResponseTypeDef:
         """
@@ -398,15 +398,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#enable_key_rotation)
         """
 
     async def encrypt(
         self,
         *,
         KeyId: str,
-        Plaintext: Union[str, bytes, IO[Any], StreamingBody],
+        Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
@@ -477,15 +477,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_without_plaintext)
         """
 
     async def generate_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         GrantTokens: Sequence[str] = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
         HMAC KMS key and a MAC algorithm that the key supports.
@@ -565,17 +565,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_public_key)
         """
 
     async def import_key_material(
         self,
         *,
         KeyId: str,
-        ImportToken: Union[str, bytes, IO[Any], StreamingBody],
-        EncryptedKeyMaterial: Union[str, bytes, IO[Any], StreamingBody],
-        ValidTo: Union[datetime, str] = ...,
+        ImportToken: BlobTypeDef,
+        EncryptedKeyMaterial: BlobTypeDef,
+        ValidTo: TimestampTypeDef = ...,
         ExpirationModel: ExpirationModelTypeType = ...
     ) -> Dict[str, Any]:
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
@@ -662,15 +662,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#put_key_policy)
         """
 
     async def re_encrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         GrantTokens: Sequence[str] = ...
@@ -727,15 +727,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#schedule_key_deletion)
         """
 
     async def sign(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
         for a message or message digest by using the private key in an asymmetric
@@ -819,34 +819,34 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_primary_region)
         """
 
     async def verify(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
-        Signature: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
+        Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify)
         """
 
     async def verify_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        Mac: Union[str, bytes, IO[Any], StreamingBody],
+        Mac: BlobTypeDef,
         GrantTokens: Sequence[str] = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/client.pyi` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 
     session = get_session()
     async with session.create_client("kms") as client:
         client: KMSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AlgorithmSpecType,
     CustomerMasterKeySpecType,
     CustomKeyStoreTypeType,
     DataKeyPairSpecType,
@@ -46,14 +44,15 @@
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     CreateKeyResponseTypeDef,
     DecryptResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     DescribeKeyResponseTypeDef,
@@ -65,26 +64,27 @@
     GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacResponseTypeDef,
     GenerateRandomResponseTypeDef,
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
-    GrantConstraintsTypeDef,
+    GrantConstraintsUnionTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
     ReplicateKeyResponseTypeDef,
     ScheduleKeyDeletionResponseTypeDef,
     SignResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VerifyMacResponseTypeDef,
     VerifyResponseTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -229,15 +229,15 @@
     async def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
-        Constraints: GrantConstraintsTypeDef = ...,
+        Constraints: GrantConstraintsUnionTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
         Name: str = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
@@ -265,15 +265,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_key)
         """
     async def decrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         Recipient: RecipientInfoTypeDef = ...
     ) -> DecryptResponseTypeDef:
         """
@@ -374,15 +374,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#enable_key_rotation)
         """
     async def encrypt(
         self,
         *,
         KeyId: str,
-        Plaintext: Union[str, bytes, IO[Any], StreamingBody],
+        Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
@@ -448,15 +448,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_without_plaintext)
         """
     async def generate_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         GrantTokens: Sequence[str] = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
         HMAC KMS key and a MAC algorithm that the key supports.
@@ -529,17 +529,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_public_key)
         """
     async def import_key_material(
         self,
         *,
         KeyId: str,
-        ImportToken: Union[str, bytes, IO[Any], StreamingBody],
-        EncryptedKeyMaterial: Union[str, bytes, IO[Any], StreamingBody],
-        ValidTo: Union[datetime, str] = ...,
+        ImportToken: BlobTypeDef,
+        EncryptedKeyMaterial: BlobTypeDef,
+        ValidTo: TimestampTypeDef = ...,
         ExpirationModel: ExpirationModelTypeType = ...
     ) -> Dict[str, Any]:
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
@@ -618,15 +618,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#put_key_policy)
         """
     async def re_encrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         GrantTokens: Sequence[str] = ...
@@ -678,15 +678,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#schedule_key_deletion)
         """
     async def sign(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
         for a message or message digest by using the private key in an asymmetric
@@ -763,33 +763,33 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_primary_region)
         """
     async def verify(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
-        Signature: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
+        Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify)
         """
     async def verify_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        Mac: Union[str, bytes, IO[Any], StreamingBody],
+        Mac: BlobTypeDef,
         GrantTokens: Sequence[str] = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/literals.py` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/literals.pyi` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/paginator.py` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,30 +75,30 @@
     """
 
     def paginate(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#describecustomkeystorespaginator)
         """
 
 
 class ListAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listaliasespaginator)
         """
 
 
@@ -110,73 +110,73 @@
 
     def paginate(
         self,
         *,
         KeyId: str,
         GrantId: str = ...,
         GranteePrincipal: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listgrantspaginator)
         """
 
 
 class ListKeyPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeypoliciespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeyPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeypoliciespaginator)
         """
 
 
 class ListKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeyspaginator)
         """
 
 
 class ListResourceTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listresourcetagspaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listresourcetagspaginator)
         """
 
 
 class ListRetirableGrantsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listretirablegrantspaginator)
     """
 
     def paginate(
-        self, *, RetiringPrincipal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RetiringPrincipal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listretirablegrantspaginator)
         """
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/paginator.pyi` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,29 +72,29 @@
     """
 
     def paginate(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#describecustomkeystorespaginator)
         """
 
 class ListAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listaliasespaginator)
         """
 
 class ListGrantsPaginator(AioPaginator):
@@ -105,69 +105,69 @@
 
     def paginate(
         self,
         *,
         KeyId: str,
         GrantId: str = ...,
         GranteePrincipal: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listgrantspaginator)
         """
 
 class ListKeyPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeypoliciespaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeyPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeypoliciespaginator)
         """
 
 class ListKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listkeyspaginator)
         """
 
 class ListResourceTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listresourcetagspaginator)
     """
 
     def paginate(
-        self, *, KeyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listresourcetagspaginator)
         """
 
 class ListRetirableGrantsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listretirablegrantspaginator)
     """
 
     def paginate(
-        self, *, RetiringPrincipal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RetiringPrincipal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGrantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/paginators/#listretirablegrantspaginator)
         """
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/type_defs.py` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kms.type_defs import AliasListEntryTypeDef
 
-    data: AliasListEntryTypeDef = {...}
+    data: AliasListEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -46,114 +46,117 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasListEntryTypeDef",
+    "BlobTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
-    "CancelKeyDeletionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
-    "CreateCustomKeyStoreResponseTypeDef",
     "GrantConstraintsTypeDef",
-    "CreateGrantResponseTypeDef",
     "TagTypeDef",
     "XksProxyConfigurationTypeTypeDef",
-    "RecipientInfoTypeDef",
-    "DecryptResponseTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCustomKeyStoreRequestRequestTypeDef",
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DisableKeyRequestRequestTypeDef",
     "DisableKeyRotationRequestRequestTypeDef",
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableKeyRequestRequestTypeDef",
     "EnableKeyRotationRequestRequestTypeDef",
-    "EncryptRequestRequestTypeDef",
-    "EncryptResponseTypeDef",
-    "GenerateDataKeyPairResponseTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    "GenerateDataKeyResponseTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
-    "GenerateMacRequestRequestTypeDef",
-    "GenerateMacResponseTypeDef",
-    "GenerateRandomResponseTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
-    "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
-    "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
-    "GetParametersForImportResponseTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
-    "GetPublicKeyResponseTypeDef",
-    "ImportKeyMaterialRequestRequestTypeDef",
+    "GrantConstraintsOutputTypeDef",
+    "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListGrantsRequestRequestTypeDef",
-    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
-    "ListKeyPoliciesResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
-    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
-    "PaginatorConfigTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
-    "ReEncryptRequestRequestTypeDef",
-    "ReEncryptResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
-    "ScheduleKeyDeletionResponseTypeDef",
-    "SignRequestRequestTypeDef",
-    "SignResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
+    "EncryptRequestRequestTypeDef",
+    "GenerateMacRequestRequestTypeDef",
+    "ReEncryptRequestRequestTypeDef",
+    "RecipientInfoTypeDef",
+    "SignRequestRequestTypeDef",
     "VerifyMacRequestRequestTypeDef",
-    "VerifyMacResponseTypeDef",
     "VerifyRequestRequestTypeDef",
-    "VerifyResponseTypeDef",
+    "CancelKeyDeletionResponseTypeDef",
+    "CreateCustomKeyStoreResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "DecryptResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EncryptResponseTypeDef",
+    "GenerateDataKeyPairResponseTypeDef",
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    "GenerateDataKeyResponseTypeDef",
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    "GenerateMacResponseTypeDef",
+    "GenerateRandomResponseTypeDef",
+    "GetKeyPolicyResponseTypeDef",
+    "GetKeyRotationStatusResponseTypeDef",
+    "GetParametersForImportResponseTypeDef",
+    "GetPublicKeyResponseTypeDef",
     "ListAliasesResponseTypeDef",
+    "ListKeyPoliciesResponseTypeDef",
+    "ReEncryptResponseTypeDef",
+    "ScheduleKeyDeletionResponseTypeDef",
+    "SignResponseTypeDef",
+    "VerifyMacResponseTypeDef",
+    "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "GrantListEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListGrantsRequestListGrantsPaginateTypeDef",
+    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    "GrantConstraintsUnionTypeDef",
+    "GrantListEntryTypeDef",
+    "ImportKeyMaterialRequestRequestTypeDef",
+    "ListKeysResponseTypeDef",
+    "MultiRegionConfigurationTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
-    "ListKeysResponseTypeDef",
-    "MultiRegionConfigurationTypeDef",
-    "ListGrantsResponseTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
+    "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
 
 AliasListEntryTypeDef = TypedDict(
@@ -164,26 +167,30 @@
         "TargetKeyId": str,
         "CreationDate": datetime,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelKeyDeletionRequestRequestTypeDef = TypedDict(
     "CancelKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-CancelKeyDeletionResponseTypeDef = TypedDict(
-    "CancelKeyDeletionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
@@ -202,40 +209,23 @@
     "XksProxyAuthenticationCredentialTypeTypeDef",
     {
         "AccessKeyId": str,
         "RawSecretAccessKey": str,
     },
 )
 
-CreateCustomKeyStoreResponseTypeDef = TypedDict(
-    "CreateCustomKeyStoreResponseTypeDef",
-    {
-        "CustomKeyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrantConstraintsTypeDef = TypedDict(
     "GrantConstraintsTypeDef",
     {
         "EncryptionContextSubset": Mapping[str, str],
         "EncryptionContextEquals": Mapping[str, str],
     },
     total=False,
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantToken": str,
-        "GrantId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "TagKey": str,
         "TagValue": str,
     },
 )
@@ -248,34 +238,14 @@
         "UriEndpoint": str,
         "UriPath": str,
         "VpcEndpointServiceName": str,
     },
     total=False,
 )
 
-RecipientInfoTypeDef = TypedDict(
-    "RecipientInfoTypeDef",
-    {
-        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
-        "AttestationDocument": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-DecryptResponseTypeDef = TypedDict(
-    "DecryptResponseTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": bytes,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -289,20 +259,20 @@
 DeleteImportedKeyMaterialRequestRequestTypeDef = TypedDict(
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CustomKeyStoreId": str,
-        "CustomKeyStoreName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCustomKeyStoresRequestRequestTypeDef = TypedDict(
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     {
@@ -324,21 +294,19 @@
     "_OptionalDescribeKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeKeyRequestRequestTypeDef(
     _RequiredDescribeKeyRequestRequestTypeDef, _OptionalDescribeKeyRequestRequestTypeDef
 ):
     pass
 
-
 DisableKeyRequestRequestTypeDef = TypedDict(
     "DisableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -352,82 +320,28 @@
 DisconnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableKeyRequestRequestTypeDef = TypedDict(
     "EnableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
 EnableKeyRotationRequestRequestTypeDef = TypedDict(
     "EnableKeyRotationRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-_RequiredEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredEncryptRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalEncryptRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-    },
-    total=False,
-)
-
-
-class EncryptRequestRequestTypeDef(
-    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
-):
-    pass
-
-
-EncryptResponseTypeDef = TypedDict(
-    "EncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyPairResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PrivateKeyPlaintext": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -436,44 +350,20 @@
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-
-GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyResponseTypeDef = TypedDict(
-    "GenerateDataKeyResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "Plaintext": bytes,
-        "KeyId": str,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
@@ -483,183 +373,73 @@
         "KeySpec": DataKeySpecType,
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-
-GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateMacRequestRequestTypeDef",
-    {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "KeyId": str,
-        "MacAlgorithm": MacAlgorithmSpecType,
-    },
-)
-_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateMacRequestRequestTypeDef",
-    {
-        "GrantTokens": Sequence[str],
-    },
-    total=False,
-)
-
-
-class GenerateMacRequestRequestTypeDef(
-    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
-):
-    pass
-
-
-GenerateMacResponseTypeDef = TypedDict(
-    "GenerateMacResponseTypeDef",
-    {
-        "Mac": bytes,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateRandomResponseTypeDef = TypedDict(
-    "GenerateRandomResponseTypeDef",
-    {
-        "Plaintext": bytes,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKeyPolicyRequestRequestTypeDef = TypedDict(
     "GetKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
     },
 )
 
-GetKeyPolicyResponseTypeDef = TypedDict(
-    "GetKeyPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKeyRotationStatusRequestRequestTypeDef = TypedDict(
     "GetKeyRotationStatusRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-GetKeyRotationStatusResponseTypeDef = TypedDict(
-    "GetKeyRotationStatusResponseTypeDef",
-    {
-        "KeyRotationEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParametersForImportRequestRequestTypeDef = TypedDict(
     "GetParametersForImportRequestRequestTypeDef",
     {
         "KeyId": str,
         "WrappingAlgorithm": AlgorithmSpecType,
         "WrappingKeySpec": WrappingKeySpecType,
     },
 )
 
-GetParametersForImportResponseTypeDef = TypedDict(
-    "GetParametersForImportResponseTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": bytes,
-        "PublicKey": bytes,
-        "ParametersValidTo": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGetPublicKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalGetPublicKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
-
-GetPublicKeyResponseTypeDef = TypedDict(
-    "GetPublicKeyResponseTypeDef",
+GrantConstraintsOutputTypeDef = TypedDict(
+    "GrantConstraintsOutputTypeDef",
     {
-        "KeyId": str,
-        "PublicKey": bytes,
-        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
-        "KeySpec": KeySpecType,
-        "KeyUsage": KeyUsageTypeType,
-        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
-        "SigningAlgorithms": List[SigningAlgorithmSpecType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_RequiredImportKeyMaterialRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": Union[str, bytes, IO[Any], StreamingBody],
-        "EncryptedKeyMaterial": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_OptionalImportKeyMaterialRequestRequestTypeDef",
-    {
-        "ValidTo": Union[datetime, str],
-        "ExpirationModel": ExpirationModelTypeType,
+        "EncryptionContextSubset": Dict[str, str],
+        "EncryptionContextEquals": Dict[str, str],
     },
     total=False,
 )
 
-
-class ImportKeyMaterialRequestRequestTypeDef(
-    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -669,57 +449,24 @@
     "XksKeyConfigurationTypeTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "KeyId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAliasesRequestRequestTypeDef = TypedDict(
     "ListAliasesRequestRequestTypeDef",
     {
         "KeyId": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "GrantId": str,
-        "GranteePrincipal": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGrantsRequestListGrantsPaginateTypeDef(
-    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
-    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListGrantsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListGrantsRequestRequestTypeDef = TypedDict(
@@ -729,43 +476,19 @@
         "Marker": str,
         "GrantId": str,
         "GranteePrincipal": str,
     },
     total=False,
 )
 
-
 class ListGrantsRequestRequestTypeDef(
     _RequiredListGrantsRequestRequestTypeDef, _OptionalListGrantsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
-    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListKeyPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListKeyPoliciesRequestRequestTypeDef = TypedDict(
@@ -773,70 +496,28 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListKeyPoliciesRequestRequestTypeDef(
     _RequiredListKeyPoliciesRequestRequestTypeDef, _OptionalListKeyPoliciesRequestRequestTypeDef
 ):
     pass
 
-
-ListKeyPoliciesResponseTypeDef = TypedDict(
-    "ListKeyPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
-    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
-    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceTagsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListResourceTagsRequestRequestTypeDef = TypedDict(
@@ -844,43 +525,19 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListResourceTagsRequestRequestTypeDef(
     _RequiredListResourceTagsRequestRequestTypeDef, _OptionalListResourceTagsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "RetiringPrincipal": str,
-    },
-)
-_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
-    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRetirableGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
 _OptionalListRetirableGrantsRequestRequestTypeDef = TypedDict(
@@ -888,41 +545,29 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListRetirableGrantsRequestRequestTypeDef(
     _RequiredListRetirableGrantsRequestRequestTypeDef,
     _OptionalListRetirableGrantsRequestRequestTypeDef,
 ):
     pass
 
-
 MultiRegionKeyTypeDef = TypedDict(
     "MultiRegionKeyTypeDef",
     {
         "Arn": str,
         "Region": str,
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
 _RequiredPutKeyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -931,264 +576,460 @@
     "_OptionalPutKeyPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
-
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
+RetireGrantRequestRequestTypeDef = TypedDict(
+    "RetireGrantRequestRequestTypeDef",
+    {
+        "GrantToken": str,
+        "KeyId": str,
+        "GrantId": str,
+    },
+    total=False,
+)
 
-_RequiredReEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredReEncryptRequestRequestTypeDef",
+RevokeGrantRequestRequestTypeDef = TypedDict(
+    "RevokeGrantRequestRequestTypeDef",
     {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "DestinationKeyId": str,
+        "KeyId": str,
+        "GrantId": str,
     },
 )
-_OptionalReEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalReEncryptRequestRequestTypeDef",
+
+_RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
+    "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
-        "SourceEncryptionContext": Mapping[str, str],
-        "SourceKeyId": str,
-        "DestinationEncryptionContext": Mapping[str, str],
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "GrantTokens": Sequence[str],
+        "KeyId": str,
+    },
+)
+_OptionalScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
+    "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
+    {
+        "PendingWindowInDays": int,
     },
     total=False,
 )
 
-
-class ReEncryptRequestRequestTypeDef(
-    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
+class ScheduleKeyDeletionRequestRequestTypeDef(
+    _RequiredScheduleKeyDeletionRequestRequestTypeDef,
+    _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
-
-ReEncryptResponseTypeDef = TypedDict(
-    "ReEncryptResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "CiphertextBlob": bytes,
-        "SourceKeyId": str,
         "KeyId": str,
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagKeys": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UpdateAliasRequestRequestTypeDef = TypedDict(
+    "UpdateAliasRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AliasName": str,
+        "TargetKeyId": str,
     },
 )
 
-RetireGrantRequestRequestTypeDef = TypedDict(
-    "RetireGrantRequestRequestTypeDef",
+UpdateKeyDescriptionRequestRequestTypeDef = TypedDict(
+    "UpdateKeyDescriptionRequestRequestTypeDef",
     {
-        "GrantToken": str,
         "KeyId": str,
-        "GrantId": str,
+        "Description": str,
     },
-    total=False,
 )
 
-RevokeGrantRequestRequestTypeDef = TypedDict(
-    "RevokeGrantRequestRequestTypeDef",
+UpdatePrimaryRegionRequestRequestTypeDef = TypedDict(
+    "UpdatePrimaryRegionRequestRequestTypeDef",
     {
         "KeyId": str,
-        "GrantId": str,
+        "PrimaryRegion": str,
     },
 )
 
-_RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
-    "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
+_RequiredEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredEncryptRequestRequestTypeDef",
     {
         "KeyId": str,
+        "Plaintext": BlobTypeDef,
     },
 )
-_OptionalScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
-    "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
+_OptionalEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalEncryptRequestRequestTypeDef",
     {
-        "PendingWindowInDays": int,
+        "EncryptionContext": Mapping[str, str],
+        "GrantTokens": Sequence[str],
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
     },
     total=False,
 )
 
+class EncryptRequestRequestTypeDef(
+    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
+):
+    pass
 
-class ScheduleKeyDeletionRequestRequestTypeDef(
-    _RequiredScheduleKeyDeletionRequestRequestTypeDef,
-    _OptionalScheduleKeyDeletionRequestRequestTypeDef,
+_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateMacRequestRequestTypeDef",
+    {
+        "Message": BlobTypeDef,
+        "KeyId": str,
+        "MacAlgorithm": MacAlgorithmSpecType,
+    },
+)
+_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateMacRequestRequestTypeDef",
+    {
+        "GrantTokens": Sequence[str],
+    },
+    total=False,
+)
+
+class GenerateMacRequestRequestTypeDef(
+    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
     pass
 
+_RequiredReEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredReEncryptRequestRequestTypeDef",
+    {
+        "CiphertextBlob": BlobTypeDef,
+        "DestinationKeyId": str,
+    },
+)
+_OptionalReEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalReEncryptRequestRequestTypeDef",
+    {
+        "SourceEncryptionContext": Mapping[str, str],
+        "SourceKeyId": str,
+        "DestinationEncryptionContext": Mapping[str, str],
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "GrantTokens": Sequence[str],
+    },
+    total=False,
+)
+
+class ReEncryptRequestRequestTypeDef(
+    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
+):
+    pass
 
-ScheduleKeyDeletionResponseTypeDef = TypedDict(
-    "ScheduleKeyDeletionResponseTypeDef",
+RecipientInfoTypeDef = TypedDict(
+    "RecipientInfoTypeDef",
     {
-        "KeyId": str,
-        "DeletionDate": datetime,
-        "KeyState": KeyStateType,
-        "PendingWindowInDays": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
+        "AttestationDocument": BlobTypeDef,
     },
+    total=False,
 )
 
 _RequiredSignRequestRequestTypeDef = TypedDict(
     "_RequiredSignRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmSpecType,
     },
 )
 _OptionalSignRequestRequestTypeDef = TypedDict(
     "_OptionalSignRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
     pass
 
+_RequiredVerifyMacRequestRequestTypeDef = TypedDict(
+    "_RequiredVerifyMacRequestRequestTypeDef",
+    {
+        "Message": BlobTypeDef,
+        "KeyId": str,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "Mac": BlobTypeDef,
+    },
+)
+_OptionalVerifyMacRequestRequestTypeDef = TypedDict(
+    "_OptionalVerifyMacRequestRequestTypeDef",
+    {
+        "GrantTokens": Sequence[str],
+    },
+    total=False,
+)
+
+class VerifyMacRequestRequestTypeDef(
+    _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
+):
+    pass
 
-SignResponseTypeDef = TypedDict(
-    "SignResponseTypeDef",
+_RequiredVerifyRequestRequestTypeDef = TypedDict(
+    "_RequiredVerifyRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Signature": bytes,
+        "Message": BlobTypeDef,
+        "Signature": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalVerifyRequestRequestTypeDef = TypedDict(
+    "_OptionalVerifyRequestRequestTypeDef",
+    {
+        "MessageType": MessageTypeType,
+        "GrantTokens": Sequence[str],
+    },
+    total=False,
+)
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+class VerifyRequestRequestTypeDef(
+    _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
+):
+    pass
+
+CancelKeyDeletionResponseTypeDef = TypedDict(
+    "CancelKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
-        "TagKeys": Sequence[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAliasRequestRequestTypeDef = TypedDict(
-    "UpdateAliasRequestRequestTypeDef",
+CreateCustomKeyStoreResponseTypeDef = TypedDict(
+    "CreateCustomKeyStoreResponseTypeDef",
     {
-        "AliasName": str,
-        "TargetKeyId": str,
+        "CustomKeyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateKeyDescriptionRequestRequestTypeDef = TypedDict(
-    "UpdateKeyDescriptionRequestRequestTypeDef",
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
     {
-        "KeyId": str,
-        "Description": str,
+        "GrantToken": str,
+        "GrantId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePrimaryRegionRequestRequestTypeDef = TypedDict(
-    "UpdatePrimaryRegionRequestRequestTypeDef",
+DecryptResponseTypeDef = TypedDict(
+    "DecryptResponseTypeDef",
     {
         "KeyId": str,
-        "PrimaryRegion": str,
+        "Plaintext": bytes,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredVerifyMacRequestRequestTypeDef = TypedDict(
-    "_RequiredVerifyMacRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "KeyId": str,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "Mac": Union[str, bytes, IO[Any], StreamingBody],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalVerifyMacRequestRequestTypeDef = TypedDict(
-    "_OptionalVerifyMacRequestRequestTypeDef",
+
+EncryptResponseTypeDef = TypedDict(
+    "EncryptResponseTypeDef",
     {
-        "GrantTokens": Sequence[str],
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GenerateDataKeyPairResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PrivateKeyPlaintext": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class VerifyMacRequestRequestTypeDef(
-    _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
-):
-    pass
+GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GenerateDataKeyResponseTypeDef = TypedDict(
+    "GenerateDataKeyResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "Plaintext": bytes,
+        "KeyId": str,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VerifyMacResponseTypeDef = TypedDict(
-    "VerifyMacResponseTypeDef",
+GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
     {
+        "CiphertextBlob": bytes,
         "KeyId": str,
-        "MacValid": bool,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredVerifyRequestRequestTypeDef = TypedDict(
-    "_RequiredVerifyRequestRequestTypeDef",
+GenerateMacResponseTypeDef = TypedDict(
+    "GenerateMacResponseTypeDef",
     {
+        "Mac": bytes,
+        "MacAlgorithm": MacAlgorithmSpecType,
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "Signature": Union[str, bytes, IO[Any], StreamingBody],
-        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalVerifyRequestRequestTypeDef = TypedDict(
-    "_OptionalVerifyRequestRequestTypeDef",
+
+GenerateRandomResponseTypeDef = TypedDict(
+    "GenerateRandomResponseTypeDef",
     {
-        "MessageType": MessageTypeType,
-        "GrantTokens": Sequence[str],
+        "Plaintext": bytes,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetKeyPolicyResponseTypeDef = TypedDict(
+    "GetKeyPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class VerifyRequestRequestTypeDef(
-    _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
-):
-    pass
+GetKeyRotationStatusResponseTypeDef = TypedDict(
+    "GetKeyRotationStatusResponseTypeDef",
+    {
+        "KeyRotationEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetParametersForImportResponseTypeDef = TypedDict(
+    "GetParametersForImportResponseTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": bytes,
+        "PublicKey": bytes,
+        "ParametersValidTo": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VerifyResponseTypeDef = TypedDict(
-    "VerifyResponseTypeDef",
+GetPublicKeyResponseTypeDef = TypedDict(
+    "GetPublicKeyResponseTypeDef",
     {
         "KeyId": str,
-        "SignatureValid": bool,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PublicKey": bytes,
+        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
+        "KeySpec": KeySpecType,
+        "KeyUsage": KeyUsageTypeType,
+        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
+        "SigningAlgorithms": List[SigningAlgorithmSpecType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "Aliases": List[AliasListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListKeyPoliciesResponseTypeDef = TypedDict(
+    "ListKeyPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReEncryptResponseTypeDef = TypedDict(
+    "ReEncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "SourceKeyId": str,
+        "KeyId": str,
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduleKeyDeletionResponseTypeDef = TypedDict(
+    "ScheduleKeyDeletionResponseTypeDef",
+    {
+        "KeyId": str,
+        "DeletionDate": datetime,
+        "KeyState": KeyStateType,
+        "PendingWindowInDays": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignResponseTypeDef = TypedDict(
+    "SignResponseTypeDef",
+    {
+        "KeyId": str,
+        "Signature": bytes,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyMacResponseTypeDef = TypedDict(
+    "VerifyMacResponseTypeDef",
+    {
+        "KeyId": str,
+        "MacValid": bool,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyResponseTypeDef = TypedDict(
+    "VerifyResponseTypeDef",
+    {
+        "KeyId": str,
+        "SignatureValid": bool,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreName": str,
@@ -1206,22 +1047,20 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
-
 class CreateCustomKeyStoreRequestRequestTypeDef(
     _RequiredCreateCustomKeyStoreRequestRequestTypeDef,
     _OptionalCreateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 _OptionalUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
@@ -1235,22 +1074,20 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
-
 class UpdateCustomKeyStoreRequestRequestTypeDef(
     _RequiredUpdateCustomKeyStoreRequestRequestTypeDef,
     _OptionalUpdateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateGrantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GranteePrincipal": str,
         "Operations": Sequence[GrantOperationType],
     },
@@ -1262,37 +1099,19 @@
         "Constraints": GrantConstraintsTypeDef,
         "GrantTokens": Sequence[str],
         "Name": str,
     },
     total=False,
 )
 
-
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
-
-GrantListEntryTypeDef = TypedDict(
-    "GrantListEntryTypeDef",
-    {
-        "KeyId": str,
-        "GrantId": str,
-        "Name": str,
-        "CreationDate": datetime,
-        "GranteePrincipal": str,
-        "RetiringPrincipal": str,
-        "IssuingAccount": str,
-        "Operations": List[GrantOperationType],
-        "Constraints": GrantConstraintsTypeDef,
-    },
-    total=False,
-)
-
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
@@ -1309,15 +1128,15 @@
 
 ListResourceTagsResponseTypeDef = TypedDict(
     "ListResourceTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredReplicateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateKeyRequestRequestTypeDef",
     {
         "KeyId": str,
@@ -1331,21 +1150,19 @@
         "BypassPolicyLockoutSafetyCheck": bool,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ReplicateKeyRequestRequestTypeDef(
     _RequiredReplicateKeyRequestRequestTypeDef, _OptionalReplicateKeyRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1362,39 +1179,205 @@
         "CreationDate": datetime,
         "CustomKeyStoreType": CustomKeyStoreTypeType,
         "XksProxyConfiguration": XksProxyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "CustomKeyStoreName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "KeyId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "GrantId": str,
+        "GranteePrincipal": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGrantsRequestListGrantsPaginateTypeDef(
+    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
+    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
+):
+    pass
+
+_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
+    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+):
+    pass
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
+    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "RetiringPrincipal": str,
+    },
+)
+_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
+    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+):
+    pass
+
+GrantConstraintsUnionTypeDef = Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef]
+GrantListEntryTypeDef = TypedDict(
+    "GrantListEntryTypeDef",
+    {
+        "KeyId": str,
+        "GrantId": str,
+        "Name": str,
+        "CreationDate": datetime,
+        "GranteePrincipal": str,
+        "RetiringPrincipal": str,
+        "IssuingAccount": str,
+        "Operations": List[GrantOperationType],
+        "Constraints": GrantConstraintsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_RequiredImportKeyMaterialRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": BlobTypeDef,
+        "EncryptedKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_OptionalImportKeyMaterialRequestRequestTypeDef",
+    {
+        "ValidTo": TimestampTypeDef,
+        "ExpirationModel": ExpirationModelTypeType,
+    },
+    total=False,
+)
+
+class ImportKeyMaterialRequestRequestTypeDef(
+    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
+):
+    pass
+
+ListKeysResponseTypeDef = TypedDict(
+    "ListKeysResponseTypeDef",
+    {
+        "Keys": List[KeyListEntryTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MultiRegionConfigurationTypeDef = TypedDict(
+    "MultiRegionConfigurationTypeDef",
+    {
+        "MultiRegionKeyType": MultiRegionKeyTypeType,
+        "PrimaryKey": MultiRegionKeyTypeDef,
+        "ReplicaKeys": List[MultiRegionKeyTypeDef],
+    },
+    total=False,
+)
+
 _RequiredDecryptRequestRequestTypeDef = TypedDict(
     "_RequiredDecryptRequestRequestTypeDef",
     {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "CiphertextBlob": BlobTypeDef,
     },
 )
 _OptionalDecryptRequestRequestTypeDef = TypedDict(
     "_OptionalDecryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -1404,22 +1387,20 @@
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
@@ -1430,68 +1411,46 @@
         "KeySpec": DataKeySpecType,
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
     pass
 
-
 GenerateRandomRequestRequestTypeDef = TypedDict(
     "GenerateRandomRequestRequestTypeDef",
     {
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-ListKeysResponseTypeDef = TypedDict(
-    "ListKeysResponseTypeDef",
+DescribeCustomKeyStoresResponseTypeDef = TypedDict(
+    "DescribeCustomKeyStoresResponseTypeDef",
     {
-        "Keys": List[KeyListEntryTypeDef],
+        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MultiRegionConfigurationTypeDef = TypedDict(
-    "MultiRegionConfigurationTypeDef",
-    {
-        "MultiRegionKeyType": MultiRegionKeyTypeType,
-        "PrimaryKey": MultiRegionKeyTypeDef,
-        "ReplicaKeys": List[MultiRegionKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListGrantsResponseTypeDef = TypedDict(
     "ListGrantsResponseTypeDef",
     {
         "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeCustomKeyStoresResponseTypeDef = TypedDict(
-    "DescribeCustomKeyStoresResponseTypeDef",
-    {
-        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
     "_RequiredKeyMetadataTypeDef",
     {
         "KeyId": str,
@@ -1523,37 +1482,35 @@
         "PendingDeletionWindowInDays": int,
         "MacAlgorithms": List[MacAlgorithmSpecType],
         "XksKeyConfiguration": XksKeyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class KeyMetadataTypeDef(_RequiredKeyMetadataTypeDef, _OptionalKeyMetadataTypeDef):
     pass
 
-
 CreateKeyResponseTypeDef = TypedDict(
     "CreateKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicateKeyResponseTypeDef = TypedDict(
     "ReplicateKeyResponseTypeDef",
     {
         "ReplicaKeyMetadata": KeyMetadataTypeDef,
         "ReplicaPolicy": str,
         "ReplicaTags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms/type_defs.pyi` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kms.type_defs import AliasListEntryTypeDef
 
-    data: AliasListEntryTypeDef = {...}
+    data: AliasListEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -46,113 +46,118 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasListEntryTypeDef",
+    "BlobTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
-    "CancelKeyDeletionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
-    "CreateCustomKeyStoreResponseTypeDef",
     "GrantConstraintsTypeDef",
-    "CreateGrantResponseTypeDef",
     "TagTypeDef",
     "XksProxyConfigurationTypeTypeDef",
-    "RecipientInfoTypeDef",
-    "DecryptResponseTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCustomKeyStoreRequestRequestTypeDef",
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DisableKeyRequestRequestTypeDef",
     "DisableKeyRotationRequestRequestTypeDef",
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableKeyRequestRequestTypeDef",
     "EnableKeyRotationRequestRequestTypeDef",
-    "EncryptRequestRequestTypeDef",
-    "EncryptResponseTypeDef",
-    "GenerateDataKeyPairResponseTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    "GenerateDataKeyResponseTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
-    "GenerateMacRequestRequestTypeDef",
-    "GenerateMacResponseTypeDef",
-    "GenerateRandomResponseTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
-    "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
-    "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
-    "GetParametersForImportResponseTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
-    "GetPublicKeyResponseTypeDef",
-    "ImportKeyMaterialRequestRequestTypeDef",
+    "GrantConstraintsOutputTypeDef",
+    "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListGrantsRequestRequestTypeDef",
-    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
-    "ListKeyPoliciesResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
-    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
-    "PaginatorConfigTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
-    "ReEncryptRequestRequestTypeDef",
-    "ReEncryptResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
-    "ScheduleKeyDeletionResponseTypeDef",
-    "SignRequestRequestTypeDef",
-    "SignResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
+    "EncryptRequestRequestTypeDef",
+    "GenerateMacRequestRequestTypeDef",
+    "ReEncryptRequestRequestTypeDef",
+    "RecipientInfoTypeDef",
+    "SignRequestRequestTypeDef",
     "VerifyMacRequestRequestTypeDef",
-    "VerifyMacResponseTypeDef",
     "VerifyRequestRequestTypeDef",
-    "VerifyResponseTypeDef",
+    "CancelKeyDeletionResponseTypeDef",
+    "CreateCustomKeyStoreResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "DecryptResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EncryptResponseTypeDef",
+    "GenerateDataKeyPairResponseTypeDef",
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    "GenerateDataKeyResponseTypeDef",
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    "GenerateMacResponseTypeDef",
+    "GenerateRandomResponseTypeDef",
+    "GetKeyPolicyResponseTypeDef",
+    "GetKeyRotationStatusResponseTypeDef",
+    "GetParametersForImportResponseTypeDef",
+    "GetPublicKeyResponseTypeDef",
     "ListAliasesResponseTypeDef",
+    "ListKeyPoliciesResponseTypeDef",
+    "ReEncryptResponseTypeDef",
+    "ScheduleKeyDeletionResponseTypeDef",
+    "SignResponseTypeDef",
+    "VerifyMacResponseTypeDef",
+    "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "GrantListEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListGrantsRequestListGrantsPaginateTypeDef",
+    "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    "GrantConstraintsUnionTypeDef",
+    "GrantListEntryTypeDef",
+    "ImportKeyMaterialRequestRequestTypeDef",
+    "ListKeysResponseTypeDef",
+    "MultiRegionConfigurationTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
-    "ListKeysResponseTypeDef",
-    "MultiRegionConfigurationTypeDef",
-    "ListGrantsResponseTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
+    "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
 
 AliasListEntryTypeDef = TypedDict(
@@ -163,26 +168,30 @@
         "TargetKeyId": str,
         "CreationDate": datetime,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelKeyDeletionRequestRequestTypeDef = TypedDict(
     "CancelKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-CancelKeyDeletionResponseTypeDef = TypedDict(
-    "CancelKeyDeletionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
@@ -201,40 +210,23 @@
     "XksProxyAuthenticationCredentialTypeTypeDef",
     {
         "AccessKeyId": str,
         "RawSecretAccessKey": str,
     },
 )
 
-CreateCustomKeyStoreResponseTypeDef = TypedDict(
-    "CreateCustomKeyStoreResponseTypeDef",
-    {
-        "CustomKeyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GrantConstraintsTypeDef = TypedDict(
     "GrantConstraintsTypeDef",
     {
         "EncryptionContextSubset": Mapping[str, str],
         "EncryptionContextEquals": Mapping[str, str],
     },
     total=False,
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantToken": str,
-        "GrantId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "TagKey": str,
         "TagValue": str,
     },
 )
@@ -247,34 +239,14 @@
         "UriEndpoint": str,
         "UriPath": str,
         "VpcEndpointServiceName": str,
     },
     total=False,
 )
 
-RecipientInfoTypeDef = TypedDict(
-    "RecipientInfoTypeDef",
-    {
-        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
-        "AttestationDocument": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-DecryptResponseTypeDef = TypedDict(
-    "DecryptResponseTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": bytes,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -288,20 +260,20 @@
 DeleteImportedKeyMaterialRequestRequestTypeDef = TypedDict(
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
-    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CustomKeyStoreId": str,
-        "CustomKeyStoreName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCustomKeyStoresRequestRequestTypeDef = TypedDict(
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     {
@@ -323,19 +295,21 @@
     "_OptionalDescribeKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeKeyRequestRequestTypeDef(
     _RequiredDescribeKeyRequestRequestTypeDef, _OptionalDescribeKeyRequestRequestTypeDef
 ):
     pass
 
+
 DisableKeyRequestRequestTypeDef = TypedDict(
     "DisableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -349,80 +323,28 @@
 DisconnectCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableKeyRequestRequestTypeDef = TypedDict(
     "EnableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
 EnableKeyRotationRequestRequestTypeDef = TypedDict(
     "EnableKeyRotationRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-_RequiredEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredEncryptRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalEncryptRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-    },
-    total=False,
-)
-
-class EncryptRequestRequestTypeDef(
-    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
-):
-    pass
-
-EncryptResponseTypeDef = TypedDict(
-    "EncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyPairResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PrivateKeyPlaintext": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -431,41 +353,21 @@
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
-    {
-        "PrivateKeyCiphertextBlob": bytes,
-        "PublicKey": bytes,
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateDataKeyResponseTypeDef = TypedDict(
-    "GenerateDataKeyResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "Plaintext": bytes,
-        "KeyId": str,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -476,175 +378,77 @@
         "KeySpec": DataKeySpecType,
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
-    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateMacRequestRequestTypeDef",
-    {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "KeyId": str,
-        "MacAlgorithm": MacAlgorithmSpecType,
-    },
-)
-_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateMacRequestRequestTypeDef",
-    {
-        "GrantTokens": Sequence[str],
-    },
-    total=False,
-)
-
-class GenerateMacRequestRequestTypeDef(
-    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
-):
-    pass
-
-GenerateMacResponseTypeDef = TypedDict(
-    "GenerateMacResponseTypeDef",
-    {
-        "Mac": bytes,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "KeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateRandomResponseTypeDef = TypedDict(
-    "GenerateRandomResponseTypeDef",
-    {
-        "Plaintext": bytes,
-        "CiphertextForRecipient": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetKeyPolicyRequestRequestTypeDef = TypedDict(
     "GetKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
     },
 )
 
-GetKeyPolicyResponseTypeDef = TypedDict(
-    "GetKeyPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKeyRotationStatusRequestRequestTypeDef = TypedDict(
     "GetKeyRotationStatusRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-GetKeyRotationStatusResponseTypeDef = TypedDict(
-    "GetKeyRotationStatusResponseTypeDef",
-    {
-        "KeyRotationEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParametersForImportRequestRequestTypeDef = TypedDict(
     "GetParametersForImportRequestRequestTypeDef",
     {
         "KeyId": str,
         "WrappingAlgorithm": AlgorithmSpecType,
         "WrappingKeySpec": WrappingKeySpecType,
     },
 )
 
-GetParametersForImportResponseTypeDef = TypedDict(
-    "GetParametersForImportResponseTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": bytes,
-        "PublicKey": bytes,
-        "ParametersValidTo": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGetPublicKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGetPublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalGetPublicKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
-GetPublicKeyResponseTypeDef = TypedDict(
-    "GetPublicKeyResponseTypeDef",
-    {
-        "KeyId": str,
-        "PublicKey": bytes,
-        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
-        "KeySpec": KeySpecType,
-        "KeyUsage": KeyUsageTypeType,
-        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
-        "SigningAlgorithms": List[SigningAlgorithmSpecType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_RequiredImportKeyMaterialRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": Union[str, bytes, IO[Any], StreamingBody],
-        "EncryptedKeyMaterial": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_OptionalImportKeyMaterialRequestRequestTypeDef",
+GrantConstraintsOutputTypeDef = TypedDict(
+    "GrantConstraintsOutputTypeDef",
     {
-        "ValidTo": Union[datetime, str],
-        "ExpirationModel": ExpirationModelTypeType,
+        "EncryptionContextSubset": Dict[str, str],
+        "EncryptionContextEquals": Dict[str, str],
     },
     total=False,
 )
 
-class ImportKeyMaterialRequestRequestTypeDef(
-    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -654,55 +458,24 @@
     "XksKeyConfigurationTypeTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "KeyId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAliasesRequestRequestTypeDef = TypedDict(
     "ListAliasesRequestRequestTypeDef",
     {
         "KeyId": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
-    {
-        "GrantId": str,
-        "GranteePrincipal": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGrantsRequestListGrantsPaginateTypeDef(
-    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
-    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListGrantsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListGrantsRequestRequestTypeDef = TypedDict(
@@ -712,38 +485,20 @@
         "Marker": str,
         "GrantId": str,
         "GranteePrincipal": str,
     },
     total=False,
 )
 
+
 class ListGrantsRequestRequestTypeDef(
     _RequiredListGrantsRequestRequestTypeDef, _OptionalListGrantsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
-    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListKeyPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -752,66 +507,30 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListKeyPoliciesRequestRequestTypeDef(
     _RequiredListKeyPoliciesRequestRequestTypeDef, _OptionalListKeyPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListKeyPoliciesResponseTypeDef = TypedDict(
-    "ListKeyPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
-    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
-    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceTagsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListResourceTagsRequestRequestTypeDef = TypedDict(
@@ -819,38 +538,20 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListResourceTagsRequestRequestTypeDef(
     _RequiredListResourceTagsRequestRequestTypeDef, _OptionalListResourceTagsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "RetiringPrincipal": str,
-    },
-)
-_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
-    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
-    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
-):
-    pass
 
 _RequiredListRetirableGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
@@ -859,39 +560,31 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListRetirableGrantsRequestRequestTypeDef(
     _RequiredListRetirableGrantsRequestRequestTypeDef,
     _OptionalListRetirableGrantsRequestRequestTypeDef,
 ):
     pass
 
+
 MultiRegionKeyTypeDef = TypedDict(
     "MultiRegionKeyTypeDef",
     {
         "Arn": str,
         "Region": str,
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
 _RequiredPutKeyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -900,66 +593,20 @@
     "_OptionalPutKeyPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
+
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
-_RequiredReEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredReEncryptRequestRequestTypeDef",
-    {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "DestinationKeyId": str,
-    },
-)
-_OptionalReEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalReEncryptRequestRequestTypeDef",
-    {
-        "SourceEncryptionContext": Mapping[str, str],
-        "SourceKeyId": str,
-        "DestinationEncryptionContext": Mapping[str, str],
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "GrantTokens": Sequence[str],
-    },
-    total=False,
-)
-
-class ReEncryptRequestRequestTypeDef(
-    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
-):
-    pass
-
-ReEncryptResponseTypeDef = TypedDict(
-    "ReEncryptResponseTypeDef",
-    {
-        "CiphertextBlob": bytes,
-        "SourceKeyId": str,
-        "KeyId": str,
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
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
 
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
@@ -985,167 +632,437 @@
     "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
     {
         "PendingWindowInDays": int,
     },
     total=False,
 )
 
+
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
-ScheduleKeyDeletionResponseTypeDef = TypedDict(
-    "ScheduleKeyDeletionResponseTypeDef",
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
-        "DeletionDate": datetime,
-        "KeyState": KeyStateType,
-        "PendingWindowInDays": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagKeys": Sequence[str],
     },
 )
 
-_RequiredSignRequestRequestTypeDef = TypedDict(
-    "_RequiredSignRequestRequestTypeDef",
+UpdateAliasRequestRequestTypeDef = TypedDict(
+    "UpdateAliasRequestRequestTypeDef",
+    {
+        "AliasName": str,
+        "TargetKeyId": str,
+    },
+)
+
+UpdateKeyDescriptionRequestRequestTypeDef = TypedDict(
+    "UpdateKeyDescriptionRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "Description": str,
     },
 )
-_OptionalSignRequestRequestTypeDef = TypedDict(
-    "_OptionalSignRequestRequestTypeDef",
+
+UpdatePrimaryRegionRequestRequestTypeDef = TypedDict(
+    "UpdatePrimaryRegionRequestRequestTypeDef",
     {
-        "MessageType": MessageTypeType,
+        "KeyId": str,
+        "PrimaryRegion": str,
+    },
+)
+
+_RequiredEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredEncryptRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Plaintext": BlobTypeDef,
+    },
+)
+_OptionalEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalEncryptRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
     },
     total=False,
 )
 
-class SignRequestRequestTypeDef(
-    _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
+
+class EncryptRequestRequestTypeDef(
+    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
     pass
 
-SignResponseTypeDef = TypedDict(
-    "SignResponseTypeDef",
+
+_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateMacRequestRequestTypeDef",
     {
+        "Message": BlobTypeDef,
         "KeyId": str,
-        "Signature": bytes,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MacAlgorithm": MacAlgorithmSpecType,
     },
 )
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateMacRequestRequestTypeDef",
     {
-        "KeyId": str,
-        "TagKeys": Sequence[str],
+        "GrantTokens": Sequence[str],
     },
+    total=False,
 )
 
-UpdateAliasRequestRequestTypeDef = TypedDict(
-    "UpdateAliasRequestRequestTypeDef",
+
+class GenerateMacRequestRequestTypeDef(
+    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredReEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredReEncryptRequestRequestTypeDef",
     {
-        "AliasName": str,
-        "TargetKeyId": str,
+        "CiphertextBlob": BlobTypeDef,
+        "DestinationKeyId": str,
+    },
+)
+_OptionalReEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalReEncryptRequestRequestTypeDef",
+    {
+        "SourceEncryptionContext": Mapping[str, str],
+        "SourceKeyId": str,
+        "DestinationEncryptionContext": Mapping[str, str],
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "GrantTokens": Sequence[str],
     },
+    total=False,
 )
 
-UpdateKeyDescriptionRequestRequestTypeDef = TypedDict(
-    "UpdateKeyDescriptionRequestRequestTypeDef",
+
+class ReEncryptRequestRequestTypeDef(
+    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
+):
+    pass
+
+
+RecipientInfoTypeDef = TypedDict(
+    "RecipientInfoTypeDef",
     {
-        "KeyId": str,
-        "Description": str,
+        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
+        "AttestationDocument": BlobTypeDef,
     },
+    total=False,
 )
 
-UpdatePrimaryRegionRequestRequestTypeDef = TypedDict(
-    "UpdatePrimaryRegionRequestRequestTypeDef",
+_RequiredSignRequestRequestTypeDef = TypedDict(
+    "_RequiredSignRequestRequestTypeDef",
     {
         "KeyId": str,
-        "PrimaryRegion": str,
+        "Message": BlobTypeDef,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+    },
+)
+_OptionalSignRequestRequestTypeDef = TypedDict(
+    "_OptionalSignRequestRequestTypeDef",
+    {
+        "MessageType": MessageTypeType,
+        "GrantTokens": Sequence[str],
     },
+    total=False,
 )
 
+
+class SignRequestRequestTypeDef(
+    _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredVerifyMacRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyMacRequestRequestTypeDef",
     {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
         "KeyId": str,
         "MacAlgorithm": MacAlgorithmSpecType,
-        "Mac": Union[str, bytes, IO[Any], StreamingBody],
+        "Mac": BlobTypeDef,
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
     pass
 
-VerifyMacResponseTypeDef = TypedDict(
-    "VerifyMacResponseTypeDef",
-    {
-        "KeyId": str,
-        "MacValid": bool,
-        "MacAlgorithm": MacAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredVerifyRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "Signature": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
+        "Signature": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmSpecType,
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
     pass
 
-VerifyResponseTypeDef = TypedDict(
-    "VerifyResponseTypeDef",
+
+CancelKeyDeletionResponseTypeDef = TypedDict(
+    "CancelKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
-        "SignatureValid": bool,
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomKeyStoreResponseTypeDef = TypedDict(
+    "CreateCustomKeyStoreResponseTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
+    {
+        "GrantToken": str,
+        "GrantId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DecryptResponseTypeDef = TypedDict(
+    "DecryptResponseTypeDef",
+    {
+        "KeyId": str,
+        "Plaintext": bytes,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "CiphertextForRecipient": bytes,
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
+EncryptResponseTypeDef = TypedDict(
+    "EncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyPairResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PrivateKeyPlaintext": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
+    {
+        "PrivateKeyCiphertextBlob": bytes,
+        "PublicKey": bytes,
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyResponseTypeDef = TypedDict(
+    "GenerateDataKeyResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "Plaintext": bytes,
+        "KeyId": str,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
+    "GenerateDataKeyWithoutPlaintextResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMacResponseTypeDef = TypedDict(
+    "GenerateMacResponseTypeDef",
+    {
+        "Mac": bytes,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateRandomResponseTypeDef = TypedDict(
+    "GenerateRandomResponseTypeDef",
+    {
+        "Plaintext": bytes,
+        "CiphertextForRecipient": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyPolicyResponseTypeDef = TypedDict(
+    "GetKeyPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyRotationStatusResponseTypeDef = TypedDict(
+    "GetKeyRotationStatusResponseTypeDef",
+    {
+        "KeyRotationEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForImportResponseTypeDef = TypedDict(
+    "GetParametersForImportResponseTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": bytes,
+        "PublicKey": bytes,
+        "ParametersValidTo": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicKeyResponseTypeDef = TypedDict(
+    "GetPublicKeyResponseTypeDef",
+    {
+        "KeyId": str,
+        "PublicKey": bytes,
+        "CustomerMasterKeySpec": CustomerMasterKeySpecType,
+        "KeySpec": KeySpecType,
+        "KeyUsage": KeyUsageTypeType,
+        "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
+        "SigningAlgorithms": List[SigningAlgorithmSpecType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "Aliases": List[AliasListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListKeyPoliciesResponseTypeDef = TypedDict(
+    "ListKeyPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReEncryptResponseTypeDef = TypedDict(
+    "ReEncryptResponseTypeDef",
+    {
+        "CiphertextBlob": bytes,
+        "SourceKeyId": str,
+        "KeyId": str,
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduleKeyDeletionResponseTypeDef = TypedDict(
+    "ScheduleKeyDeletionResponseTypeDef",
+    {
+        "KeyId": str,
+        "DeletionDate": datetime,
+        "KeyState": KeyStateType,
+        "PendingWindowInDays": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignResponseTypeDef = TypedDict(
+    "SignResponseTypeDef",
+    {
+        "KeyId": str,
+        "Signature": bytes,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyMacResponseTypeDef = TypedDict(
+    "VerifyMacResponseTypeDef",
+    {
+        "KeyId": str,
+        "MacValid": bool,
+        "MacAlgorithm": MacAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyResponseTypeDef = TypedDict(
+    "VerifyResponseTypeDef",
+    {
+        "KeyId": str,
+        "SignatureValid": bool,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreName": str,
@@ -1163,20 +1080,22 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
+
 class CreateCustomKeyStoreRequestRequestTypeDef(
     _RequiredCreateCustomKeyStoreRequestRequestTypeDef,
     _OptionalCreateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 _OptionalUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
@@ -1190,20 +1109,22 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
+
 class UpdateCustomKeyStoreRequestRequestTypeDef(
     _RequiredUpdateCustomKeyStoreRequestRequestTypeDef,
     _OptionalUpdateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateGrantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GranteePrincipal": str,
         "Operations": Sequence[GrantOperationType],
     },
@@ -1215,34 +1136,20 @@
         "Constraints": GrantConstraintsTypeDef,
         "GrantTokens": Sequence[str],
         "Name": str,
     },
     total=False,
 )
 
+
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
-GrantListEntryTypeDef = TypedDict(
-    "GrantListEntryTypeDef",
-    {
-        "KeyId": str,
-        "GrantId": str,
-        "Name": str,
-        "CreationDate": datetime,
-        "GranteePrincipal": str,
-        "RetiringPrincipal": str,
-        "IssuingAccount": str,
-        "Operations": List[GrantOperationType],
-        "Constraints": GrantConstraintsTypeDef,
-    },
-    total=False,
-)
 
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
@@ -1260,15 +1167,15 @@
 
 ListResourceTagsResponseTypeDef = TypedDict(
     "ListResourceTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredReplicateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateKeyRequestRequestTypeDef",
     {
         "KeyId": str,
@@ -1282,19 +1189,21 @@
         "BypassPolicyLockoutSafetyCheck": bool,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ReplicateKeyRequestRequestTypeDef(
     _RequiredReplicateKeyRequestRequestTypeDef, _OptionalReplicateKeyRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1311,37 +1220,217 @@
         "CreationDate": datetime,
         "CustomKeyStoreType": CustomKeyStoreTypeType,
         "XksProxyConfiguration": XksProxyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
+    "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
+    {
+        "CustomKeyStoreId": str,
+        "CustomKeyStoreName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "KeyId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListGrantsRequestListGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListGrantsRequestListGrantsPaginateTypeDef",
+    {
+        "GrantId": str,
+        "GranteePrincipal": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGrantsRequestListGrantsPaginateTypeDef(
+    _RequiredListGrantsRequestListGrantsPaginateTypeDef,
+    _OptionalListGrantsRequestListGrantsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
+    _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+):
+    pass
+
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
+    _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "RetiringPrincipal": str,
+    },
+)
+_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
+    "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
+    _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+):
+    pass
+
+
+GrantConstraintsUnionTypeDef = Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef]
+GrantListEntryTypeDef = TypedDict(
+    "GrantListEntryTypeDef",
+    {
+        "KeyId": str,
+        "GrantId": str,
+        "Name": str,
+        "CreationDate": datetime,
+        "GranteePrincipal": str,
+        "RetiringPrincipal": str,
+        "IssuingAccount": str,
+        "Operations": List[GrantOperationType],
+        "Constraints": GrantConstraintsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_RequiredImportKeyMaterialRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": BlobTypeDef,
+        "EncryptedKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_OptionalImportKeyMaterialRequestRequestTypeDef",
+    {
+        "ValidTo": TimestampTypeDef,
+        "ExpirationModel": ExpirationModelTypeType,
+    },
+    total=False,
+)
+
+
+class ImportKeyMaterialRequestRequestTypeDef(
+    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
+):
+    pass
+
+
+ListKeysResponseTypeDef = TypedDict(
+    "ListKeysResponseTypeDef",
+    {
+        "Keys": List[KeyListEntryTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MultiRegionConfigurationTypeDef = TypedDict(
+    "MultiRegionConfigurationTypeDef",
+    {
+        "MultiRegionKeyType": MultiRegionKeyTypeType,
+        "PrimaryKey": MultiRegionKeyTypeDef,
+        "ReplicaKeys": List[MultiRegionKeyTypeDef],
+    },
+    total=False,
+)
+
 _RequiredDecryptRequestRequestTypeDef = TypedDict(
     "_RequiredDecryptRequestRequestTypeDef",
     {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "CiphertextBlob": BlobTypeDef,
     },
 )
 _OptionalDecryptRequestRequestTypeDef = TypedDict(
     "_OptionalDecryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -1351,20 +1440,22 @@
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
@@ -1375,66 +1466,48 @@
         "KeySpec": DataKeySpecType,
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
     pass
 
+
 GenerateRandomRequestRequestTypeDef = TypedDict(
     "GenerateRandomRequestRequestTypeDef",
     {
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-ListKeysResponseTypeDef = TypedDict(
-    "ListKeysResponseTypeDef",
+DescribeCustomKeyStoresResponseTypeDef = TypedDict(
+    "DescribeCustomKeyStoresResponseTypeDef",
     {
-        "Keys": List[KeyListEntryTypeDef],
+        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MultiRegionConfigurationTypeDef = TypedDict(
-    "MultiRegionConfigurationTypeDef",
-    {
-        "MultiRegionKeyType": MultiRegionKeyTypeType,
-        "PrimaryKey": MultiRegionKeyTypeDef,
-        "ReplicaKeys": List[MultiRegionKeyTypeDef],
-    },
-    total=False,
-)
-
 ListGrantsResponseTypeDef = TypedDict(
     "ListGrantsResponseTypeDef",
     {
         "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeCustomKeyStoresResponseTypeDef = TypedDict(
-    "DescribeCustomKeyStoresResponseTypeDef",
-    {
-        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
     "_RequiredKeyMetadataTypeDef",
     {
         "KeyId": str,
@@ -1466,35 +1539,37 @@
         "PendingDeletionWindowInDays": int,
         "MacAlgorithms": List[MacAlgorithmSpecType],
         "XksKeyConfiguration": XksKeyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class KeyMetadataTypeDef(_RequiredKeyMetadataTypeDef, _OptionalKeyMetadataTypeDef):
     pass
 
+
 CreateKeyResponseTypeDef = TypedDict(
     "CreateKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicateKeyResponseTypeDef = TypedDict(
     "ReplicateKeyResponseTypeDef",
     {
         "ReplicaKeyMetadata": KeyMetadataTypeDef,
         "ReplicaPolicy": str,
         "ReplicaTags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/PKG-INFO` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KMS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kms"></a>
 
 # types-aiobotocore-kms
 
 [![PyPI - types-aiobotocore-kms](https://img.shields.io/pypi/v/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kms?color=blue)](https://pypistats.org/packages/types-aiobotocore-kms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kms)](https://pepy.tech/project/types-aiobotocore-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [types-aiobotocore-kms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/).
 
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
@@ -353,129 +352,133 @@
 )
 
 
 def check_value(value: AlgorithmSpecType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kms.type_defs import (
     AliasListEntryTypeDef,
+    BlobTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
-    CancelKeyDeletionResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
-    CreateCustomKeyStoreResponseTypeDef,
     GrantConstraintsTypeDef,
-    CreateGrantResponseTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
-    RecipientInfoTypeDef,
-    DecryptResponseTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
-    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
-    EncryptRequestRequestTypeDef,
-    EncryptResponseTypeDef,
-    GenerateDataKeyPairResponseTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
-    GenerateDataKeyResponseTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateDataKeyWithoutPlaintextResponseTypeDef,
-    GenerateMacRequestRequestTypeDef,
-    GenerateMacResponseTypeDef,
-    GenerateRandomResponseTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
-    GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
-    GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
-    GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
-    GetPublicKeyResponseTypeDef,
-    ImportKeyMaterialRequestRequestTypeDef,
+    GrantConstraintsOutputTypeDef,
+    TimestampTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
-    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
-    ListKeyPoliciesResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
-    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
-    PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
-    ReEncryptRequestRequestTypeDef,
-    ReEncryptResponseTypeDef,
-    ResponseMetadataTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    ScheduleKeyDeletionResponseTypeDef,
-    SignRequestRequestTypeDef,
-    SignResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
+    EncryptRequestRequestTypeDef,
+    GenerateMacRequestRequestTypeDef,
+    ReEncryptRequestRequestTypeDef,
+    RecipientInfoTypeDef,
+    SignRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
-    VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
-    VerifyResponseTypeDef,
+    CancelKeyDeletionResponseTypeDef,
+    CreateCustomKeyStoreResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    DecryptResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EncryptResponseTypeDef,
+    GenerateDataKeyPairResponseTypeDef,
+    GenerateDataKeyPairWithoutPlaintextResponseTypeDef,
+    GenerateDataKeyResponseTypeDef,
+    GenerateDataKeyWithoutPlaintextResponseTypeDef,
+    GenerateMacResponseTypeDef,
+    GenerateRandomResponseTypeDef,
+    GetKeyPolicyResponseTypeDef,
+    GetKeyRotationStatusResponseTypeDef,
+    GetParametersForImportResponseTypeDef,
+    GetPublicKeyResponseTypeDef,
     ListAliasesResponseTypeDef,
+    ListKeyPoliciesResponseTypeDef,
+    ReEncryptResponseTypeDef,
+    ScheduleKeyDeletionResponseTypeDef,
+    SignResponseTypeDef,
+    VerifyMacResponseTypeDef,
+    VerifyResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
-    GrantListEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
     ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
+    DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListGrantsRequestListGrantsPaginateTypeDef,
+    ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListResourceTagsRequestListResourceTagsPaginateTypeDef,
+    ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    GrantConstraintsUnionTypeDef,
+    GrantListEntryTypeDef,
+    ImportKeyMaterialRequestRequestTypeDef,
+    ListKeysResponseTypeDef,
+    MultiRegionConfigurationTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
-    ListKeysResponseTypeDef,
-    MultiRegionConfigurationTypeDef,
-    ListGrantsResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
+    ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
 
 
-def get_structure() -> AliasListEntryTypeDef:
+def get_value() -> AliasListEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kms-2.5.2/types_aiobotocore_kms.egg-info/SOURCES.txt` & `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


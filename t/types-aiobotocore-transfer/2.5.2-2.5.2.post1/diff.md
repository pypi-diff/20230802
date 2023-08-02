# Comparing `tmp/types-aiobotocore-transfer-2.5.2.tar.gz` & `tmp/types-aiobotocore-transfer-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transfer-2.5.2.tar", last modified: Sat Jul  8 01:44:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-transfer-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
```

## Comparing `types-aiobotocore-transfer-2.5.2.tar` & `types-aiobotocore-transfer-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.183011 types-aiobotocore-transfer-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-07-08 01:44:26.175011 types-aiobotocore-transfer-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:26.183011 types-aiobotocore-transfer-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:42:04.000000 types-aiobotocore-transfer-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.171011 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48970 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-08 01:42:08.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59204 2023-07-08 01:42:09.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59115 2023-07-08 01:42:08.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-08 01:42:05.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.175011 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-07-08 01:44:26.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-08 01:44:26.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:26.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:26.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:26.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:26.000000 types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.097434 types-aiobotocore-transfer-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22452 2023-08-02 14:53:08.081435 types-aiobotocore-transfer-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.097434 types-aiobotocore-transfer-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49024 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48944 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-08-02 14:50:44.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61839 2023-08-02 14:50:45.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61749 2023-08-02 14:50:44.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22452 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transfer-2.5.2/LICENSE` & `types-aiobotocore-transfer-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/PKG-INFO` & `types-aiobotocore-transfer-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-transfer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore transfer type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-transfer"></a>
 
 # types-aiobotocore-transfer
 
 [![PyPI - types-aiobotocore-transfer](https://img.shields.io/pypi/v/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-transfer?color=blue)](https://pypistats.org/packages/types-aiobotocore-transfer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Transfer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [types-aiobotocore-transfer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +42,15 @@
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
@@ -395,37 +362,31 @@
 )
 
 
 def check_value(value: AgreementStatusTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_transfer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_transfer.type_defs import (
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
-    CreateAccessResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAgreementResponseTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateProfileResponseTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CreateServerResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
@@ -443,146 +404,164 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
+    PosixProfileOutputTypeDef,
     LoggingConfigurationTypeDef,
+    EndpointDetailsOutputTypeDef,
+    ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
     EfsFileLocationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
-    ImportCertificateResponseTypeDef,
-    ImportHostKeyResponseTypeDef,
+    TimestampTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    ImportSshPublicKeyResponseTypeDef,
     S3InputFileLocationTypeDef,
-    ListAccessesRequestListAccessesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
-    ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListedCertificateTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListedConnectorTypeDef,
-    ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListExecutionsRequestRequestTypeDef,
     ListHostKeysRequestRequestTypeDef,
     ListedHostKeyTypeDef,
-    ListProfilesRequestListProfilesPaginateTypeDef,
     ListProfilesRequestRequestTypeDef,
     ListedProfileTypeDef,
-    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
-    ListSecurityPoliciesResponseTypeDef,
-    ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
-    StartFileTransferResponseTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
-    TestIdentityProviderResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAccessResponseTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateAgreementResponseTypeDef,
-    UpdateCertificateRequestRequestTypeDef,
-    UpdateCertificateResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
-    UpdateHostKeyResponseTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    UpdateProfileResponseTypeDef,
-    UpdateServerResponseTypeDef,
-    UpdateUserResponseTypeDef,
     WorkflowDetailTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     CreateAccessRequestRequestTypeDef,
-    DescribedAccessTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    CreateAccessResponseTypeDef,
+    CreateAgreementResponseTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    CreateServerResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ImportCertificateResponseTypeDef,
+    ImportHostKeyResponseTypeDef,
+    ImportSshPublicKeyResponseTypeDef,
+    ListSecurityPoliciesResponseTypeDef,
+    StartFileTransferResponseTypeDef,
+    TestIdentityProviderResponseTypeDef,
+    UpdateAccessResponseTypeDef,
+    UpdateAgreementResponseTypeDef,
+    UpdateCertificateResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
+    UpdateHostKeyResponseTypeDef,
+    UpdateProfileResponseTypeDef,
+    UpdateServerResponseTypeDef,
+    UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribedAgreementTypeDef,
     DescribedCertificateTypeDef,
     DescribedConnectorTypeDef,
     DescribedHostKeyTypeDef,
     DescribedProfileTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
+    DescribedAccessTypeDef,
+    PosixProfileUnionTypeDef,
+    EndpointDetailsUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    ImportCertificateRequestRequestTypeDef,
+    UpdateCertificateRequestRequestTypeDef,
     InputFileLocationTypeDef,
+    ListAccessesRequestListAccessesPaginateTypeDef,
+    ListAgreementsRequestListAgreementsPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListExecutionsRequestListExecutionsPaginateTypeDef,
+    ListProfilesRequestListProfilesPaginateTypeDef,
+    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
+    ListServersRequestListServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
     ListCertificatesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListServersResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
-    DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeAccessResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
-    CreateServerRequestRequestTypeDef,
     DescribedServerTypeDef,
+    CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    WorkflowDetailsUnionTypeDef,
     DescribedExecutionTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
     DescribedWorkflowTypeDef,
+    WorkflowStepUnionTypeDef,
     DescribeWorkflowResponseTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_value() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-transfer-2.5.2/README.md` & `types-aiobotocore-transfer-2.5.2.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-transfer
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore transfer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-transfer"></a>
 
 # types-aiobotocore-transfer
 
 [![PyPI - types-aiobotocore-transfer](https://img.shields.io/pypi/v/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-transfer?color=blue)](https://pypistats.org/packages/types-aiobotocore-transfer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Transfer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [types-aiobotocore-transfer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -362,37 +394,31 @@
 )
 
 
 def check_value(value: AgreementStatusTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_transfer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_transfer.type_defs import (
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
-    CreateAccessResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAgreementResponseTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateProfileResponseTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CreateServerResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
@@ -410,146 +436,164 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
+    PosixProfileOutputTypeDef,
     LoggingConfigurationTypeDef,
+    EndpointDetailsOutputTypeDef,
+    ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
     EfsFileLocationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
-    ImportCertificateResponseTypeDef,
-    ImportHostKeyResponseTypeDef,
+    TimestampTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    ImportSshPublicKeyResponseTypeDef,
     S3InputFileLocationTypeDef,
-    ListAccessesRequestListAccessesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
-    ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListedCertificateTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListedConnectorTypeDef,
-    ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListExecutionsRequestRequestTypeDef,
     ListHostKeysRequestRequestTypeDef,
     ListedHostKeyTypeDef,
-    ListProfilesRequestListProfilesPaginateTypeDef,
     ListProfilesRequestRequestTypeDef,
     ListedProfileTypeDef,
-    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
-    ListSecurityPoliciesResponseTypeDef,
-    ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
-    StartFileTransferResponseTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
-    TestIdentityProviderResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAccessResponseTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateAgreementResponseTypeDef,
-    UpdateCertificateRequestRequestTypeDef,
-    UpdateCertificateResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
-    UpdateHostKeyResponseTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    UpdateProfileResponseTypeDef,
-    UpdateServerResponseTypeDef,
-    UpdateUserResponseTypeDef,
     WorkflowDetailTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     CreateAccessRequestRequestTypeDef,
-    DescribedAccessTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    CreateAccessResponseTypeDef,
+    CreateAgreementResponseTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    CreateServerResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ImportCertificateResponseTypeDef,
+    ImportHostKeyResponseTypeDef,
+    ImportSshPublicKeyResponseTypeDef,
+    ListSecurityPoliciesResponseTypeDef,
+    StartFileTransferResponseTypeDef,
+    TestIdentityProviderResponseTypeDef,
+    UpdateAccessResponseTypeDef,
+    UpdateAgreementResponseTypeDef,
+    UpdateCertificateResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
+    UpdateHostKeyResponseTypeDef,
+    UpdateProfileResponseTypeDef,
+    UpdateServerResponseTypeDef,
+    UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribedAgreementTypeDef,
     DescribedCertificateTypeDef,
     DescribedConnectorTypeDef,
     DescribedHostKeyTypeDef,
     DescribedProfileTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
+    DescribedAccessTypeDef,
+    PosixProfileUnionTypeDef,
+    EndpointDetailsUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    ImportCertificateRequestRequestTypeDef,
+    UpdateCertificateRequestRequestTypeDef,
     InputFileLocationTypeDef,
+    ListAccessesRequestListAccessesPaginateTypeDef,
+    ListAgreementsRequestListAgreementsPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListExecutionsRequestListExecutionsPaginateTypeDef,
+    ListProfilesRequestListProfilesPaginateTypeDef,
+    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
+    ListServersRequestListServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
     ListCertificatesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListServersResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
-    DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeAccessResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
-    CreateServerRequestRequestTypeDef,
     DescribedServerTypeDef,
+    CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    WorkflowDetailsUnionTypeDef,
     DescribedExecutionTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
     DescribedWorkflowTypeDef,
+    WorkflowStepUnionTypeDef,
     DescribeWorkflowResponseTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_value() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-transfer-2.5.2/setup.py` & `types-aiobotocore-transfer-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transfer",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore transfer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore transfer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_transfer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/"
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/__init__.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/__init__.pyi` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/__main__.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Transfer 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Transfer 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/client.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("transfer") as client:
         client: TransferClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AgreementStatusTypeType,
     CertificateUsageTypeType,
@@ -62,15 +61,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointDetailsTypeDef,
+    EndpointDetailsUnionTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
@@ -80,29 +79,30 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
-    PosixProfileTypeDef,
-    ProtocolDetailsTypeDef,
+    PosixProfileUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestIdentityProviderResponseTypeDef,
+    TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
-    WorkflowDetailsTypeDef,
-    WorkflowStepTypeDef,
+    WorkflowDetailsUnionTypeDef,
+    WorkflowStepUnionTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,15 +171,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...
+        PosixProfile: PosixProfileUnionTypeDef = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -238,27 +238,27 @@
         """
 
     async def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -271,32 +271,32 @@
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_user)
         """
 
     async def create_workflow(
         self,
         *,
-        Steps: Sequence[WorkflowStepTypeDef],
+        Steps: Sequence[WorkflowStepUnionTypeDef],
         Description: str = ...,
-        OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
+        OnExceptionSteps: Sequence[WorkflowStepUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -518,16 +518,16 @@
     async def import_certificate(
         self,
         *,
         Usage: CertificateUsageTypeType,
         Certificate: str,
         CertificateChain: str = ...,
         PrivateKey: str = ...,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports the signing and encryption certificates that you need to create local
         (AS2) profiles and partner profiles.
 
@@ -773,15 +773,15 @@
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -807,16 +807,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_agreement)
         """
 
     async def update_certificate(
         self,
         *,
         CertificateId: str,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...
     ) -> UpdateCertificateResponseTypeDef:
         """
         Updates the active and inactive dates for a certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_certificate)
@@ -860,25 +860,25 @@
         """
 
     async def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -890,15 +890,15 @@
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_user)
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/client.pyi` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("transfer") as client:
         client: TransferClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AgreementStatusTypeType,
     CertificateUsageTypeType,
@@ -62,15 +61,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointDetailsTypeDef,
+    EndpointDetailsUnionTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
@@ -80,29 +79,30 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
-    PosixProfileTypeDef,
-    ProtocolDetailsTypeDef,
+    PosixProfileUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestIdentityProviderResponseTypeDef,
+    TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
-    WorkflowDetailsTypeDef,
-    WorkflowStepTypeDef,
+    WorkflowDetailsUnionTypeDef,
+    WorkflowStepUnionTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -164,15 +164,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...
+        PosixProfile: PosixProfileUnionTypeDef = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -227,27 +227,27 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_profile)
         """
     async def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -259,31 +259,31 @@
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_user)
         """
     async def create_workflow(
         self,
         *,
-        Steps: Sequence[WorkflowStepTypeDef],
+        Steps: Sequence[WorkflowStepUnionTypeDef],
         Description: str = ...,
-        OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
+        OnExceptionSteps: Sequence[WorkflowStepUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -482,16 +482,16 @@
     async def import_certificate(
         self,
         *,
         Usage: CertificateUsageTypeType,
         Certificate: str,
         CertificateChain: str = ...,
         PrivateKey: str = ...,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports the signing and encryption certificates that you need to create local
         (AS2) profiles and partner profiles.
 
@@ -715,15 +715,15 @@
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -747,16 +747,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_agreement)
         """
     async def update_certificate(
         self,
         *,
         CertificateId: str,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...
     ) -> UpdateCertificateResponseTypeDef:
         """
         Updates the active and inactive dates for a certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_certificate)
@@ -796,25 +796,25 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_profile)
         """
     async def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: ProtocolDetailsTypeDef = ...,
-        EndpointDetails: EndpointDetailsTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: WorkflowDetailsTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -825,15 +825,15 @@
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileTypeDef = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_user)
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/literals.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/literals.pyi` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/paginator.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,166 +89,163 @@
 class ListAccessesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listaccessespaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listaccessespaginator)
         """
 
 
 class ListAgreementsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listagreementspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAgreementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listagreementspaginator)
         """
 
 
 class ListCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listcertificatespaginator)
         """
 
 
 class ListConnectorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listconnectorspaginator)
         """
 
 
 class ListExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listexecutionspaginator)
         """
 
 
 class ListProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ProfileType: ProfileTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProfileType: ProfileTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listprofilespaginator)
         """
 
 
 class ListSecurityPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listsecuritypoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listsecuritypoliciespaginator)
         """
 
 
 class ListServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listserverspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listserverspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListUsersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listuserspaginator)
         """
 
 
 class ListWorkflowsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listworkflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/paginator.pyi` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -86,156 +86,153 @@
 class ListAccessesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listaccessespaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listaccessespaginator)
         """
 
 class ListAgreementsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listagreementspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAgreementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAgreements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listagreementspaginator)
         """
 
 class ListCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listcertificatespaginator)
         """
 
 class ListConnectorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListConnectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listconnectorspaginator)
         """
 
 class ListExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listexecutionspaginator)
         """
 
 class ListProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ProfileType: ProfileTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ProfileType: ProfileTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listprofilespaginator)
         """
 
 class ListSecurityPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listsecuritypoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecurityPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listsecuritypoliciespaginator)
         """
 
 class ListServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listserverspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listserverspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, Arn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Arn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listtagsforresourcepaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, ServerId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listuserspaginator)
         """
 
 class ListWorkflowsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listworkflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/type_defs.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_transfer.type_defs import As2ConnectorConfigTypeDef
 
-    data: As2ConnectorConfigTypeDef = {...}
+    data: As2ConnectorConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -52,25 +52,19 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
-    "CreateAccessResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateAgreementResponseTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateProfileResponseTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
-    "CreateServerResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "CreateWorkflowResponseTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
     "DeleteHostKeyRequestRequestTypeDef",
     "DeleteProfileRequestRequestTypeDef",
@@ -88,142 +82,160 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
+    "PosixProfileOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "EndpointDetailsOutputTypeDef",
+    "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
     "EfsFileLocationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
-    "ImportCertificateResponseTypeDef",
-    "ImportHostKeyResponseTypeDef",
+    "TimestampTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
-    "ImportSshPublicKeyResponseTypeDef",
     "S3InputFileLocationTypeDef",
-    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
-    "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListedCertificateTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListedConnectorTypeDef",
-    "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListExecutionsRequestRequestTypeDef",
     "ListHostKeysRequestRequestTypeDef",
     "ListedHostKeyTypeDef",
-    "ListProfilesRequestListProfilesPaginateTypeDef",
     "ListProfilesRequestRequestTypeDef",
     "ListedProfileTypeDef",
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
-    "ListSecurityPoliciesResponseTypeDef",
-    "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "ListedServerTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
-    "StartFileTransferResponseTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
-    "TestIdentityProviderResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAccessResponseTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
-    "UpdateAgreementResponseTypeDef",
-    "UpdateCertificateRequestRequestTypeDef",
-    "UpdateCertificateResponseTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
-    "UpdateHostKeyResponseTypeDef",
     "UpdateProfileRequestRequestTypeDef",
-    "UpdateProfileResponseTypeDef",
-    "UpdateServerResponseTypeDef",
-    "UpdateUserResponseTypeDef",
     "WorkflowDetailTypeDef",
     "UpdateConnectorRequestRequestTypeDef",
     "CreateAccessRequestRequestTypeDef",
-    "DescribedAccessTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "CreateAccessResponseTypeDef",
+    "CreateAgreementResponseTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "CreateServerResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ImportCertificateResponseTypeDef",
+    "ImportHostKeyResponseTypeDef",
+    "ImportSshPublicKeyResponseTypeDef",
+    "ListSecurityPoliciesResponseTypeDef",
+    "StartFileTransferResponseTypeDef",
+    "TestIdentityProviderResponseTypeDef",
+    "UpdateAccessResponseTypeDef",
+    "UpdateAgreementResponseTypeDef",
+    "UpdateCertificateResponseTypeDef",
+    "UpdateConnectorResponseTypeDef",
+    "UpdateHostKeyResponseTypeDef",
+    "UpdateProfileResponseTypeDef",
+    "UpdateServerResponseTypeDef",
+    "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
     "CreateConnectorRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribedAgreementTypeDef",
     "DescribedCertificateTypeDef",
     "DescribedConnectorTypeDef",
     "DescribedHostKeyTypeDef",
     "DescribedProfileTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
+    "DescribedAccessTypeDef",
+    "PosixProfileUnionTypeDef",
+    "EndpointDetailsUnionTypeDef",
+    "ProtocolDetailsUnionTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
+    "UpdateCertificateRequestRequestTypeDef",
     "InputFileLocationTypeDef",
+    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "ListAgreementsRequestListAgreementsPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "ListExecutionsRequestListExecutionsPaginateTypeDef",
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    "ListServersRequestListServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAccessesResponseTypeDef",
     "ListAgreementsResponseTypeDef",
     "ListCertificatesResponseTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListHostKeysResponseTypeDef",
     "ListProfilesResponseTypeDef",
     "ListServersResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
+    "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
-    "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
+    "DescribeAccessResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
-    "CreateServerRequestRequestTypeDef",
     "DescribedServerTypeDef",
+    "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
+    "WorkflowDetailsUnionTypeDef",
     "DescribedExecutionTypeDef",
+    "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
     "DescribedWorkflowTypeDef",
+    "WorkflowStepUnionTypeDef",
     "DescribeWorkflowResponseTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
@@ -261,55 +273,33 @@
 )
 
 
 class PosixProfileTypeDef(_RequiredPosixProfileTypeDef, _OptionalPosixProfileTypeDef):
     pass
 
 
-CreateAccessResponseTypeDef = TypedDict(
-    "CreateAccessResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAgreementResponseTypeDef = TypedDict(
-    "CreateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "AddressAllocationIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcEndpointId": str,
         "VpcId": str,
@@ -337,39 +327,14 @@
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": Sequence[Literal["HTTP"]],
     },
     total=False,
 )
 
-CreateServerResponseTypeDef = TypedDict(
-    "CreateServerResponseTypeDef",
-    {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
         "Target": str,
         "TimeoutSeconds": int,
         "SourceFileLocation": str,
@@ -574,23 +539,68 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
+_RequiredPosixProfileOutputTypeDef = TypedDict(
+    "_RequiredPosixProfileOutputTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+    },
+)
+_OptionalPosixProfileOutputTypeDef = TypedDict(
+    "_OptionalPosixProfileOutputTypeDef",
+    {
+        "SecondaryGids": List[int],
+    },
+    total=False,
+)
+
+
+class PosixProfileOutputTypeDef(
+    _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
+):
+    pass
+
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
     total=False,
 )
 
+EndpointDetailsOutputTypeDef = TypedDict(
+    "EndpointDetailsOutputTypeDef",
+    {
+        "AddressAllocationIds": List[str],
+        "SubnetIds": List[str],
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+ProtocolDetailsOutputTypeDef = TypedDict(
+    "ProtocolDetailsOutputTypeDef",
+    {
+        "PassiveIp": str,
+        "TlsSessionResumptionMode": TlsSessionResumptionModeType,
+        "SetStatOption": SetStatOptionType,
+        "As2Transports": List[Literal["HTTP"]],
+    },
+    total=False,
+)
+
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
@@ -601,21 +611,14 @@
     {
         "FileSystemId": str,
         "Path": str,
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
 ExecutionErrorTypeDef = TypedDict(
     "ExecutionErrorTypeDef",
     {
         "Type": ExecutionErrorTypeType,
         "Message": str,
     },
 )
@@ -627,81 +630,43 @@
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
     total=False,
 )
 
-ImportCertificateResponseTypeDef = TypedDict(
-    "ImportCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportHostKeyResponseTypeDef = TypedDict(
-    "ImportHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
 )
 
-ImportSshPublicKeyResponseTypeDef = TypedDict(
-    "ImportSshPublicKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "SshPublicKeyId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
-_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
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
 
-
-class ListAccessesRequestListAccessesPaginateTypeDef(
-    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
-    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccessesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessesRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAccessesRequestRequestTypeDef = TypedDict(
@@ -727,36 +692,14 @@
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "ExternalId": str,
     },
     total=False,
 )
 
-_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAgreementsRequestListAgreementsPaginateTypeDef(
-    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
-    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAgreementsRequestRequestTypeDef = TypedDict(
     "_RequiredListAgreementsRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAgreementsRequestRequestTypeDef = TypedDict(
@@ -785,22 +728,14 @@
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
     },
     total=False,
 )
 
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -817,22 +752,14 @@
         "InactiveDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
     },
     total=False,
 )
 
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -844,36 +771,14 @@
         "Arn": str,
         "ConnectorId": str,
         "Url": str,
     },
     total=False,
 )
 
-_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "WorkflowId": str,
-    },
-)
-_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExecutionsRequestListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExecutionsRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 _OptionalListExecutionsRequestRequestTypeDef = TypedDict(
@@ -933,23 +838,14 @@
 )
 
 
 class ListedHostKeyTypeDef(_RequiredListedHostKeyTypeDef, _OptionalListedHostKeyTypeDef):
     pass
 
 
-ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListProfilesRequestListProfilesPaginateTypeDef",
-    {
-        "ProfileType": ProfileTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProfilesRequestRequestTypeDef = TypedDict(
     "ListProfilesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ProfileType": ProfileTypeType,
     },
@@ -963,48 +859,23 @@
         "ProfileId": str,
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
     total=False,
 )
 
-ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityPoliciesRequestRequestTypeDef = TypedDict(
     "ListSecurityPoliciesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityPoliciesResponseTypeDef = TypedDict(
-    "ListSecurityPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "SecurityPolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServersRequestListServersPaginateTypeDef = TypedDict(
-    "ListServersRequestListServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1031,36 +902,14 @@
 )
 
 
 class ListedServerTypeDef(_RequiredListedServerTypeDef, _OptionalListedServerTypeDef):
     pass
 
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1076,36 +925,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1143,22 +970,14 @@
 )
 
 
 class ListedUserTypeDef(_RequiredListedUserTypeDef, _OptionalListedUserTypeDef):
     pass
 
 
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1170,35 +989,14 @@
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
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
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -1237,22 +1035,14 @@
     "StartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
         "SendFilePaths": Sequence[str],
     },
 )
 
-StartFileTransferResponseTypeDef = TypedDict(
-    "StartFileTransferResponseTypeDef",
-    {
-        "TransferId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartServerRequestRequestTypeDef = TypedDict(
     "StartServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
@@ -1284,42 +1074,22 @@
 class TestIdentityProviderRequestRequestTypeDef(
     _RequiredTestIdentityProviderRequestRequestTypeDef,
     _OptionalTestIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-TestIdentityProviderResponseTypeDef = TypedDict(
-    "TestIdentityProviderResponseTypeDef",
-    {
-        "Response": str,
-        "StatusCode": int,
-        "Message": str,
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAccessResponseTypeDef = TypedDict(
-    "UpdateAccessResponseTypeDef",
-    {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAgreementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAgreementRequestRequestTypeDef",
     {
         "AgreementId": str,
         "ServerId": str,
     },
 )
@@ -1339,79 +1109,23 @@
 
 class UpdateAgreementRequestRequestTypeDef(
     _RequiredUpdateAgreementRequestRequestTypeDef, _OptionalUpdateAgreementRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAgreementResponseTypeDef = TypedDict(
-    "UpdateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCertificateRequestRequestTypeDef",
-    {
-        "CertificateId": str,
-    },
-)
-_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCertificateRequestRequestTypeDef",
-    {
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateCertificateRequestRequestTypeDef(
-    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
-):
-    pass
-
-
-UpdateCertificateResponseTypeDef = TypedDict(
-    "UpdateCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateHostKeyRequestRequestTypeDef = TypedDict(
     "UpdateHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyId": str,
         "Description": str,
     },
 )
 
-UpdateHostKeyResponseTypeDef = TypedDict(
-    "UpdateHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
     },
 )
 _OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
@@ -1425,39 +1139,14 @@
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
 
-UpdateProfileResponseTypeDef = TypedDict(
-    "UpdateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateServerResponseTypeDef = TypedDict(
-    "UpdateServerResponseTypeDef",
-    {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateUserResponseTypeDef = TypedDict(
-    "UpdateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowDetailTypeDef = TypedDict(
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
@@ -1509,28 +1198,14 @@
 
 class CreateAccessRequestRequestTypeDef(
     _RequiredCreateAccessRequestRequestTypeDef, _OptionalCreateAccessRequestRequestTypeDef
 ):
     pass
 
 
-DescribedAccessTypeDef = TypedDict(
-    "DescribedAccessTypeDef",
-    {
-        "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
-        "Role": str,
-        "ExternalId": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessRequestRequestTypeDef",
     {
         "ServerId": str,
         "ExternalId": str,
     },
 )
@@ -1577,14 +1252,201 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
+CreateAccessResponseTypeDef = TypedDict(
+    "CreateAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAgreementResponseTypeDef = TypedDict(
+    "CreateAgreementResponseTypeDef",
+    {
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateServerResponseTypeDef = TypedDict(
+    "CreateServerResponseTypeDef",
+    {
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
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
+ImportCertificateResponseTypeDef = TypedDict(
+    "ImportCertificateResponseTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportHostKeyResponseTypeDef = TypedDict(
+    "ImportHostKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSshPublicKeyResponseTypeDef = TypedDict(
+    "ImportSshPublicKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "SshPublicKeyId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSecurityPoliciesResponseTypeDef = TypedDict(
+    "ListSecurityPoliciesResponseTypeDef",
+    {
+        "NextToken": str,
+        "SecurityPolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFileTransferResponseTypeDef = TypedDict(
+    "StartFileTransferResponseTypeDef",
+    {
+        "TransferId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestIdentityProviderResponseTypeDef = TypedDict(
+    "TestIdentityProviderResponseTypeDef",
+    {
+        "Response": str,
+        "StatusCode": int,
+        "Message": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccessResponseTypeDef = TypedDict(
+    "UpdateAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAgreementResponseTypeDef = TypedDict(
+    "UpdateAgreementResponseTypeDef",
+    {
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCertificateResponseTypeDef = TypedDict(
+    "UpdateCertificateResponseTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateHostKeyResponseTypeDef = TypedDict(
+    "UpdateHostKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProfileResponseTypeDef = TypedDict(
+    "UpdateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServerResponseTypeDef = TypedDict(
+    "UpdateServerResponseTypeDef",
+    {
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserResponseTypeDef = TypedDict(
+    "UpdateUserResponseTypeDef",
+    {
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAgreementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAgreementRequestRequestTypeDef",
     {
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "BaseDirectory": str,
@@ -1815,41 +1677,14 @@
 )
 
 
 class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
     pass
 
 
-_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateRequestRequestTypeDef",
-    {
-        "Usage": CertificateUsageTypeType,
-        "Certificate": str,
-    },
-)
-_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": str,
-        "PrivateKey": str,
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredImportHostKeyRequestRequestTypeDef = TypedDict(
     "_RequiredImportHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyBody": str,
     },
 )
@@ -1871,15 +1706,15 @@
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Arn": str,
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
@@ -1887,15 +1722,15 @@
     },
 )
 
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeServerRequestServerOfflineWaitTypeDef = TypedDict(
     "_RequiredDescribeServerRequestServerOfflineWaitTypeDef",
     {
         "ServerId": str,
@@ -1935,28 +1770,45 @@
 class DescribeServerRequestServerOnlineWaitTypeDef(
     _RequiredDescribeServerRequestServerOnlineWaitTypeDef,
     _OptionalDescribeServerRequestServerOnlineWaitTypeDef,
 ):
     pass
 
 
+DescribedAccessTypeDef = TypedDict(
+    "DescribedAccessTypeDef",
+    {
+        "HomeDirectory": str,
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "Policy": str,
+        "PosixProfile": PosixProfileOutputTypeDef,
+        "Role": str,
+        "ExternalId": str,
+    },
+    total=False,
+)
+
+PosixProfileUnionTypeDef = Union[PosixProfileTypeDef, PosixProfileOutputTypeDef]
+EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
+ProtocolDetailsUnionTypeDef = Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef]
 _RequiredDescribedUserTypeDef = TypedDict(
     "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
     "_OptionalDescribedUserTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
         "Tags": List[TagTypeDef],
         "UserName": str,
     },
     total=False,
 )
@@ -1981,105 +1833,324 @@
     {
         "S3FileLocation": S3FileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateRequestRequestTypeDef",
+    {
+        "Usage": CertificateUsageTypeType,
+        "Certificate": str,
+    },
+)
+_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": str,
+        "PrivateKey": str,
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCertificateRequestRequestTypeDef",
+    {
+        "CertificateId": str,
+    },
+)
+_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCertificateRequestRequestTypeDef",
+    {
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateCertificateRequestRequestTypeDef(
+    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
+):
+    pass
+
+
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccessesRequestListAccessesPaginateTypeDef(
+    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
+    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAgreementsRequestListAgreementsPaginateTypeDef(
+    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
+    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
+):
+    pass
+
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "WorkflowId": str,
+    },
+)
+_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExecutionsRequestListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
+):
+    pass
+
+
+ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    {
+        "ProfileType": ProfileTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServersRequestListServersPaginateTypeDef = TypedDict(
+    "ListServersRequestListServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccessesResponseTypeDef = TypedDict(
     "ListAccessesResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Accesses": List[ListedAccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAgreementsResponseTypeDef = TypedDict(
     "ListAgreementsResponseTypeDef",
     {
         "NextToken": str,
         "Agreements": List[ListedAgreementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "NextToken": str,
         "Certificates": List[ListedCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "NextToken": str,
         "Connectors": List[ListedConnectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostKeysResponseTypeDef = TypedDict(
     "ListHostKeysResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "HostKeys": List[ListedHostKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "NextToken": str,
         "Profiles": List[ListedProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "NextToken": str,
         "Servers": List[ListedServerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Users": List[ListedUserTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "NextToken": str,
         "Workflows": List[ListedWorkflowTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagStepDetailsOutputTypeDef = TypedDict(
+    "TagStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Tags": List[S3TagTypeDef],
+        "SourceFileLocation": str,
     },
+    total=False,
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
         "Tags": Sequence[S3TagTypeDef],
@@ -2091,78 +2162,87 @@
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
-WorkflowDetailsTypeDef = TypedDict(
-    "WorkflowDetailsTypeDef",
+WorkflowDetailsOutputTypeDef = TypedDict(
+    "WorkflowDetailsOutputTypeDef",
     {
-        "OnUpload": Sequence[WorkflowDetailTypeDef],
-        "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
+        "OnUpload": List[WorkflowDetailTypeDef],
+        "OnPartialUpload": List[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
-DescribeAccessResponseTypeDef = TypedDict(
-    "DescribeAccessResponseTypeDef",
+WorkflowDetailsTypeDef = TypedDict(
+    "WorkflowDetailsTypeDef",
     {
-        "ServerId": str,
-        "Access": DescribedAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OnUpload": Sequence[WorkflowDetailTypeDef],
+        "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
+    total=False,
 )
 
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "Certificate": DescribedCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "Connector": DescribedConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHostKeyResponseTypeDef = TypedDict(
     "DescribeHostKeyResponseTypeDef",
     {
         "HostKey": DescribedHostKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfileResponseTypeDef = TypedDict(
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccessResponseTypeDef = TypedDict(
+    "DescribeAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "Access": DescribedAccessTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "ServerId": str,
         "User": DescribedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecutionResultsTypeDef = TypedDict(
     "ExecutionResultsTypeDef",
     {
         "Steps": List[ExecutionStepResultTypeDef],
@@ -2213,74 +2293,74 @@
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
     total=False,
 )
 
-CreateServerRequestRequestTypeDef = TypedDict(
-    "CreateServerRequestRequestTypeDef",
-    {
-        "Certificate": str,
-        "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
-        "EndpointType": EndpointTypeType,
-        "HostKey": str,
-        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
-        "IdentityProviderType": IdentityProviderTypeType,
-        "LoggingRole": str,
-        "PostAuthenticationLoginBanner": str,
-        "PreAuthenticationLoginBanner": str,
-        "Protocols": Sequence[ProtocolType],
-        "ProtocolDetails": ProtocolDetailsTypeDef,
-        "SecurityPolicyName": str,
-        "Tags": Sequence[TagTypeDef],
-        "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredDescribedServerTypeDef = TypedDict(
     "_RequiredDescribedServerTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedServerTypeDef = TypedDict(
     "_OptionalDescribedServerTypeDef",
     {
         "Certificate": str,
-        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
         "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
         "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
         "ServerId": str,
         "State": StateType,
         "Tags": List[TagTypeDef],
         "UserCount": int,
-        "WorkflowDetails": WorkflowDetailsTypeDef,
+        "WorkflowDetails": WorkflowDetailsOutputTypeDef,
         "StructuredLogDestinations": List[str],
     },
     total=False,
 )
 
 
 class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
     pass
 
 
+CreateServerRequestRequestTypeDef = TypedDict(
+    "CreateServerRequestRequestTypeDef",
+    {
+        "Certificate": str,
+        "Domain": DomainType,
+        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointType": EndpointTypeType,
+        "HostKey": str,
+        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
+        "IdentityProviderType": IdentityProviderTypeType,
+        "LoggingRole": str,
+        "PostAuthenticationLoginBanner": str,
+        "PreAuthenticationLoginBanner": str,
+        "Protocols": Sequence[ProtocolType],
+        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "SecurityPolicyName": str,
+        "Tags": Sequence[TagTypeDef],
+        "WorkflowDetails": WorkflowDetailsTypeDef,
+        "StructuredLogDestinations": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -2306,29 +2386,43 @@
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
 
+WorkflowDetailsUnionTypeDef = Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef]
 DescribedExecutionTypeDef = TypedDict(
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
     total=False,
 )
 
+WorkflowStepOutputTypeDef = TypedDict(
+    "WorkflowStepOutputTypeDef",
+    {
+        "Type": WorkflowStepTypeType,
+        "CopyStepDetails": CopyStepDetailsTypeDef,
+        "CustomStepDetails": CustomStepDetailsTypeDef,
+        "DeleteStepDetails": DeleteStepDetailsTypeDef,
+        "TagStepDetails": TagStepDetailsOutputTypeDef,
+        "DecryptStepDetails": DecryptStepDetailsTypeDef,
+    },
+    total=False,
+)
+
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
         "CustomStepDetails": CustomStepDetailsTypeDef,
         "DeleteStepDetails": DeleteStepDetailsTypeDef,
@@ -2340,83 +2434,83 @@
 
 ListExecutionsResponseTypeDef = TypedDict(
     "ListExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "WorkflowId": str,
         "Executions": List[ListedExecutionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServerResponseTypeDef = TypedDict(
     "DescribeServerResponseTypeDef",
     {
         "Server": DescribedServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExecutionResponseTypeDef = TypedDict(
     "DescribeExecutionResponseTypeDef",
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowRequestRequestTypeDef",
-    {
-        "Steps": Sequence[WorkflowStepTypeDef],
-    },
-)
-_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OnExceptionSteps": Sequence[WorkflowStepTypeDef],
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateWorkflowRequestRequestTypeDef(
-    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredDescribedWorkflowTypeDef = TypedDict(
     "_RequiredDescribedWorkflowTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedWorkflowTypeDef = TypedDict(
     "_OptionalDescribedWorkflowTypeDef",
     {
         "Description": str,
-        "Steps": List[WorkflowStepTypeDef],
-        "OnExceptionSteps": List[WorkflowStepTypeDef],
+        "Steps": List[WorkflowStepOutputTypeDef],
+        "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
         "WorkflowId": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
 
+WorkflowStepUnionTypeDef = Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]
 DescribeWorkflowResponseTypeDef = TypedDict(
     "DescribeWorkflowResponseTypeDef",
     {
         "Workflow": DescribedWorkflowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowRequestRequestTypeDef",
+    {
+        "Steps": Sequence[WorkflowStepUnionTypeDef],
+    },
+)
+_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OnExceptionSteps": Sequence[WorkflowStepUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateWorkflowRequestRequestTypeDef(
+    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/type_defs.pyi` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_transfer.type_defs import As2ConnectorConfigTypeDef
 
-    data: As2ConnectorConfigTypeDef = {...}
+    data: As2ConnectorConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -51,25 +51,19 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
-    "CreateAccessResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateAgreementResponseTypeDef",
-    "CreateConnectorResponseTypeDef",
-    "CreateProfileResponseTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
-    "CreateServerResponseTypeDef",
-    "CreateUserResponseTypeDef",
-    "CreateWorkflowResponseTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteConnectorRequestRequestTypeDef",
     "DeleteHostKeyRequestRequestTypeDef",
     "DeleteProfileRequestRequestTypeDef",
@@ -87,142 +81,160 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
+    "PosixProfileOutputTypeDef",
     "LoggingConfigurationTypeDef",
+    "EndpointDetailsOutputTypeDef",
+    "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
     "EfsFileLocationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
-    "ImportCertificateResponseTypeDef",
-    "ImportHostKeyResponseTypeDef",
+    "TimestampTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
-    "ImportSshPublicKeyResponseTypeDef",
     "S3InputFileLocationTypeDef",
-    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
-    "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListedCertificateTypeDef",
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListConnectorsRequestRequestTypeDef",
     "ListedConnectorTypeDef",
-    "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListExecutionsRequestRequestTypeDef",
     "ListHostKeysRequestRequestTypeDef",
     "ListedHostKeyTypeDef",
-    "ListProfilesRequestListProfilesPaginateTypeDef",
     "ListProfilesRequestRequestTypeDef",
     "ListedProfileTypeDef",
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
-    "ListSecurityPoliciesResponseTypeDef",
-    "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "ListedServerTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
-    "StartFileTransferResponseTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
-    "TestIdentityProviderResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAccessResponseTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
-    "UpdateAgreementResponseTypeDef",
-    "UpdateCertificateRequestRequestTypeDef",
-    "UpdateCertificateResponseTypeDef",
-    "UpdateConnectorResponseTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
-    "UpdateHostKeyResponseTypeDef",
     "UpdateProfileRequestRequestTypeDef",
-    "UpdateProfileResponseTypeDef",
-    "UpdateServerResponseTypeDef",
-    "UpdateUserResponseTypeDef",
     "WorkflowDetailTypeDef",
     "UpdateConnectorRequestRequestTypeDef",
     "CreateAccessRequestRequestTypeDef",
-    "DescribedAccessTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "CreateAccessResponseTypeDef",
+    "CreateAgreementResponseTypeDef",
+    "CreateConnectorResponseTypeDef",
+    "CreateProfileResponseTypeDef",
+    "CreateServerResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ImportCertificateResponseTypeDef",
+    "ImportHostKeyResponseTypeDef",
+    "ImportSshPublicKeyResponseTypeDef",
+    "ListSecurityPoliciesResponseTypeDef",
+    "StartFileTransferResponseTypeDef",
+    "TestIdentityProviderResponseTypeDef",
+    "UpdateAccessResponseTypeDef",
+    "UpdateAgreementResponseTypeDef",
+    "UpdateCertificateResponseTypeDef",
+    "UpdateConnectorResponseTypeDef",
+    "UpdateHostKeyResponseTypeDef",
+    "UpdateProfileResponseTypeDef",
+    "UpdateServerResponseTypeDef",
+    "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
     "CreateConnectorRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribedAgreementTypeDef",
     "DescribedCertificateTypeDef",
     "DescribedConnectorTypeDef",
     "DescribedHostKeyTypeDef",
     "DescribedProfileTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
+    "DescribedAccessTypeDef",
+    "PosixProfileUnionTypeDef",
+    "EndpointDetailsUnionTypeDef",
+    "ProtocolDetailsUnionTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
+    "UpdateCertificateRequestRequestTypeDef",
     "InputFileLocationTypeDef",
+    "ListAccessesRequestListAccessesPaginateTypeDef",
+    "ListAgreementsRequestListAgreementsPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    "ListExecutionsRequestListExecutionsPaginateTypeDef",
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    "ListServersRequestListServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAccessesResponseTypeDef",
     "ListAgreementsResponseTypeDef",
     "ListCertificatesResponseTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListHostKeysResponseTypeDef",
     "ListProfilesResponseTypeDef",
     "ListServersResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
+    "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
-    "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "DescribeConnectorResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
+    "DescribeAccessResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
-    "CreateServerRequestRequestTypeDef",
     "DescribedServerTypeDef",
+    "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
+    "WorkflowDetailsUnionTypeDef",
     "DescribedExecutionTypeDef",
+    "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
     "DescribedWorkflowTypeDef",
+    "WorkflowStepUnionTypeDef",
     "DescribeWorkflowResponseTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
@@ -258,55 +270,33 @@
     },
     total=False,
 )
 
 class PosixProfileTypeDef(_RequiredPosixProfileTypeDef, _OptionalPosixProfileTypeDef):
     pass
 
-CreateAccessResponseTypeDef = TypedDict(
-    "CreateAccessResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAgreementResponseTypeDef = TypedDict(
-    "CreateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateConnectorResponseTypeDef = TypedDict(
-    "CreateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "AddressAllocationIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcEndpointId": str,
         "VpcId": str,
@@ -334,39 +324,14 @@
         "TlsSessionResumptionMode": TlsSessionResumptionModeType,
         "SetStatOption": SetStatOptionType,
         "As2Transports": Sequence[Literal["HTTP"]],
     },
     total=False,
 )
 
-CreateServerResponseTypeDef = TypedDict(
-    "CreateServerResponseTypeDef",
-    {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomStepDetailsTypeDef = TypedDict(
     "CustomStepDetailsTypeDef",
     {
         "Name": str,
         "Target": str,
         "TimeoutSeconds": int,
         "SourceFileLocation": str,
@@ -569,23 +534,66 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
+_RequiredPosixProfileOutputTypeDef = TypedDict(
+    "_RequiredPosixProfileOutputTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+    },
+)
+_OptionalPosixProfileOutputTypeDef = TypedDict(
+    "_OptionalPosixProfileOutputTypeDef",
+    {
+        "SecondaryGids": List[int],
+    },
+    total=False,
+)
+
+class PosixProfileOutputTypeDef(
+    _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
+):
+    pass
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
     total=False,
 )
 
+EndpointDetailsOutputTypeDef = TypedDict(
+    "EndpointDetailsOutputTypeDef",
+    {
+        "AddressAllocationIds": List[str],
+        "SubnetIds": List[str],
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+ProtocolDetailsOutputTypeDef = TypedDict(
+    "ProtocolDetailsOutputTypeDef",
+    {
+        "PassiveIp": str,
+        "TlsSessionResumptionMode": TlsSessionResumptionModeType,
+        "SetStatOption": SetStatOptionType,
+        "As2Transports": List[Literal["HTTP"]],
+    },
+    total=False,
+)
+
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
@@ -596,21 +604,14 @@
     {
         "FileSystemId": str,
         "Path": str,
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
 ExecutionErrorTypeDef = TypedDict(
     "ExecutionErrorTypeDef",
     {
         "Type": ExecutionErrorTypeType,
         "Message": str,
     },
 )
@@ -622,79 +623,43 @@
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
     total=False,
 )
 
-ImportCertificateResponseTypeDef = TypedDict(
-    "ImportCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportHostKeyResponseTypeDef = TypedDict(
-    "ImportHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
 )
 
-ImportSshPublicKeyResponseTypeDef = TypedDict(
-    "ImportSshPublicKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "SshPublicKeyId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3InputFileLocationTypeDef = TypedDict(
     "S3InputFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
-_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
-    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
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
 
-class ListAccessesRequestListAccessesPaginateTypeDef(
-    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
-    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccessesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessesRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAccessesRequestRequestTypeDef = TypedDict(
@@ -718,34 +683,14 @@
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Role": str,
         "ExternalId": str,
     },
     total=False,
 )
 
-_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
-    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAgreementsRequestListAgreementsPaginateTypeDef(
-    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
-    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAgreementsRequestRequestTypeDef = TypedDict(
     "_RequiredListAgreementsRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListAgreementsRequestRequestTypeDef = TypedDict(
@@ -772,22 +717,14 @@
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
     },
     total=False,
 )
 
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -804,22 +741,14 @@
         "InactiveDate": datetime,
         "Type": CertificateTypeType,
         "Description": str,
     },
     total=False,
 )
 
-ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
-    "ListConnectorsRequestListConnectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConnectorsRequestRequestTypeDef = TypedDict(
     "ListConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -831,34 +760,14 @@
         "Arn": str,
         "ConnectorId": str,
         "Url": str,
     },
     total=False,
 )
 
-_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "WorkflowId": str,
-    },
-)
-_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExecutionsRequestListExecutionsPaginateTypeDef(
-    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
-    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExecutionsRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 _OptionalListExecutionsRequestRequestTypeDef = TypedDict(
@@ -912,23 +821,14 @@
     },
     total=False,
 )
 
 class ListedHostKeyTypeDef(_RequiredListedHostKeyTypeDef, _OptionalListedHostKeyTypeDef):
     pass
 
-ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListProfilesRequestListProfilesPaginateTypeDef",
-    {
-        "ProfileType": ProfileTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProfilesRequestRequestTypeDef = TypedDict(
     "ListProfilesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ProfileType": ProfileTypeType,
     },
@@ -942,48 +842,23 @@
         "ProfileId": str,
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
     total=False,
 )
 
-ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
-    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityPoliciesRequestRequestTypeDef = TypedDict(
     "ListSecurityPoliciesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListSecurityPoliciesResponseTypeDef = TypedDict(
-    "ListSecurityPoliciesResponseTypeDef",
-    {
-        "NextToken": str,
-        "SecurityPolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListServersRequestListServersPaginateTypeDef = TypedDict(
-    "ListServersRequestListServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1008,34 +883,14 @@
     },
     total=False,
 )
 
 class ListedServerTypeDef(_RequiredListedServerTypeDef, _OptionalListedServerTypeDef):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1049,34 +904,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "ServerId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1110,22 +945,14 @@
     },
     total=False,
 )
 
 class ListedUserTypeDef(_RequiredListedUserTypeDef, _OptionalListedUserTypeDef):
     pass
 
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1137,35 +964,14 @@
         "WorkflowId": str,
         "Description": str,
         "Arn": str,
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
 S3TagTypeDef = TypedDict(
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -1202,22 +1008,14 @@
     "StartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
         "SendFilePaths": Sequence[str],
     },
 )
 
-StartFileTransferResponseTypeDef = TypedDict(
-    "StartFileTransferResponseTypeDef",
-    {
-        "TransferId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartServerRequestRequestTypeDef = TypedDict(
     "StartServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
@@ -1247,42 +1045,22 @@
 
 class TestIdentityProviderRequestRequestTypeDef(
     _RequiredTestIdentityProviderRequestRequestTypeDef,
     _OptionalTestIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-TestIdentityProviderResponseTypeDef = TypedDict(
-    "TestIdentityProviderResponseTypeDef",
-    {
-        "Response": str,
-        "StatusCode": int,
-        "Message": str,
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAccessResponseTypeDef = TypedDict(
-    "UpdateAccessResponseTypeDef",
-    {
-        "ServerId": str,
-        "ExternalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAgreementRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAgreementRequestRequestTypeDef",
     {
         "AgreementId": str,
         "ServerId": str,
     },
 )
@@ -1300,77 +1078,23 @@
 )
 
 class UpdateAgreementRequestRequestTypeDef(
     _RequiredUpdateAgreementRequestRequestTypeDef, _OptionalUpdateAgreementRequestRequestTypeDef
 ):
     pass
 
-UpdateAgreementResponseTypeDef = TypedDict(
-    "UpdateAgreementResponseTypeDef",
-    {
-        "AgreementId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCertificateRequestRequestTypeDef",
-    {
-        "CertificateId": str,
-    },
-)
-_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCertificateRequestRequestTypeDef",
-    {
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateCertificateRequestRequestTypeDef(
-    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
-):
-    pass
-
-UpdateCertificateResponseTypeDef = TypedDict(
-    "UpdateCertificateResponseTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateConnectorResponseTypeDef = TypedDict(
-    "UpdateConnectorResponseTypeDef",
-    {
-        "ConnectorId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateHostKeyRequestRequestTypeDef = TypedDict(
     "UpdateHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyId": str,
         "Description": str,
     },
 )
 
-UpdateHostKeyResponseTypeDef = TypedDict(
-    "UpdateHostKeyResponseTypeDef",
-    {
-        "ServerId": str,
-        "HostKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
     },
 )
 _OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
@@ -1382,39 +1106,14 @@
 )
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
-UpdateProfileResponseTypeDef = TypedDict(
-    "UpdateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateServerResponseTypeDef = TypedDict(
-    "UpdateServerResponseTypeDef",
-    {
-        "ServerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateUserResponseTypeDef = TypedDict(
-    "UpdateUserResponseTypeDef",
-    {
-        "ServerId": str,
-        "UserName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowDetailTypeDef = TypedDict(
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
@@ -1462,28 +1161,14 @@
 )
 
 class CreateAccessRequestRequestTypeDef(
     _RequiredCreateAccessRequestRequestTypeDef, _OptionalCreateAccessRequestRequestTypeDef
 ):
     pass
 
-DescribedAccessTypeDef = TypedDict(
-    "DescribedAccessTypeDef",
-    {
-        "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
-        "Role": str,
-        "ExternalId": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessRequestRequestTypeDef",
     {
         "ServerId": str,
         "ExternalId": str,
     },
 )
@@ -1526,14 +1211,201 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+CreateAccessResponseTypeDef = TypedDict(
+    "CreateAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAgreementResponseTypeDef = TypedDict(
+    "CreateAgreementResponseTypeDef",
+    {
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConnectorResponseTypeDef = TypedDict(
+    "CreateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateServerResponseTypeDef = TypedDict(
+    "CreateServerResponseTypeDef",
+    {
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
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
+ImportCertificateResponseTypeDef = TypedDict(
+    "ImportCertificateResponseTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportHostKeyResponseTypeDef = TypedDict(
+    "ImportHostKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSshPublicKeyResponseTypeDef = TypedDict(
+    "ImportSshPublicKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "SshPublicKeyId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSecurityPoliciesResponseTypeDef = TypedDict(
+    "ListSecurityPoliciesResponseTypeDef",
+    {
+        "NextToken": str,
+        "SecurityPolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFileTransferResponseTypeDef = TypedDict(
+    "StartFileTransferResponseTypeDef",
+    {
+        "TransferId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestIdentityProviderResponseTypeDef = TypedDict(
+    "TestIdentityProviderResponseTypeDef",
+    {
+        "Response": str,
+        "StatusCode": int,
+        "Message": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccessResponseTypeDef = TypedDict(
+    "UpdateAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "ExternalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAgreementResponseTypeDef = TypedDict(
+    "UpdateAgreementResponseTypeDef",
+    {
+        "AgreementId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCertificateResponseTypeDef = TypedDict(
+    "UpdateCertificateResponseTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateConnectorResponseTypeDef = TypedDict(
+    "UpdateConnectorResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateHostKeyResponseTypeDef = TypedDict(
+    "UpdateHostKeyResponseTypeDef",
+    {
+        "ServerId": str,
+        "HostKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProfileResponseTypeDef = TypedDict(
+    "UpdateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServerResponseTypeDef = TypedDict(
+    "UpdateServerResponseTypeDef",
+    {
+        "ServerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserResponseTypeDef = TypedDict(
+    "UpdateUserResponseTypeDef",
+    {
+        "ServerId": str,
+        "UserName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAgreementRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAgreementRequestRequestTypeDef",
     {
         "ServerId": str,
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "BaseDirectory": str,
@@ -1746,39 +1618,14 @@
     },
     total=False,
 )
 
 class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
     pass
 
-_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateRequestRequestTypeDef",
-    {
-        "Usage": CertificateUsageTypeType,
-        "Certificate": str,
-    },
-)
-_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": str,
-        "PrivateKey": str,
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class ImportCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
-):
-    pass
-
 _RequiredImportHostKeyRequestRequestTypeDef = TypedDict(
     "_RequiredImportHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyBody": str,
     },
 )
@@ -1798,15 +1645,15 @@
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Arn": str,
         "NextToken": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
@@ -1814,15 +1661,15 @@
     },
 )
 
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeServerRequestServerOfflineWaitTypeDef = TypedDict(
     "_RequiredDescribeServerRequestServerOfflineWaitTypeDef",
     {
         "ServerId": str,
@@ -1858,28 +1705,45 @@
 
 class DescribeServerRequestServerOnlineWaitTypeDef(
     _RequiredDescribeServerRequestServerOnlineWaitTypeDef,
     _OptionalDescribeServerRequestServerOnlineWaitTypeDef,
 ):
     pass
 
+DescribedAccessTypeDef = TypedDict(
+    "DescribedAccessTypeDef",
+    {
+        "HomeDirectory": str,
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "Policy": str,
+        "PosixProfile": PosixProfileOutputTypeDef,
+        "Role": str,
+        "ExternalId": str,
+    },
+    total=False,
+)
+
+PosixProfileUnionTypeDef = Union[PosixProfileTypeDef, PosixProfileOutputTypeDef]
+EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
+ProtocolDetailsUnionTypeDef = Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef]
 _RequiredDescribedUserTypeDef = TypedDict(
     "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
     "_OptionalDescribedUserTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
         "Tags": List[TagTypeDef],
         "UserName": str,
     },
     total=False,
 )
@@ -1902,105 +1766,310 @@
     {
         "S3FileLocation": S3FileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateRequestRequestTypeDef",
+    {
+        "Usage": CertificateUsageTypeType,
+        "Certificate": str,
+    },
+)
+_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": str,
+        "PrivateKey": str,
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class ImportCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCertificateRequestRequestTypeDef",
+    {
+        "CertificateId": str,
+    },
+)
+_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCertificateRequestRequestTypeDef",
+    {
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateCertificateRequestRequestTypeDef(
+    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
+):
+    pass
+
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_RequiredListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAccessesRequestListAccessesPaginateTypeDef = TypedDict(
+    "_OptionalListAccessesRequestListAccessesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccessesRequestListAccessesPaginateTypeDef(
+    _RequiredListAccessesRequestListAccessesPaginateTypeDef,
+    _OptionalListAccessesRequestListAccessesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_RequiredListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListAgreementsRequestListAgreementsPaginateTypeDef = TypedDict(
+    "_OptionalListAgreementsRequestListAgreementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAgreementsRequestListAgreementsPaginateTypeDef(
+    _RequiredListAgreementsRequestListAgreementsPaginateTypeDef,
+    _OptionalListAgreementsRequestListAgreementsPaginateTypeDef,
+):
+    pass
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConnectorsRequestListConnectorsPaginateTypeDef = TypedDict(
+    "ListConnectorsRequestListConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "WorkflowId": str,
+    },
+)
+_OptionalListExecutionsRequestListExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListExecutionsRequestListExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExecutionsRequestListExecutionsPaginateTypeDef(
+    _RequiredListExecutionsRequestListExecutionsPaginateTypeDef,
+    _OptionalListExecutionsRequestListExecutionsPaginateTypeDef,
+):
+    pass
+
+ListProfilesRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListProfilesRequestListProfilesPaginateTypeDef",
+    {
+        "ProfileType": ProfileTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef = TypedDict(
+    "ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServersRequestListServersPaginateTypeDef = TypedDict(
+    "ListServersRequestListServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "ServerId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccessesResponseTypeDef = TypedDict(
     "ListAccessesResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Accesses": List[ListedAccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAgreementsResponseTypeDef = TypedDict(
     "ListAgreementsResponseTypeDef",
     {
         "NextToken": str,
         "Agreements": List[ListedAgreementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "NextToken": str,
         "Certificates": List[ListedCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectorsResponseTypeDef = TypedDict(
     "ListConnectorsResponseTypeDef",
     {
         "NextToken": str,
         "Connectors": List[ListedConnectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostKeysResponseTypeDef = TypedDict(
     "ListHostKeysResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "HostKeys": List[ListedHostKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "NextToken": str,
         "Profiles": List[ListedProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "NextToken": str,
         "Servers": List[ListedServerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "NextToken": str,
         "ServerId": str,
         "Users": List[ListedUserTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "NextToken": str,
         "Workflows": List[ListedWorkflowTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagStepDetailsOutputTypeDef = TypedDict(
+    "TagStepDetailsOutputTypeDef",
+    {
+        "Name": str,
+        "Tags": List[S3TagTypeDef],
+        "SourceFileLocation": str,
     },
+    total=False,
 )
 
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
         "Tags": Sequence[S3TagTypeDef],
@@ -2012,78 +2081,87 @@
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
-WorkflowDetailsTypeDef = TypedDict(
-    "WorkflowDetailsTypeDef",
+WorkflowDetailsOutputTypeDef = TypedDict(
+    "WorkflowDetailsOutputTypeDef",
     {
-        "OnUpload": Sequence[WorkflowDetailTypeDef],
-        "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
+        "OnUpload": List[WorkflowDetailTypeDef],
+        "OnPartialUpload": List[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
-DescribeAccessResponseTypeDef = TypedDict(
-    "DescribeAccessResponseTypeDef",
+WorkflowDetailsTypeDef = TypedDict(
+    "WorkflowDetailsTypeDef",
     {
-        "ServerId": str,
-        "Access": DescribedAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OnUpload": Sequence[WorkflowDetailTypeDef],
+        "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
+    total=False,
 )
 
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "Certificate": DescribedCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectorResponseTypeDef = TypedDict(
     "DescribeConnectorResponseTypeDef",
     {
         "Connector": DescribedConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHostKeyResponseTypeDef = TypedDict(
     "DescribeHostKeyResponseTypeDef",
     {
         "HostKey": DescribedHostKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfileResponseTypeDef = TypedDict(
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccessResponseTypeDef = TypedDict(
+    "DescribeAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "Access": DescribedAccessTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "ServerId": str,
         "User": DescribedUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecutionResultsTypeDef = TypedDict(
     "ExecutionResultsTypeDef",
     {
         "Steps": List[ExecutionStepResultTypeDef],
@@ -2132,72 +2210,72 @@
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
     total=False,
 )
 
-CreateServerRequestRequestTypeDef = TypedDict(
-    "CreateServerRequestRequestTypeDef",
-    {
-        "Certificate": str,
-        "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
-        "EndpointType": EndpointTypeType,
-        "HostKey": str,
-        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
-        "IdentityProviderType": IdentityProviderTypeType,
-        "LoggingRole": str,
-        "PostAuthenticationLoginBanner": str,
-        "PreAuthenticationLoginBanner": str,
-        "Protocols": Sequence[ProtocolType],
-        "ProtocolDetails": ProtocolDetailsTypeDef,
-        "SecurityPolicyName": str,
-        "Tags": Sequence[TagTypeDef],
-        "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredDescribedServerTypeDef = TypedDict(
     "_RequiredDescribedServerTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedServerTypeDef = TypedDict(
     "_OptionalDescribedServerTypeDef",
     {
         "Certificate": str,
-        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "ProtocolDetails": ProtocolDetailsOutputTypeDef,
         "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointDetails": EndpointDetailsOutputTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
         "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
         "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
         "ServerId": str,
         "State": StateType,
         "Tags": List[TagTypeDef],
         "UserCount": int,
-        "WorkflowDetails": WorkflowDetailsTypeDef,
+        "WorkflowDetails": WorkflowDetailsOutputTypeDef,
         "StructuredLogDestinations": List[str],
     },
     total=False,
 )
 
 class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
     pass
 
+CreateServerRequestRequestTypeDef = TypedDict(
+    "CreateServerRequestRequestTypeDef",
+    {
+        "Certificate": str,
+        "Domain": DomainType,
+        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointType": EndpointTypeType,
+        "HostKey": str,
+        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
+        "IdentityProviderType": IdentityProviderTypeType,
+        "LoggingRole": str,
+        "PostAuthenticationLoginBanner": str,
+        "PreAuthenticationLoginBanner": str,
+        "Protocols": Sequence[ProtocolType],
+        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "SecurityPolicyName": str,
+        "Tags": Sequence[TagTypeDef],
+        "WorkflowDetails": WorkflowDetailsTypeDef,
+        "StructuredLogDestinations": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -2221,29 +2299,43 @@
 )
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
+WorkflowDetailsUnionTypeDef = Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef]
 DescribedExecutionTypeDef = TypedDict(
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "PosixProfile": PosixProfileTypeDef,
+        "PosixProfile": PosixProfileOutputTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
     total=False,
 )
 
+WorkflowStepOutputTypeDef = TypedDict(
+    "WorkflowStepOutputTypeDef",
+    {
+        "Type": WorkflowStepTypeType,
+        "CopyStepDetails": CopyStepDetailsTypeDef,
+        "CustomStepDetails": CustomStepDetailsTypeDef,
+        "DeleteStepDetails": DeleteStepDetailsTypeDef,
+        "TagStepDetails": TagStepDetailsOutputTypeDef,
+        "DecryptStepDetails": DecryptStepDetailsTypeDef,
+    },
+    total=False,
+)
+
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
         "CustomStepDetails": CustomStepDetailsTypeDef,
         "DeleteStepDetails": DeleteStepDetailsTypeDef,
@@ -2255,79 +2347,80 @@
 
 ListExecutionsResponseTypeDef = TypedDict(
     "ListExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "WorkflowId": str,
         "Executions": List[ListedExecutionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServerResponseTypeDef = TypedDict(
     "DescribeServerResponseTypeDef",
     {
         "Server": DescribedServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExecutionResponseTypeDef = TypedDict(
     "DescribeExecutionResponseTypeDef",
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowRequestRequestTypeDef",
-    {
-        "Steps": Sequence[WorkflowStepTypeDef],
-    },
-)
-_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OnExceptionSteps": Sequence[WorkflowStepTypeDef],
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateWorkflowRequestRequestTypeDef(
-    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
-):
-    pass
-
 _RequiredDescribedWorkflowTypeDef = TypedDict(
     "_RequiredDescribedWorkflowTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedWorkflowTypeDef = TypedDict(
     "_OptionalDescribedWorkflowTypeDef",
     {
         "Description": str,
-        "Steps": List[WorkflowStepTypeDef],
-        "OnExceptionSteps": List[WorkflowStepTypeDef],
+        "Steps": List[WorkflowStepOutputTypeDef],
+        "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
         "WorkflowId": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
+WorkflowStepUnionTypeDef = Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]
 DescribeWorkflowResponseTypeDef = TypedDict(
     "DescribeWorkflowResponseTypeDef",
     {
         "Workflow": DescribedWorkflowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowRequestRequestTypeDef",
+    {
+        "Steps": Sequence[WorkflowStepUnionTypeDef],
     },
 )
+_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OnExceptionSteps": Sequence[WorkflowStepUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateWorkflowRequestRequestTypeDef(
+    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/waiter.py` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer/waiter.pyi` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/PKG-INFO` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transfer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore transfer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore transfer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-transfer"></a>
 
 # types-aiobotocore-transfer
 
 [![PyPI - types-aiobotocore-transfer](https://img.shields.io/pypi/v/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transfer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transfer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-transfer?color=blue)](https://pypistats.org/packages/types-aiobotocore-transfer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transfer)](https://pepy.tech/project/types-aiobotocore-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Transfer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [types-aiobotocore-transfer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/).
 
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
@@ -395,37 +394,31 @@
 )
 
 
 def check_value(value: AgreementStatusTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_transfer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_transfer.type_defs import (
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
-    CreateAccessResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateAgreementResponseTypeDef,
-    CreateConnectorResponseTypeDef,
-    CreateProfileResponseTypeDef,
     EndpointDetailsTypeDef,
     IdentityProviderDetailsTypeDef,
     ProtocolDetailsTypeDef,
-    CreateServerResponseTypeDef,
-    CreateUserResponseTypeDef,
-    CreateWorkflowResponseTypeDef,
     CustomStepDetailsTypeDef,
     DeleteAccessRequestRequestTypeDef,
     DeleteAgreementRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteConnectorRequestRequestTypeDef,
     DeleteHostKeyRequestRequestTypeDef,
     DeleteProfileRequestRequestTypeDef,
@@ -443,146 +436,164 @@
     DescribeProfileRequestRequestTypeDef,
     DescribeSecurityPolicyRequestRequestTypeDef,
     DescribedSecurityPolicyTypeDef,
     DescribeServerRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeUserRequestRequestTypeDef,
     DescribeWorkflowRequestRequestTypeDef,
+    PosixProfileOutputTypeDef,
     LoggingConfigurationTypeDef,
+    EndpointDetailsOutputTypeDef,
+    ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
     EfsFileLocationTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
-    ImportCertificateResponseTypeDef,
-    ImportHostKeyResponseTypeDef,
+    TimestampTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
-    ImportSshPublicKeyResponseTypeDef,
     S3InputFileLocationTypeDef,
-    ListAccessesRequestListAccessesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
-    ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListedCertificateTypeDef,
-    ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListConnectorsRequestRequestTypeDef,
     ListedConnectorTypeDef,
-    ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListExecutionsRequestRequestTypeDef,
     ListHostKeysRequestRequestTypeDef,
     ListedHostKeyTypeDef,
-    ListProfilesRequestListProfilesPaginateTypeDef,
     ListProfilesRequestRequestTypeDef,
     ListedProfileTypeDef,
-    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
-    ListSecurityPoliciesResponseTypeDef,
-    ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     ListedServerTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListedUserTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     ListedWorkflowTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     S3TagTypeDef,
     SendWorkflowStepStateRequestRequestTypeDef,
     UserDetailsTypeDef,
     StartFileTransferRequestRequestTypeDef,
-    StartFileTransferResponseTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
-    TestIdentityProviderResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAccessResponseTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateAgreementResponseTypeDef,
-    UpdateCertificateRequestRequestTypeDef,
-    UpdateCertificateResponseTypeDef,
-    UpdateConnectorResponseTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
-    UpdateHostKeyResponseTypeDef,
     UpdateProfileRequestRequestTypeDef,
-    UpdateProfileResponseTypeDef,
-    UpdateServerResponseTypeDef,
-    UpdateUserResponseTypeDef,
     WorkflowDetailTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     CreateAccessRequestRequestTypeDef,
-    DescribedAccessTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    CreateAccessResponseTypeDef,
+    CreateAgreementResponseTypeDef,
+    CreateConnectorResponseTypeDef,
+    CreateProfileResponseTypeDef,
+    CreateServerResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ImportCertificateResponseTypeDef,
+    ImportHostKeyResponseTypeDef,
+    ImportSshPublicKeyResponseTypeDef,
+    ListSecurityPoliciesResponseTypeDef,
+    StartFileTransferResponseTypeDef,
+    TestIdentityProviderResponseTypeDef,
+    UpdateAccessResponseTypeDef,
+    UpdateAgreementResponseTypeDef,
+    UpdateCertificateResponseTypeDef,
+    UpdateConnectorResponseTypeDef,
+    UpdateHostKeyResponseTypeDef,
+    UpdateProfileResponseTypeDef,
+    UpdateServerResponseTypeDef,
+    UpdateUserResponseTypeDef,
     CreateAgreementRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribedAgreementTypeDef,
     DescribedCertificateTypeDef,
     DescribedConnectorTypeDef,
     DescribedHostKeyTypeDef,
     DescribedProfileTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
+    DescribedAccessTypeDef,
+    PosixProfileUnionTypeDef,
+    EndpointDetailsUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    ImportCertificateRequestRequestTypeDef,
+    UpdateCertificateRequestRequestTypeDef,
     InputFileLocationTypeDef,
+    ListAccessesRequestListAccessesPaginateTypeDef,
+    ListAgreementsRequestListAgreementsPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListConnectorsRequestListConnectorsPaginateTypeDef,
+    ListExecutionsRequestListExecutionsPaginateTypeDef,
+    ListProfilesRequestListProfilesPaginateTypeDef,
+    ListSecurityPoliciesRequestListSecurityPoliciesPaginateTypeDef,
+    ListServersRequestListServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
     ListCertificatesResponseTypeDef,
     ListConnectorsResponseTypeDef,
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListServersResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
+    TagStepDetailsOutputTypeDef,
     TagStepDetailsTypeDef,
     ServiceMetadataTypeDef,
+    WorkflowDetailsOutputTypeDef,
     WorkflowDetailsTypeDef,
-    DescribeAccessResponseTypeDef,
     DescribeAgreementResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     DescribeConnectorResponseTypeDef,
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
+    DescribeAccessResponseTypeDef,
     DescribeUserResponseTypeDef,
     ExecutionResultsTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
-    CreateServerRequestRequestTypeDef,
     DescribedServerTypeDef,
+    CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    WorkflowDetailsUnionTypeDef,
     DescribedExecutionTypeDef,
+    WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
     DescribedWorkflowTypeDef,
+    WorkflowStepUnionTypeDef,
     DescribeWorkflowResponseTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_value() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-transfer-2.5.2/types_aiobotocore_transfer.egg-info/SOURCES.txt` & `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-iam-2.5.2.tar.gz` & `tmp/types-aiobotocore-iam-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iam-2.5.2.tar", last modified: Sat Jul  8 01:43:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-iam-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:23 2023, max compression
```

## Comparing `types-aiobotocore-iam-2.5.2.tar` & `types-aiobotocore-iam-2.5.2.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:43.318239 types-aiobotocore-iam-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-07-08 01:43:43.318239 types-aiobotocore-iam-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    41551 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:43.318239 types-aiobotocore-iam-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:43.306239 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119024 2023-07-08 01:32:01.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   118818 2023-07-08 01:32:01.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-08 01:32:04.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-08 01:32:04.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40152 2023-07-08 01:32:03.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-07-08 01:32:03.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   154972 2023-07-08 01:32:03.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   154591 2023-07-08 01:32:02.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   146148 2023-07-08 01:32:06.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   145933 2023-07-08 01:32:05.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:00.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-08 01:32:03.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-08 01:32:03.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:43.318239 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43100 2023-07-08 01:43:43.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-08 01:43:43.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:43.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:43.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:43.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:43.000000 types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    41570 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:39:58.000000 types-aiobotocore-iam-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119024 2023-08-02 14:40:01.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118818 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    40084 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40048 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   154892 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154511 2023-08-02 14:40:01.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   146306 2023-08-02 14:40:06.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146091 2023-08-02 14:40:05.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:00.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-02 14:40:02.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.709571 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:23.000000 types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iam-2.5.2/LICENSE` & `types-aiobotocore-iam-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/PKG-INFO` & `types-aiobotocore-iam-2.5.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iam
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iam type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iam type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iam"></a>
 
 # types-aiobotocore-iam
 
 [![PyPI - types-aiobotocore-iam](https://img.shields.io/pypi/v/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iam?color=blue)](https://pypistats.org/packages/types-aiobotocore-iam)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [types-aiobotocore-iam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -637,20 +636,20 @@
 )
 
 
 def check_value(value: AccessAdvisorUsageGranularityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iam.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iam.type_defs import (
     AccessDetailTypeDef,
     AccessKeyLastUsedTypeDef,
     AccessKeyMetadataTypeDef,
     AccessKeyTypeDef,
@@ -665,15 +664,15 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
-    AttachedPermissionsBoundaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     AttachedPermissionsBoundaryTypeDef,
     AttachedPolicyTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
@@ -685,15 +684,14 @@
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     LoginProfileTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
     ServiceSpecificCredentialTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
@@ -706,15 +704,14 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
     RoleUsageTypeTypeDef,
@@ -723,141 +720,95 @@
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
     EntityInfoTypeDef,
     ErrorDetailsTypeDef,
     OrganizationsDecisionDetailTypeDef,
     PermissionsBoundaryDecisionDetailTypeDef,
-    GenerateCredentialReportResponseTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
-    GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
     PasswordPolicyTypeDef,
-    GetAccountSummaryResponseTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseTypeDef,
-    GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
     SSHPublicKeyTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseTypeDef,
     GetUserRequestRequestTypeDef,
     PolicyDetailTypeDef,
-    ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
-    ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
-    ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
-    ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
-    ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
     PolicyGroupTypeDef,
     PolicyRoleTypeDef,
     PolicyUserTypeDef,
-    ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
-    ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
-    ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
-    ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
     MFADeviceTypeDef,
-    ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
     OpenIDConnectProviderListEntryTypeDef,
     PolicyGrantingServiceAccessTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
-    ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
-    ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
-    ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
-    ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
     SAMLProviderListEntryTypeDef,
-    ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
     SSHPublicKeyMetadataTypeDef,
-    ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
-    ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
     ServerCertificateMetadataTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
     ServiceSpecificCredentialMetadataTypeDef,
-    ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
     SigningCertificateTypeDef,
-    ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PolicyDocumentStatementTypeDef,
     PositionTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
@@ -868,20 +819,17 @@
     RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef,
     RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef,
     RemoveRoleFromInstanceProfileRequestRequestTypeDef,
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
     RoleLastUsedTypeDef,
-    RoleLastUsedResponseMetadataTypeDef,
-    ServerCertificateMetadataResponseMetadataTypeDef,
     TrackedActionLastAccessedTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
@@ -904,37 +852,54 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
+    AttachedPermissionsBoundaryResponseTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GenerateCredentialReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedResponseTypeDef,
+    GetAccountSummaryResponseTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
+    GetCredentialReportResponseTypeDef,
+    GetGroupPolicyResponseTypeDef,
+    GetMFADeviceResponseTypeDef,
+    GetRolePolicyResponseTypeDef,
+    GetUserPolicyResponseTypeDef,
     ListAccessKeysResponseTypeDef,
-    CreateAccessKeyResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    RoleLastUsedResponseTypeDef,
+    ServerCertificateMetadataResponseTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     ListAttachedGroupPoliciesResponseTypeDef,
     ListAttachedRolePoliciesResponseTypeDef,
     ListAttachedUserPoliciesResponseTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
-    SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
-    SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     CreateGroupResponseTypeDef,
     ListGroupsForUserResponseTypeDef,
     ListGroupsResponseTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
     CreateOpenIDConnectProviderResponseTypeDef,
@@ -967,27 +932,57 @@
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CreateLoginProfileResponseTypeDef,
     GetLoginProfileResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ManagedPolicyDetailTypeDef,
     CreateServiceSpecificCredentialResponseTypeDef,
     ResetServiceSpecificCredentialResponseTypeDef,
     DeletionTaskFailureReasonTypeTypeDef,
     EntityDetailsTypeDef,
     GetOrganizationsAccessReportResponseTypeDef,
+    GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
+    GetGroupRequestGetGroupPaginateTypeDef,
+    ListAccessKeysRequestListAccessKeysPaginateTypeDef,
+    ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
+    ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+    ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+    ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+    ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+    ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+    ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+    ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
+    ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+    ListMFADevicesRequestListMFADevicesPaginateTypeDef,
+    ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+    ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+    ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+    ListRoleTagsRequestListRoleTagsPaginateTypeDef,
+    ListRolesRequestListRolesPaginateTypeDef,
+    ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+    ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
+    ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+    ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
+    ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
+    ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+    ListUserTagsRequestListUserTagsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
+    SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+    SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     GetAccountPasswordPolicyResponseTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
     GetSSHPublicKeyResponseTypeDef,
     UploadSSHPublicKeyResponseTypeDef,
@@ -1001,14 +996,15 @@
     ListSSHPublicKeysResponseTypeDef,
     ListServerCertificatesResponseTypeDef,
     ServerCertificateTypeDef,
     UploadServerCertificateResponseTypeDef,
     ListServiceSpecificCredentialsResponseTypeDef,
     ListSigningCertificatesResponseTypeDef,
     UploadSigningCertificateResponseTypeDef,
+    PolicyDocumentFixedTypeDef,
     StatementTypeDef,
     RoleTypeDef,
     ServiceLastAccessedTypeDef,
     CreatePolicyResponseTypeDef,
     GetPolicyResponseTypeDef,
     ListPoliciesResponseTypeDef,
     CreateUserResponseTypeDef,
@@ -1016,36 +1012,41 @@
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     VirtualMFADeviceTypeDef,
     GetServiceLinkedRoleDeletionStatusResponseTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
     ListPoliciesGrantingServiceAccessResponseTypeDef,
     GetServerCertificateResponseTypeDef,
+    PolicyVersionTypeDef,
     ResourceSpecificResultTypeDef,
     CreateRoleResponseTypeDef,
     CreateServiceLinkedRoleResponseTypeDef,
     GetRoleResponseTypeDef,
     InstanceProfileTypeDef,
     ListRolesResponseTypeDef,
     UpdateRoleDescriptionResponseTypeDef,
     GetServiceLastAccessedDetailsResponseTypeDef,
     CreateVirtualMFADeviceResponseTypeDef,
     ListVirtualMFADevicesResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ManagedPolicyDetailTypeDef,
     EvaluationResultTypeDef,
     CreateInstanceProfileResponseTypeDef,
     GetInstanceProfileResponseTypeDef,
     ListInstanceProfilesForRoleResponseTypeDef,
     ListInstanceProfilesResponseTypeDef,
     RoleDetailTypeDef,
     SimulatePolicyResponseTypeDef,
     GetAccountAuthorizationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessDetailTypeDef:
+def get_value() -> AccessDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iam-2.5.2/README.md` & `types-aiobotocore-iam-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iam"></a>
 
 # types-aiobotocore-iam
 
 [![PyPI - types-aiobotocore-iam](https://img.shields.io/pypi/v/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iam?color=blue)](https://pypistats.org/packages/types-aiobotocore-iam)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [types-aiobotocore-iam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -45,15 +45,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -604,20 +604,20 @@
 )
 
 
 def check_value(value: AccessAdvisorUsageGranularityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iam.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iam.type_defs import (
     AccessDetailTypeDef,
     AccessKeyLastUsedTypeDef,
     AccessKeyMetadataTypeDef,
     AccessKeyTypeDef,
@@ -632,15 +632,15 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
-    AttachedPermissionsBoundaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     AttachedPermissionsBoundaryTypeDef,
     AttachedPolicyTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
@@ -652,15 +652,14 @@
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     LoginProfileTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
     ServiceSpecificCredentialTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
@@ -673,15 +672,14 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
     RoleUsageTypeTypeDef,
@@ -690,141 +688,95 @@
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
     EntityInfoTypeDef,
     ErrorDetailsTypeDef,
     OrganizationsDecisionDetailTypeDef,
     PermissionsBoundaryDecisionDetailTypeDef,
-    GenerateCredentialReportResponseTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
-    GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
     PasswordPolicyTypeDef,
-    GetAccountSummaryResponseTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseTypeDef,
-    GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
     SSHPublicKeyTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseTypeDef,
     GetUserRequestRequestTypeDef,
     PolicyDetailTypeDef,
-    ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
-    ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
-    ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
-    ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
-    ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
     PolicyGroupTypeDef,
     PolicyRoleTypeDef,
     PolicyUserTypeDef,
-    ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
-    ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
-    ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
-    ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
     MFADeviceTypeDef,
-    ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
     OpenIDConnectProviderListEntryTypeDef,
     PolicyGrantingServiceAccessTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
-    ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
-    ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
-    ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
-    ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
     SAMLProviderListEntryTypeDef,
-    ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
     SSHPublicKeyMetadataTypeDef,
-    ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
-    ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
     ServerCertificateMetadataTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
     ServiceSpecificCredentialMetadataTypeDef,
-    ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
     SigningCertificateTypeDef,
-    ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PolicyDocumentStatementTypeDef,
     PositionTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
@@ -835,20 +787,17 @@
     RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef,
     RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef,
     RemoveRoleFromInstanceProfileRequestRequestTypeDef,
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
     RoleLastUsedTypeDef,
-    RoleLastUsedResponseMetadataTypeDef,
-    ServerCertificateMetadataResponseMetadataTypeDef,
     TrackedActionLastAccessedTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
@@ -871,37 +820,54 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
+    AttachedPermissionsBoundaryResponseTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GenerateCredentialReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedResponseTypeDef,
+    GetAccountSummaryResponseTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
+    GetCredentialReportResponseTypeDef,
+    GetGroupPolicyResponseTypeDef,
+    GetMFADeviceResponseTypeDef,
+    GetRolePolicyResponseTypeDef,
+    GetUserPolicyResponseTypeDef,
     ListAccessKeysResponseTypeDef,
-    CreateAccessKeyResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    RoleLastUsedResponseTypeDef,
+    ServerCertificateMetadataResponseTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     ListAttachedGroupPoliciesResponseTypeDef,
     ListAttachedRolePoliciesResponseTypeDef,
     ListAttachedUserPoliciesResponseTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
-    SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
-    SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     CreateGroupResponseTypeDef,
     ListGroupsForUserResponseTypeDef,
     ListGroupsResponseTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
     CreateOpenIDConnectProviderResponseTypeDef,
@@ -934,27 +900,57 @@
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CreateLoginProfileResponseTypeDef,
     GetLoginProfileResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ManagedPolicyDetailTypeDef,
     CreateServiceSpecificCredentialResponseTypeDef,
     ResetServiceSpecificCredentialResponseTypeDef,
     DeletionTaskFailureReasonTypeTypeDef,
     EntityDetailsTypeDef,
     GetOrganizationsAccessReportResponseTypeDef,
+    GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
+    GetGroupRequestGetGroupPaginateTypeDef,
+    ListAccessKeysRequestListAccessKeysPaginateTypeDef,
+    ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
+    ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+    ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+    ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+    ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+    ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+    ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+    ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
+    ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+    ListMFADevicesRequestListMFADevicesPaginateTypeDef,
+    ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+    ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+    ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+    ListRoleTagsRequestListRoleTagsPaginateTypeDef,
+    ListRolesRequestListRolesPaginateTypeDef,
+    ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+    ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
+    ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+    ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
+    ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
+    ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+    ListUserTagsRequestListUserTagsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
+    SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+    SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     GetAccountPasswordPolicyResponseTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
     GetSSHPublicKeyResponseTypeDef,
     UploadSSHPublicKeyResponseTypeDef,
@@ -968,14 +964,15 @@
     ListSSHPublicKeysResponseTypeDef,
     ListServerCertificatesResponseTypeDef,
     ServerCertificateTypeDef,
     UploadServerCertificateResponseTypeDef,
     ListServiceSpecificCredentialsResponseTypeDef,
     ListSigningCertificatesResponseTypeDef,
     UploadSigningCertificateResponseTypeDef,
+    PolicyDocumentFixedTypeDef,
     StatementTypeDef,
     RoleTypeDef,
     ServiceLastAccessedTypeDef,
     CreatePolicyResponseTypeDef,
     GetPolicyResponseTypeDef,
     ListPoliciesResponseTypeDef,
     CreateUserResponseTypeDef,
@@ -983,36 +980,41 @@
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     VirtualMFADeviceTypeDef,
     GetServiceLinkedRoleDeletionStatusResponseTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
     ListPoliciesGrantingServiceAccessResponseTypeDef,
     GetServerCertificateResponseTypeDef,
+    PolicyVersionTypeDef,
     ResourceSpecificResultTypeDef,
     CreateRoleResponseTypeDef,
     CreateServiceLinkedRoleResponseTypeDef,
     GetRoleResponseTypeDef,
     InstanceProfileTypeDef,
     ListRolesResponseTypeDef,
     UpdateRoleDescriptionResponseTypeDef,
     GetServiceLastAccessedDetailsResponseTypeDef,
     CreateVirtualMFADeviceResponseTypeDef,
     ListVirtualMFADevicesResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ManagedPolicyDetailTypeDef,
     EvaluationResultTypeDef,
     CreateInstanceProfileResponseTypeDef,
     GetInstanceProfileResponseTypeDef,
     ListInstanceProfilesForRoleResponseTypeDef,
     ListInstanceProfilesResponseTypeDef,
     RoleDetailTypeDef,
     SimulatePolicyResponseTypeDef,
     GetAccountAuthorizationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessDetailTypeDef:
+def get_value() -> AccessDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iam-2.5.2/setup.py` & `types-aiobotocore-iam-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iam",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore iam type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iam type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iam": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/__init__.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,17 @@
     RoleExistsWaiter,
     UserExistsWaiter,
 )
 
 Client = IAMClient
 
 
+ServiceResource = IAMServiceResource
+
+
 __all__ = (
     "Client",
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "IAMClient",
     "IAMServiceResource",
     "InstanceProfileExistsWaiter",
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/__init__.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,16 @@
     PolicyExistsWaiter,
     RoleExistsWaiter,
     UserExistsWaiter,
 )
 
 Client = IAMClient
 
+ServiceResource = IAMServiceResource
+
 __all__ = (
     "Client",
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "IAMClient",
     "IAMServiceResource",
     "InstanceProfileExistsWaiter",
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/__main__.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IAM 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IAM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
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

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/client.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/client.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/literals.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/literals.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/paginator.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,60 +189,60 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 
 class GetGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getgrouppaginator)
     """
 
     def paginate(
-        self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getgrouppaginator)
         """
 
 
 class ListAccessKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccesskeyspaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccesskeyspaginator)
         """
 
 
 class ListAccountAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccountaliasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccountaliasespaginator)
         """
 
 
@@ -253,15 +253,15 @@
     """
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 
@@ -272,15 +272,15 @@
     """
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 
@@ -291,15 +291,15 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 
@@ -312,150 +312,150 @@
     def paginate(
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntitiesForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 
 class ListGroupPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgrouppoliciespaginator)
     """
 
     def paginate(
-        self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgrouppoliciespaginator)
         """
 
 
 class ListGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupspaginator)
         """
 
 
 class ListGroupsForUserPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupsforuserpaginator)
         """
 
 
 class ListInstanceProfileTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofiletagspaginator)
     """
 
     def paginate(
-        self, *, InstanceProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceProfileName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstanceProfileTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofiletagspaginator)
         """
 
 
 class ListInstanceProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstanceProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilespaginator)
         """
 
 
 class ListInstanceProfilesForRolePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilesforrolepaginator)
     """
 
     def paginate(
-        self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstanceProfilesForRoleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilesforrolepaginator)
         """
 
 
 class ListMFADeviceTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicetagspaginator)
     """
 
     def paginate(
-        self, *, SerialNumber: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SerialNumber: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMFADeviceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicetagspaginator)
         """
 
 
 class ListMFADevicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicespaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicespaginator)
         """
 
 
 class ListOpenIDConnectProviderTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listopenidconnectprovidertagspaginator)
     """
 
     def paginate(
-        self, *, OpenIDConnectProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OpenIDConnectProviderArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listopenidconnectprovidertagspaginator)
         """
 
 
@@ -468,210 +468,210 @@
     def paginate(
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpoliciespaginator)
         """
 
 
 class ListPolicyTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicytagspaginator)
     """
 
     def paginate(
-        self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicytagspaginator)
         """
 
 
 class ListPolicyVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicyversionspaginator)
     """
 
     def paginate(
-        self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicyversionspaginator)
         """
 
 
 class ListRolePoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolepoliciespaginator)
     """
 
     def paginate(
-        self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolepoliciespaginator)
         """
 
 
 class ListRoleTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listroletagspaginator)
     """
 
     def paginate(
-        self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoleTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listroletagspaginator)
         """
 
 
 class ListRolesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolespaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolespaginator)
         """
 
 
 class ListSAMLProviderTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsamlprovidertagspaginator)
     """
 
     def paginate(
-        self, *, SAMLProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SAMLProviderArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSAMLProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsamlprovidertagspaginator)
         """
 
 
 class ListSSHPublicKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsshpublickeyspaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSSHPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsshpublickeyspaginator)
         """
 
 
 class ListServerCertificateTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatetagspaginator)
     """
 
     def paginate(
-        self, *, ServerCertificateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerCertificateName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServerCertificateTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatetagspaginator)
         """
 
 
 class ListServerCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatespaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServerCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatespaginator)
         """
 
 
 class ListSigningCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsigningcertificatespaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsigningcertificatespaginator)
         """
 
 
 class ListUserPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserpoliciespaginator)
     """
 
     def paginate(
-        self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserpoliciespaginator)
         """
 
 
 class ListUserTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listusertagspaginator)
     """
 
     def paginate(
-        self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listusertagspaginator)
         """
 
 
 class ListUsersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserspaginator)
         """
 
 
@@ -681,15 +681,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 
@@ -707,15 +707,15 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulatecustompolicypaginator)
         """
 
 
@@ -734,13 +734,13 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/paginator.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -186,57 +186,57 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 class GetGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getgrouppaginator)
     """
 
     def paginate(
-        self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#getgrouppaginator)
         """
 
 class ListAccessKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccesskeyspaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccesskeyspaginator)
         """
 
 class ListAccountAliasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccountaliasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listaccountaliasespaginator)
         """
 
 class ListAttachedGroupPoliciesPaginator(AioPaginator):
@@ -246,15 +246,15 @@
     """
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 class ListAttachedRolePoliciesPaginator(AioPaginator):
@@ -264,15 +264,15 @@
     """
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 class ListAttachedUserPoliciesPaginator(AioPaginator):
@@ -282,15 +282,15 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 class ListEntitiesForPolicyPaginator(AioPaginator):
@@ -302,141 +302,141 @@
     def paginate(
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntitiesForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 class ListGroupPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgrouppoliciespaginator)
     """
 
     def paginate(
-        self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgrouppoliciespaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupspaginator)
         """
 
 class ListGroupsForUserPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listgroupsforuserpaginator)
         """
 
 class ListInstanceProfileTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofiletagspaginator)
     """
 
     def paginate(
-        self, *, InstanceProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceProfileName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstanceProfileTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofiletagspaginator)
         """
 
 class ListInstanceProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstanceProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilespaginator)
         """
 
 class ListInstanceProfilesForRolePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilesforrolepaginator)
     """
 
     def paginate(
-        self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstanceProfilesForRoleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listinstanceprofilesforrolepaginator)
         """
 
 class ListMFADeviceTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicetagspaginator)
     """
 
     def paginate(
-        self, *, SerialNumber: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SerialNumber: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMFADeviceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicetagspaginator)
         """
 
 class ListMFADevicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicespaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listmfadevicespaginator)
         """
 
 class ListOpenIDConnectProviderTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listopenidconnectprovidertagspaginator)
     """
 
     def paginate(
-        self, *, OpenIDConnectProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OpenIDConnectProviderArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listopenidconnectprovidertagspaginator)
         """
 
 class ListPoliciesPaginator(AioPaginator):
@@ -448,197 +448,197 @@
     def paginate(
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicytagspaginator)
     """
 
     def paginate(
-        self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicytagspaginator)
         """
 
 class ListPolicyVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicyversionspaginator)
     """
 
     def paginate(
-        self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listpolicyversionspaginator)
         """
 
 class ListRolePoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolepoliciespaginator)
     """
 
     def paginate(
-        self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolepoliciespaginator)
         """
 
 class ListRoleTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listroletagspaginator)
     """
 
     def paginate(
-        self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RoleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoleTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listroletagspaginator)
         """
 
 class ListRolesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolespaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listrolespaginator)
         """
 
 class ListSAMLProviderTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsamlprovidertagspaginator)
     """
 
     def paginate(
-        self, *, SAMLProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SAMLProviderArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSAMLProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsamlprovidertagspaginator)
         """
 
 class ListSSHPublicKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsshpublickeyspaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSSHPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsshpublickeyspaginator)
         """
 
 class ListServerCertificateTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatetagspaginator)
     """
 
     def paginate(
-        self, *, ServerCertificateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerCertificateName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServerCertificateTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatetagspaginator)
         """
 
 class ListServerCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatespaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServerCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listservercertificatespaginator)
         """
 
 class ListSigningCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsigningcertificatespaginator)
     """
 
     def paginate(
-        self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSigningCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listsigningcertificatespaginator)
         """
 
 class ListUserPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserpoliciespaginator)
     """
 
     def paginate(
-        self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserpoliciespaginator)
         """
 
 class ListUserTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listusertagspaginator)
     """
 
     def paginate(
-        self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listusertagspaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PathPrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listuserspaginator)
         """
 
 class ListVirtualMFADevicesPaginator(AioPaginator):
@@ -647,15 +647,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 class SimulateCustomPolicyPaginator(AioPaginator):
@@ -672,15 +672,15 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulatecustompolicypaginator)
         """
 
 class SimulatePrincipalPolicyPaginator(AioPaginator):
@@ -698,13 +698,13 @@
         PermissionsBoundaryPolicyInputList: Sequence[str] = ...,
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/service_resource.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     PolicyUsageTypeType,
     assignmentStatusTypeType,
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
-    AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    RoleLastUsedResponseMetadataTypeDef,
+    AttachedPermissionsBoundaryResponseTypeDef,
+    RoleLastUsedResponseTypeDef,
     RoleTypeDef,
-    ServerCertificateMetadataResponseMetadataTypeDef,
+    ServerCertificateMetadataResponseTypeDef,
     TagTypeDef,
     UpdateSAMLProviderResponseTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
@@ -1588,15 +1588,15 @@
 
     path: Awaitable[str]
     user_name: Awaitable[str]
     user_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     password_last_used: Awaitable[datetime]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseMetadataTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
 
     async def get_available_subresources(self) -> Sequence[str]:
@@ -1820,15 +1820,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.VirtualMfaDevice)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#virtualmfadevice)
     """
 
     base32_string_seed: Awaitable[bytes]
     qr_code_png: Awaitable[bytes]
-    user_attribute: Awaitable[UserResponseMetadataTypeDef]
+    user_attribute: Awaitable[UserResponseTypeDef]
     enable_date: Awaitable[datetime]
     tags: Awaitable[List[TagTypeDef]]
     serial_number: str
     user: "User"
 
     async def delete(self) -> None:
         """
@@ -2254,15 +2254,15 @@
 
 class ServerCertificate(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#servercertificate)
     """
 
-    server_certificate_metadata: Awaitable[ServerCertificateMetadataResponseMetadataTypeDef]
+    server_certificate_metadata: Awaitable[ServerCertificateMetadataResponseTypeDef]
     certificate_body: Awaitable[str]
     certificate_chain: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     name: str
 
     async def delete(self) -> None:
         """
@@ -2523,17 +2523,17 @@
     role_name: Awaitable[str]
     role_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     assume_role_policy_document: Awaitable[str]
     description: Awaitable[str]
     max_session_duration: Awaitable[int]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseMetadataTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
     tags: Awaitable[List[TagTypeDef]]
-    role_last_used: Awaitable[RoleLastUsedResponseMetadataTypeDef]
+    role_last_used: Awaitable[RoleLastUsedResponseTypeDef]
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
 
     async def AssumeRolePolicy(self) -> _AssumeRolePolicy:
         """
@@ -2732,15 +2732,15 @@
 
     path: Awaitable[str]
     user_name: Awaitable[str]
     user_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     password_last_used: Awaitable[datetime]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseMetadataTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/service_resource.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     PolicyUsageTypeType,
     assignmentStatusTypeType,
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
-    AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    RoleLastUsedResponseMetadataTypeDef,
+    AttachedPermissionsBoundaryResponseTypeDef,
+    RoleLastUsedResponseTypeDef,
     RoleTypeDef,
-    ServerCertificateMetadataResponseMetadataTypeDef,
+    ServerCertificateMetadataResponseTypeDef,
     TagTypeDef,
     UpdateSAMLProviderResponseTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
@@ -1382,15 +1382,15 @@
 
     path: Awaitable[str]
     user_name: Awaitable[str]
     user_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     password_last_used: Awaitable[datetime]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseMetadataTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     user: "User"
     access_keys: CurrentUserAccessKeysCollection
     mfa_devices: CurrentUserMfaDevicesCollection
     signing_certificates: CurrentUserSigningCertificatesCollection
 
     async def get_available_subresources(self) -> Sequence[str]:
@@ -1591,15 +1591,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.VirtualMfaDevice)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#virtualmfadevice)
     """
 
     base32_string_seed: Awaitable[bytes]
     qr_code_png: Awaitable[bytes]
-    user_attribute: Awaitable[UserResponseMetadataTypeDef]
+    user_attribute: Awaitable[UserResponseTypeDef]
     enable_date: Awaitable[datetime]
     tags: Awaitable[List[TagTypeDef]]
     serial_number: str
     user: "User"
 
     async def delete(self) -> None:
         """
@@ -1980,15 +1980,15 @@
 
 class ServerCertificate(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.ServiceResource.ServerCertificate)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/service_resource/#servercertificate)
     """
 
-    server_certificate_metadata: Awaitable[ServerCertificateMetadataResponseMetadataTypeDef]
+    server_certificate_metadata: Awaitable[ServerCertificateMetadataResponseTypeDef]
     certificate_body: Awaitable[str]
     certificate_chain: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     name: str
 
     async def delete(self) -> None:
         """
@@ -2328,17 +2328,17 @@
     role_name: Awaitable[str]
     role_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     assume_role_policy_document: Awaitable[str]
     description: Awaitable[str]
     max_session_duration: Awaitable[int]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseMetadataTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
     tags: Awaitable[List[TagTypeDef]]
-    role_last_used: Awaitable[RoleLastUsedResponseMetadataTypeDef]
+    role_last_used: Awaitable[RoleLastUsedResponseTypeDef]
     name: str
     attached_policies: RoleAttachedPoliciesCollection
     instance_profiles: RoleInstanceProfilesCollection
     policies: RolePoliciesCollection
 
     async def AssumeRolePolicy(self) -> _AssumeRolePolicy:
         """
@@ -2409,15 +2409,15 @@
 
     path: Awaitable[str]
     user_name: Awaitable[str]
     user_id: Awaitable[str]
     arn: Awaitable[str]
     create_date: Awaitable[datetime]
     password_last_used: Awaitable[datetime]
-    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseMetadataTypeDef]
+    permissions_boundary: Awaitable[AttachedPermissionsBoundaryResponseTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     name: str
     access_keys: UserAccessKeysCollection
     attached_policies: UserAttachedPoliciesCollection
     groups: UserGroupsCollection
     mfa_devices: UserMfaDevicesCollection
     policies: UserPoliciesCollection
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/type_defs.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iam.type_defs import AccessDetailTypeDef
 
-    data: AccessDetailTypeDef = {...}
+    data: AccessDetailTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccessAdvisorUsageGranularityTypeType,
     ContextKeyTypeEnumType,
     DeletionTaskStatusTypeType,
     EntityTypeType,
     PolicyEvaluationDecisionTypeType,
@@ -41,15 +41,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessDetailTypeDef",
     "AccessKeyLastUsedTypeDef",
     "AccessKeyMetadataTypeDef",
     "AccessKeyTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
@@ -62,15 +61,15 @@
     "AttachGroupPolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachedPermissionsBoundaryTypeDef",
     "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
@@ -82,15 +81,14 @@
     "TagTypeDef",
     "CreateLoginProfileRequestLoginProfileCreateTypeDef",
     "CreateLoginProfileRequestRequestTypeDef",
     "CreateLoginProfileRequestUserCreateLoginProfileTypeDef",
     "LoginProfileTypeDef",
     "CreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "PolicyVersionTypeDef",
     "CreateServiceLinkedRoleRequestRequestTypeDef",
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     "ServiceSpecificCredentialTypeDef",
     "DeactivateMFADeviceRequestRequestTypeDef",
     "DeleteAccessKeyRequestRequestTypeDef",
     "DeleteAccountAliasRequestRequestTypeDef",
     "DeleteGroupPolicyRequestRequestTypeDef",
@@ -103,15 +101,14 @@
     "DeleteRolePermissionsBoundaryRequestRequestTypeDef",
     "DeleteRolePolicyRequestRequestTypeDef",
     "DeleteRoleRequestRequestTypeDef",
     "DeleteSAMLProviderRequestRequestTypeDef",
     "DeleteSSHPublicKeyRequestRequestTypeDef",
     "DeleteServerCertificateRequestRequestTypeDef",
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
-    "DeleteServiceLinkedRoleResponseTypeDef",
     "DeleteServiceSpecificCredentialRequestRequestTypeDef",
     "DeleteSigningCertificateRequestRequestTypeDef",
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     "DeleteUserPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
     "RoleUsageTypeTypeDef",
@@ -120,141 +117,95 @@
     "DetachGroupPolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestPolicyDetachRoleTypeDef",
     "DetachRolePolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestRoleDetachPolicyTypeDef",
     "DetachUserPolicyRequestPolicyDetachUserTypeDef",
     "DetachUserPolicyRequestRequestTypeDef",
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     "EnableMFADeviceRequestRequestTypeDef",
     "EnableMFADeviceRequestUserEnableMfaTypeDef",
     "EntityInfoTypeDef",
     "ErrorDetailsTypeDef",
     "OrganizationsDecisionDetailTypeDef",
     "PermissionsBoundaryDecisionDetailTypeDef",
-    "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportRequestRequestTypeDef",
-    "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsRequestRequestTypeDef",
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedRequestRequestTypeDef",
-    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
     "PasswordPolicyTypeDef",
-    "GetAccountSummaryResponseTypeDef",
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
-    "GetContextKeysForPolicyResponseTypeDef",
     "GetContextKeysForPrincipalPolicyRequestRequestTypeDef",
-    "GetCredentialReportResponseTypeDef",
     "GetGroupPolicyRequestRequestTypeDef",
-    "GetGroupPolicyResponseTypeDef",
-    "GetGroupRequestGetGroupPaginateTypeDef",
     "GetGroupRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetLoginProfileRequestRequestTypeDef",
     "GetMFADeviceRequestRequestTypeDef",
-    "GetMFADeviceResponseTypeDef",
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     "GetOrganizationsAccessReportRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
     "GetRolePolicyRequestRequestTypeDef",
-    "GetRolePolicyResponseTypeDef",
     "GetRoleRequestRequestTypeDef",
     "GetSAMLProviderRequestRequestTypeDef",
     "GetSSHPublicKeyRequestRequestTypeDef",
     "SSHPublicKeyTypeDef",
     "GetServerCertificateRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     "GetUserPolicyRequestRequestTypeDef",
-    "GetUserPolicyResponseTypeDef",
     "GetUserRequestRequestTypeDef",
     "PolicyDetailTypeDef",
-    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     "ListAccessKeysRequestRequestTypeDef",
-    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
     "ListAccountAliasesRequestRequestTypeDef",
-    "ListAccountAliasesResponseTypeDef",
-    "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
     "ListAttachedGroupPoliciesRequestRequestTypeDef",
-    "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
     "ListAttachedRolePoliciesRequestRequestTypeDef",
-    "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
     "ListAttachedUserPoliciesRequestRequestTypeDef",
-    "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
     "ListEntitiesForPolicyRequestRequestTypeDef",
     "PolicyGroupTypeDef",
     "PolicyRoleTypeDef",
     "PolicyUserTypeDef",
-    "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     "ListGroupPoliciesRequestRequestTypeDef",
-    "ListGroupPoliciesResponseTypeDef",
-    "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
     "ListGroupsForUserRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
     "ListInstanceProfileTagsRequestRequestTypeDef",
-    "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
     "ListInstanceProfilesForRoleRequestRequestTypeDef",
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
-    "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
     "ListMFADeviceTagsRequestRequestTypeDef",
-    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
     "ListMFADevicesRequestRequestTypeDef",
     "MFADeviceTypeDef",
-    "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
     "ListOpenIDConnectProviderTagsRequestRequestTypeDef",
     "OpenIDConnectProviderListEntryTypeDef",
     "PolicyGrantingServiceAccessTypeDef",
     "ListPoliciesGrantingServiceAccessRequestRequestTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
-    "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
     "ListPolicyTagsRequestRequestTypeDef",
-    "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
-    "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
     "ListRolePoliciesRequestRequestTypeDef",
-    "ListRolePoliciesResponseTypeDef",
-    "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
     "ListRoleTagsRequestRequestTypeDef",
-    "ListRolesRequestListRolesPaginateTypeDef",
     "ListRolesRequestRequestTypeDef",
-    "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
     "ListSAMLProviderTagsRequestRequestTypeDef",
     "SAMLProviderListEntryTypeDef",
-    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     "ListSSHPublicKeysRequestRequestTypeDef",
     "SSHPublicKeyMetadataTypeDef",
-    "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
     "ListServerCertificateTagsRequestRequestTypeDef",
-    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
     "ListServerCertificatesRequestRequestTypeDef",
     "ServerCertificateMetadataTypeDef",
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
     "ServiceSpecificCredentialMetadataTypeDef",
-    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
     "ListSigningCertificatesRequestRequestTypeDef",
     "SigningCertificateTypeDef",
-    "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     "ListUserPoliciesRequestRequestTypeDef",
-    "ListUserPoliciesResponseTypeDef",
-    "ListUserTagsRequestListUserTagsPaginateTypeDef",
     "ListUserTagsRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
     "ListVirtualMFADevicesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "PolicyDocumentStatementTypeDef",
     "PositionTypeDef",
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     "PutGroupPolicyRequestGroupPolicyPutTypeDef",
     "PutGroupPolicyRequestRequestTypeDef",
     "PutRolePermissionsBoundaryRequestRequestTypeDef",
     "PutRolePolicyRequestRequestTypeDef",
     "PutRolePolicyRequestRolePolicyPutTypeDef",
@@ -265,20 +216,17 @@
     "RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef",
     "RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef",
     "RemoveRoleFromInstanceProfileRequestRequestTypeDef",
     "RemoveUserFromGroupRequestGroupRemoveUserTypeDef",
     "RemoveUserFromGroupRequestRequestTypeDef",
     "RemoveUserFromGroupRequestUserRemoveGroupTypeDef",
     "ResetServiceSpecificCredentialRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     "ResyncMFADeviceRequestRequestTypeDef",
     "RoleLastUsedTypeDef",
-    "RoleLastUsedResponseMetadataTypeDef",
-    "ServerCertificateMetadataResponseMetadataTypeDef",
     "TrackedActionLastAccessedTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetSecurityTokenServicePreferencesRequestRequestTypeDef",
     "UntagInstanceProfileRequestRequestTypeDef",
     "UntagMFADeviceRequestRequestTypeDef",
     "UntagOpenIDConnectProviderRequestRequestTypeDef",
     "UntagPolicyRequestRequestTypeDef",
@@ -301,37 +249,54 @@
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     "UpdateLoginProfileRequestRequestTypeDef",
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     "UpdateRoleDescriptionRequestRequestTypeDef",
     "UpdateRoleRequestRequestTypeDef",
     "UpdateSAMLProviderRequestRequestTypeDef",
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
-    "UpdateSAMLProviderResponseTypeDef",
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     "UpdateServerCertificateRequestRequestTypeDef",
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     "UpdateServiceSpecificCredentialRequestRequestTypeDef",
     "UpdateSigningCertificateRequestRequestTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
+    "AttachedPermissionsBoundaryResponseTypeDef",
+    "CreateAccessKeyResponseTypeDef",
+    "DeleteServiceLinkedRoleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GenerateCredentialReportResponseTypeDef",
+    "GenerateOrganizationsAccessReportResponseTypeDef",
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedResponseTypeDef",
+    "GetAccountSummaryResponseTypeDef",
+    "GetContextKeysForPolicyResponseTypeDef",
+    "GetCredentialReportResponseTypeDef",
+    "GetGroupPolicyResponseTypeDef",
+    "GetMFADeviceResponseTypeDef",
+    "GetRolePolicyResponseTypeDef",
+    "GetUserPolicyResponseTypeDef",
     "ListAccessKeysResponseTypeDef",
-    "CreateAccessKeyResponseTypeDef",
+    "ListAccountAliasesResponseTypeDef",
+    "ListGroupPoliciesResponseTypeDef",
+    "ListRolePoliciesResponseTypeDef",
+    "ListUserPoliciesResponseTypeDef",
+    "RoleLastUsedResponseTypeDef",
+    "ServerCertificateMetadataResponseTypeDef",
+    "UpdateSAMLProviderResponseTypeDef",
     "ListAttachedGroupPoliciesResponseTypeDef",
     "ListAttachedRolePoliciesResponseTypeDef",
     "ListAttachedUserPoliciesResponseTypeDef",
     "SimulateCustomPolicyRequestRequestTypeDef",
-    "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
     "SimulatePrincipalPolicyRequestRequestTypeDef",
-    "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
     "CreateGroupResponseTypeDef",
     "ListGroupsForUserResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
     "CreateOpenIDConnectProviderResponseTypeDef",
@@ -364,27 +329,57 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
-    "UserResponseMetadataTypeDef",
+    "UserResponseTypeDef",
     "UserTypeDef",
     "CreateLoginProfileResponseTypeDef",
     "GetLoginProfileResponseTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "ListPolicyVersionsResponseTypeDef",
-    "ManagedPolicyDetailTypeDef",
     "CreateServiceSpecificCredentialResponseTypeDef",
     "ResetServiceSpecificCredentialResponseTypeDef",
     "DeletionTaskFailureReasonTypeTypeDef",
     "EntityDetailsTypeDef",
     "GetOrganizationsAccessReportResponseTypeDef",
+    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+    "GetGroupRequestGetGroupPaginateTypeDef",
+    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
+    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
+    "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
+    "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
+    "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
+    "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
+    "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
+    "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
+    "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
+    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
+    "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
+    "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
+    "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
+    "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
+    "ListRolesRequestListRolesPaginateTypeDef",
+    "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
+    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
+    "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
+    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
+    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
+    "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
+    "ListUserTagsRequestListUserTagsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
+    "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
+    "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
     "GetAccountPasswordPolicyResponseTypeDef",
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
     "GetSSHPublicKeyResponseTypeDef",
     "UploadSSHPublicKeyResponseTypeDef",
@@ -398,14 +393,15 @@
     "ListSSHPublicKeysResponseTypeDef",
     "ListServerCertificatesResponseTypeDef",
     "ServerCertificateTypeDef",
     "UploadServerCertificateResponseTypeDef",
     "ListServiceSpecificCredentialsResponseTypeDef",
     "ListSigningCertificatesResponseTypeDef",
     "UploadSigningCertificateResponseTypeDef",
+    "PolicyDocumentFixedTypeDef",
     "StatementTypeDef",
     "RoleTypeDef",
     "ServiceLastAccessedTypeDef",
     "CreatePolicyResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "CreateUserResponseTypeDef",
@@ -413,24 +409,29 @@
     "GetUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "VirtualMFADeviceTypeDef",
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     "GetServerCertificateResponseTypeDef",
+    "PolicyVersionTypeDef",
     "ResourceSpecificResultTypeDef",
     "CreateRoleResponseTypeDef",
     "CreateServiceLinkedRoleResponseTypeDef",
     "GetRoleResponseTypeDef",
     "InstanceProfileTypeDef",
     "ListRolesResponseTypeDef",
     "UpdateRoleDescriptionResponseTypeDef",
     "GetServiceLastAccessedDetailsResponseTypeDef",
     "CreateVirtualMFADeviceResponseTypeDef",
     "ListVirtualMFADevicesResponseTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "ListPolicyVersionsResponseTypeDef",
+    "ManagedPolicyDetailTypeDef",
     "EvaluationResultTypeDef",
     "CreateInstanceProfileResponseTypeDef",
     "GetInstanceProfileResponseTypeDef",
     "ListInstanceProfilesForRoleResponseTypeDef",
     "ListInstanceProfilesResponseTypeDef",
     "RoleDetailTypeDef",
     "SimulatePolicyResponseTypeDef",
@@ -451,19 +452,17 @@
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
     total=False,
 )
 
-
 class AccessDetailTypeDef(_RequiredAccessDetailTypeDef, _OptionalAccessDetailTypeDef):
     pass
 
-
 AccessKeyLastUsedTypeDef = TypedDict(
     "AccessKeyLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
@@ -493,19 +492,17 @@
     "_OptionalAccessKeyTypeDef",
     {
         "CreateDate": datetime,
     },
     total=False,
 )
 
-
 class AccessKeyTypeDef(_RequiredAccessKeyTypeDef, _OptionalAccessKeyTypeDef):
     pass
 
-
 AddClientIDToOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "ClientID": str,
     },
 )
@@ -609,20 +606,22 @@
 AttachUserPolicyRequestUserAttachPolicyTypeDef = TypedDict(
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
-        "PermissionsBoundaryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AttachedPermissionsBoundaryTypeDef = TypedDict(
     "AttachedPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
@@ -706,43 +705,39 @@
     "_OptionalCreateGroupRequestRequestTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef = TypedDict(
     "_RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef = TypedDict(
     "_OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
-
 class CreateGroupRequestServiceResourceCreateGroupTypeDef(
     _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef,
     _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef,
 ):
     pass
 
-
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
@@ -768,22 +763,20 @@
     "_OptionalCreateLoginProfileRequestLoginProfileCreateTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
-
 class CreateLoginProfileRequestLoginProfileCreateTypeDef(
     _RequiredCreateLoginProfileRequestLoginProfileCreateTypeDef,
     _OptionalCreateLoginProfileRequestLoginProfileCreateTypeDef,
 ):
     pass
 
-
 _RequiredCreateLoginProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoginProfileRequestRequestTypeDef",
     {
         "UserName": str,
         "Password": str,
     },
 )
@@ -791,44 +784,40 @@
     "_OptionalCreateLoginProfileRequestRequestTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
-
 class CreateLoginProfileRequestRequestTypeDef(
     _RequiredCreateLoginProfileRequestRequestTypeDef,
     _OptionalCreateLoginProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef = TypedDict(
     "_RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef",
     {
         "Password": str,
     },
 )
 _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef = TypedDict(
     "_OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
-
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
-
 _RequiredLoginProfileTypeDef = TypedDict(
     "_RequiredLoginProfileTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
     },
 )
@@ -836,41 +825,37 @@
     "_OptionalLoginProfileTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
-
 class LoginProfileTypeDef(_RequiredLoginProfileTypeDef, _OptionalLoginProfileTypeDef):
     pass
 
-
 _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "PolicyDocument": str,
     },
 )
 _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "SetAsDefault": bool,
     },
     total=False,
 )
 
-
 class CreatePolicyVersionRequestPolicyCreateVersionTypeDef(
     _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef,
 ):
     pass
 
-
 _RequiredCreatePolicyVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestRequestTypeDef",
     {
         "PolicyArn": str,
         "PolicyDocument": str,
     },
 )
@@ -878,33 +863,20 @@
     "_OptionalCreatePolicyVersionRequestRequestTypeDef",
     {
         "SetAsDefault": bool,
     },
     total=False,
 )
 
-
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
-
-PolicyVersionTypeDef = TypedDict(
-    "PolicyVersionTypeDef",
-    {
-        "Document": str,
-        "VersionId": str,
-        "IsDefaultVersion": bool,
-        "CreateDate": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceLinkedRoleRequestRequestTypeDef",
     {
         "AWSServiceName": str,
     },
 )
 _OptionalCreateServiceLinkedRoleRequestRequestTypeDef = TypedDict(
@@ -912,22 +884,20 @@
     {
         "Description": str,
         "CustomSuffix": str,
     },
     total=False,
 )
 
-
 class CreateServiceLinkedRoleRequestRequestTypeDef(
     _RequiredCreateServiceLinkedRoleRequestRequestTypeDef,
     _OptionalCreateServiceLinkedRoleRequestRequestTypeDef,
 ):
     pass
 
-
 CreateServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
 )
@@ -963,21 +933,19 @@
     "_OptionalDeleteAccessKeyRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class DeleteAccessKeyRequestRequestTypeDef(
     _RequiredDeleteAccessKeyRequestRequestTypeDef, _OptionalDeleteAccessKeyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteAccountAliasRequestRequestTypeDef = TypedDict(
     "DeleteAccountAliasRequestRequestTypeDef",
     {
         "AccountAlias": str,
     },
 )
 
@@ -1079,66 +1047,54 @@
 DeleteServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
-DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
-    "DeleteServiceLinkedRoleResponseTypeDef",
-    {
-        "DeletionTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef",
     {
         "ServiceSpecificCredentialId": str,
     },
 )
 _OptionalDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class DeleteServiceSpecificCredentialRequestRequestTypeDef(
     _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef,
     _OptionalDeleteServiceSpecificCredentialRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteSigningCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSigningCertificateRequestRequestTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalDeleteSigningCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSigningCertificateRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class DeleteSigningCertificateRequestRequestTypeDef(
     _RequiredDeleteSigningCertificateRequestRequestTypeDef,
     _OptionalDeleteSigningCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteUserPermissionsBoundaryRequestRequestTypeDef = TypedDict(
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 
@@ -1235,21 +1191,14 @@
 DetachUserPolicyRequestUserDetachPolicyTypeDef = TypedDict(
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableMFADeviceRequestMfaDeviceAssociateTypeDef = TypedDict(
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     {
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
@@ -1286,19 +1235,17 @@
     "_OptionalEntityInfoTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
-
 class EntityInfoTypeDef(_RequiredEntityInfoTypeDef, _OptionalEntityInfoTypeDef):
     pass
 
-
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
@@ -1315,95 +1262,67 @@
     "PermissionsBoundaryDecisionDetailTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
     total=False,
 )
 
-GenerateCredentialReportResponseTypeDef = TypedDict(
-    "GenerateCredentialReportResponseTypeDef",
-    {
-        "State": ReportStateTypeType,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef",
     {
         "EntityPath": str,
     },
 )
 _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef",
     {
         "OrganizationsPolicyId": str,
     },
     total=False,
 )
 
-
 class GenerateOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
-
-GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
-    "GenerateOrganizationsAccessReportResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef",
     {
         "Granularity": AccessAdvisorUsageGranularityTypeType,
     },
     total=False,
 )
 
-
 class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
-
-GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAccessKeyLastUsedRequestRequestTypeDef = TypedDict(
     "GetAccessKeyLastUsedRequestRequestTypeDef",
     {
         "AccessKeyId": str,
     },
 )
 
-GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef = TypedDict(
-    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filter": Sequence[EntityTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetAccountAuthorizationDetailsRequestRequestTypeDef = TypedDict(
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
     {
@@ -1427,108 +1346,49 @@
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
     total=False,
 )
 
-GetAccountSummaryResponseTypeDef = TypedDict(
-    "GetAccountSummaryResponseTypeDef",
-    {
-        "SummaryMap": Dict[summaryKeyTypeType, int],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContextKeysForCustomPolicyRequestRequestTypeDef = TypedDict(
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
 )
 
-GetContextKeysForPolicyResponseTypeDef = TypedDict(
-    "GetContextKeysForPolicyResponseTypeDef",
-    {
-        "ContextKeyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef",
     {
         "PolicySourceArn": str,
     },
 )
 _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
     total=False,
 )
 
-
 class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(
     _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
     _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-GetCredentialReportResponseTypeDef = TypedDict(
-    "GetCredentialReportResponseTypeDef",
-    {
-        "Content": bytes,
-        "ReportFormat": Literal["text/csv"],
-        "GeneratedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupPolicyRequestRequestTypeDef = TypedDict(
     "GetGroupPolicyRequestRequestTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
     },
 )
 
-GetGroupPolicyResponseTypeDef = TypedDict(
-    "GetGroupPolicyResponseTypeDef",
-    {
-        "GroupName": str,
-        "PolicyName": str,
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
-    "_RequiredGetGroupRequestGetGroupPaginateTypeDef",
-    {
-        "GroupName": str,
-    },
-)
-_OptionalGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
-    "_OptionalGetGroupRequestGetGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetGroupRequestGetGroupPaginateTypeDef(
-    _RequiredGetGroupRequestGetGroupPaginateTypeDef, _OptionalGetGroupRequestGetGroupPaginateTypeDef
-):
-    pass
-
-
 _RequiredGetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetGroupRequestRequestTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalGetGroupRequestRequestTypeDef = TypedDict(
@@ -1536,21 +1396,19 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class GetGroupRequestRequestTypeDef(
     _RequiredGetGroupRequestRequestTypeDef, _OptionalGetGroupRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1580,32 +1438,19 @@
     "_OptionalGetMFADeviceRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class GetMFADeviceRequestRequestTypeDef(
     _RequiredGetMFADeviceRequestRequestTypeDef, _OptionalGetMFADeviceRequestRequestTypeDef
 ):
     pass
 
-
-GetMFADeviceResponseTypeDef = TypedDict(
-    "GetMFADeviceResponseTypeDef",
-    {
-        "UserName": str,
-        "SerialNumber": str,
-        "EnableDate": datetime,
-        "Certifications": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
     },
 )
 
@@ -1621,22 +1466,20 @@
         "MaxItems": int,
         "Marker": str,
         "SortKey": sortKeyTypeType,
     },
     total=False,
 )
 
-
 class GetOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGetOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGetOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
-
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
@@ -1652,24 +1495,14 @@
     "GetRolePolicyRequestRequestTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
     },
 )
 
-GetRolePolicyResponseTypeDef = TypedDict(
-    "GetRolePolicyResponseTypeDef",
-    {
-        "RoleName": str,
-        "PolicyName": str,
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRoleRequestRequestTypeDef = TypedDict(
     "GetRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
@@ -1703,19 +1536,17 @@
     "_OptionalSSHPublicKeyTypeDef",
     {
         "UploadDate": datetime,
     },
     total=False,
 )
 
-
 class SSHPublicKeyTypeDef(_RequiredSSHPublicKeyTypeDef, _OptionalSSHPublicKeyTypeDef):
     pass
 
-
 GetServerCertificateRequestRequestTypeDef = TypedDict(
     "GetServerCertificateRequestRequestTypeDef",
     {
         "ServerCertificateName": str,
     },
 )
 
@@ -1730,22 +1561,20 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGetServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGetServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     {
         "JobId": str,
         "ServiceNamespace": str,
     },
 )
@@ -1754,22 +1583,20 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef(
     _RequiredGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     _OptionalGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
 ):
     pass
 
-
 GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     {
         "DeletionTaskId": str,
     },
 )
 
@@ -1777,24 +1604,14 @@
     "GetUserPolicyRequestRequestTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
     },
 )
 
-GetUserPolicyResponseTypeDef = TypedDict(
-    "GetUserPolicyResponseTypeDef",
-    {
-        "UserName": str,
-        "PolicyName": str,
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
@@ -1804,83 +1621,33 @@
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
     total=False,
 )
 
-ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
-    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAccessKeysRequestRequestTypeDef = TypedDict(
     "ListAccessKeysRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesRequestListAccountAliasesPaginateTypeDef = TypedDict(
-    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAccountAliasesRequestRequestTypeDef = TypedDict(
     "ListAccountAliasesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesResponseTypeDef = TypedDict(
-    "ListAccountAliasesResponseTypeDef",
-    {
-        "AccountAliases": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
-    {
-        "GroupName": str,
-    },
-)
-_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef(
-    _RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
-    _OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedGroupPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedGroupPoliciesRequestRequestTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalListAttachedGroupPoliciesRequestRequestTypeDef = TypedDict(
@@ -1889,45 +1656,20 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListAttachedGroupPoliciesRequestRequestTypeDef(
     _RequiredListAttachedGroupPoliciesRequestRequestTypeDef,
     _OptionalListAttachedGroupPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef(
-    _RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
-    _OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedRolePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedRolePoliciesRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 _OptionalListAttachedRolePoliciesRequestRequestTypeDef = TypedDict(
@@ -1936,45 +1678,20 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListAttachedRolePoliciesRequestRequestTypeDef(
     _RequiredListAttachedRolePoliciesRequestRequestTypeDef,
     _OptionalListAttachedRolePoliciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef(
-    _RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
-    _OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedUserPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedUserPoliciesRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalListAttachedUserPoliciesRequestRequestTypeDef = TypedDict(
@@ -1983,47 +1700,20 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListAttachedUserPoliciesRequestRequestTypeDef(
     _RequiredListAttachedUserPoliciesRequestRequestTypeDef,
     _OptionalListAttachedUserPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
-    "_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
-    "_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
-    {
-        "EntityFilter": EntityTypeType,
-        "PathPrefix": str,
-        "PolicyUsageFilter": PolicyUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef(
-    _RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
-    _OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEntitiesForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesForPolicyRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalListEntitiesForPolicyRequestRequestTypeDef = TypedDict(
@@ -2034,22 +1724,20 @@
         "PolicyUsageFilter": PolicyUsageTypeType,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListEntitiesForPolicyRequestRequestTypeDef(
     _RequiredListEntitiesForPolicyRequestRequestTypeDef,
     _OptionalListEntitiesForPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 PolicyGroupTypeDef = TypedDict(
     "PolicyGroupTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
     total=False,
@@ -2069,36 +1757,14 @@
     {
         "UserName": str,
         "UserId": str,
     },
     total=False,
 )
 
-_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
-    {
-        "GroupName": str,
-    },
-)
-_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef(
-    _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
-    _OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupPoliciesRequestRequestTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalListGroupPoliciesRequestRequestTypeDef = TypedDict(
@@ -2106,53 +1772,19 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListGroupPoliciesRequestRequestTypeDef(
     _RequiredListGroupPoliciesRequestRequestTypeDef, _OptionalListGroupPoliciesRequestRequestTypeDef
 ):
     pass
 
-
-ListGroupPoliciesResponseTypeDef = TypedDict(
-    "ListGroupPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupsForUserRequestListGroupsForUserPaginateTypeDef(
-    _RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
-    _OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsForUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalListGroupsForUserRequestRequestTypeDef = TypedDict(
@@ -2160,62 +1792,29 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListGroupsForUserRequestRequestTypeDef(
     _RequiredListGroupsForUserRequestRequestTypeDef, _OptionalListGroupsForUserRequestRequestTypeDef
 ):
     pass
 
-
-ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
-    {
-        "InstanceProfileName": str,
-    },
-)
-_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef(
-    _RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
-    _OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstanceProfileTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceProfileTagsRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
     },
 )
 _OptionalListInstanceProfileTagsRequestRequestTypeDef = TypedDict(
@@ -2223,44 +1822,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListInstanceProfileTagsRequestRequestTypeDef(
     _RequiredListInstanceProfileTagsRequestRequestTypeDef,
     _OptionalListInstanceProfileTagsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
-    "_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
-    "_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef(
-    _RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
-    _OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstanceProfilesForRoleRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceProfilesForRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 _OptionalListInstanceProfilesForRoleRequestRequestTypeDef = TypedDict(
@@ -2268,63 +1843,30 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListInstanceProfilesForRoleRequestRequestTypeDef(
     _RequiredListInstanceProfilesForRoleRequestRequestTypeDef,
     _OptionalListInstanceProfilesForRoleRequestRequestTypeDef,
 ):
     pass
 
-
-ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstanceProfilesRequestRequestTypeDef = TypedDict(
     "ListInstanceProfilesRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
-    "_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
-    {
-        "SerialNumber": str,
-    },
-)
-_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
-    "_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef(
-    _RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
-    _OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMFADeviceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListMFADeviceTagsRequestRequestTypeDef",
     {
         "SerialNumber": str,
     },
 )
 _OptionalListMFADeviceTagsRequestRequestTypeDef = TypedDict(
@@ -2332,30 +1874,19 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListMFADeviceTagsRequestRequestTypeDef(
     _RequiredListMFADeviceTagsRequestRequestTypeDef, _OptionalListMFADeviceTagsRequestRequestTypeDef
 ):
     pass
 
-
-ListMFADevicesRequestListMFADevicesPaginateTypeDef = TypedDict(
-    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMFADevicesRequestRequestTypeDef = TypedDict(
     "ListMFADevicesRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -2367,40 +1898,14 @@
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
     },
 )
 
-_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
-        {
-            "OpenIDConnectProviderArn": str,
-        },
-    )
-)
-_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef(
-    _RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
-    _OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
     },
 )
 _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef = TypedDict(
@@ -2408,22 +1913,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListOpenIDConnectProviderTagsRequestRequestTypeDef(
     _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef,
     _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef,
 ):
     pass
 
-
 OpenIDConnectProviderListEntryTypeDef = TypedDict(
     "OpenIDConnectProviderListEntryTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -2441,21 +1944,19 @@
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
     total=False,
 )
 
-
 class PolicyGrantingServiceAccessTypeDef(
     _RequiredPolicyGrantingServiceAccessTypeDef, _OptionalPolicyGrantingServiceAccessTypeDef
 ):
     pass
 
-
 _RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     {
         "Arn": str,
         "ServiceNamespaces": Sequence[str],
     },
 )
@@ -2463,69 +1964,33 @@
     "_OptionalListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListPoliciesGrantingServiceAccessRequestRequestTypeDef(
     _RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     _OptionalListPoliciesGrantingServiceAccessRequestRequestTypeDef,
 ):
     pass
 
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "Scope": policyScopeTypeType,
-        "OnlyAttached": bool,
-        "PathPrefix": str,
-        "PolicyUsageFilter": PolicyUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "Scope": policyScopeTypeType,
         "OnlyAttached": bool,
         "PathPrefix": str,
         "PolicyUsageFilter": PolicyUsageTypeType,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyTagsRequestListPolicyTagsPaginateTypeDef(
-    _RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
-    _OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyTagsRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalListPolicyTagsRequestRequestTypeDef = TypedDict(
@@ -2533,43 +1998,19 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListPolicyTagsRequestRequestTypeDef(
     _RequiredListPolicyTagsRequestRequestTypeDef, _OptionalListPolicyTagsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef(
-    _RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
-    _OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyVersionsRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalListPolicyVersionsRequestRequestTypeDef = TypedDict(
@@ -2577,44 +2018,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListPolicyVersionsRequestRequestTypeDef(
     _RequiredListPolicyVersionsRequestRequestTypeDef,
     _OptionalListPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRolePoliciesRequestListRolePoliciesPaginateTypeDef(
-    _RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
-    _OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRolePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListRolePoliciesRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 _OptionalListRolePoliciesRequestRequestTypeDef = TypedDict(
@@ -2622,53 +2039,19 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListRolePoliciesRequestRequestTypeDef(
     _RequiredListRolePoliciesRequestRequestTypeDef, _OptionalListRolePoliciesRequestRequestTypeDef
 ):
     pass
 
-
-ListRolePoliciesResponseTypeDef = TypedDict(
-    "ListRolePoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
-    "_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
-    "_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRoleTagsRequestListRoleTagsPaginateTypeDef(
-    _RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef,
-    _OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRoleTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListRoleTagsRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 _OptionalListRoleTagsRequestRequestTypeDef = TypedDict(
@@ -2676,62 +2059,29 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListRoleTagsRequestRequestTypeDef(
     _RequiredListRoleTagsRequestRequestTypeDef, _OptionalListRoleTagsRequestRequestTypeDef
 ):
     pass
 
-
-ListRolesRequestListRolesPaginateTypeDef = TypedDict(
-    "ListRolesRequestListRolesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRolesRequestRequestTypeDef = TypedDict(
     "ListRolesRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
-    "_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
-    {
-        "SAMLProviderArn": str,
-    },
-)
-_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
-    "_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef(
-    _RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
-    _OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSAMLProviderTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListSAMLProviderTagsRequestRequestTypeDef",
     {
         "SAMLProviderArn": str,
     },
 )
 _OptionalListSAMLProviderTagsRequestRequestTypeDef = TypedDict(
@@ -2739,41 +2089,30 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListSAMLProviderTagsRequestRequestTypeDef(
     _RequiredListSAMLProviderTagsRequestRequestTypeDef,
     _OptionalListSAMLProviderTagsRequestRequestTypeDef,
 ):
     pass
 
-
 SAMLProviderListEntryTypeDef = TypedDict(
     "SAMLProviderListEntryTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
     total=False,
 )
 
-ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = TypedDict(
-    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSSHPublicKeysRequestRequestTypeDef = TypedDict(
     "ListSSHPublicKeysRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -2786,36 +2125,14 @@
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
 )
 
-_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
-    "_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
-    {
-        "ServerCertificateName": str,
-    },
-)
-_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
-    "_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef(
-    _RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
-    _OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServerCertificateTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListServerCertificateTagsRequestRequestTypeDef",
     {
         "ServerCertificateName": str,
     },
 )
 _OptionalListServerCertificateTagsRequestRequestTypeDef = TypedDict(
@@ -2823,31 +2140,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListServerCertificateTagsRequestRequestTypeDef(
     _RequiredListServerCertificateTagsRequestRequestTypeDef,
     _OptionalListServerCertificateTagsRequestRequestTypeDef,
 ):
     pass
 
-
-ListServerCertificatesRequestListServerCertificatesPaginateTypeDef = TypedDict(
-    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServerCertificatesRequestRequestTypeDef = TypedDict(
     "ListServerCertificatesRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -2868,21 +2174,19 @@
     {
         "UploadDate": datetime,
         "Expiration": datetime,
     },
     total=False,
 )
 
-
 class ServerCertificateMetadataTypeDef(
     _RequiredServerCertificateMetadataTypeDef, _OptionalServerCertificateMetadataTypeDef
 ):
     pass
 
-
 ListServiceSpecificCredentialsRequestRequestTypeDef = TypedDict(
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
@@ -2896,23 +2200,14 @@
         "ServiceUserName": str,
         "CreateDate": datetime,
         "ServiceSpecificCredentialId": str,
         "ServiceName": str,
     },
 )
 
-ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef = TypedDict(
-    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningCertificatesRequestRequestTypeDef = TypedDict(
     "ListSigningCertificatesRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -2932,43 +2227,19 @@
     "_OptionalSigningCertificateTypeDef",
     {
         "UploadDate": datetime,
     },
     total=False,
 )
 
-
 class SigningCertificateTypeDef(
     _RequiredSigningCertificateTypeDef, _OptionalSigningCertificateTypeDef
 ):
     pass
 
-
-_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUserPoliciesRequestListUserPoliciesPaginateTypeDef(
-    _RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
-    _OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUserPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoliciesRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalListUserPoliciesRequestRequestTypeDef = TypedDict(
@@ -2976,53 +2247,19 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListUserPoliciesRequestRequestTypeDef(
     _RequiredListUserPoliciesRequestRequestTypeDef, _OptionalListUserPoliciesRequestRequestTypeDef
 ):
     pass
 
-
-ListUserPoliciesResponseTypeDef = TypedDict(
-    "ListUserPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
-    "_RequiredListUserTagsRequestListUserTagsPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
-    "_OptionalListUserTagsRequestListUserTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUserTagsRequestListUserTagsPaginateTypeDef(
-    _RequiredListUserTagsRequestListUserTagsPaginateTypeDef,
-    _OptionalListUserTagsRequestListUserTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUserTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserTagsRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalListUserTagsRequestRequestTypeDef = TypedDict(
@@ -3030,67 +2267,47 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListUserTagsRequestRequestTypeDef(
     _RequiredListUserTagsRequestRequestTypeDef, _OptionalListUserTagsRequestRequestTypeDef
 ):
     pass
 
-
-ListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "ListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsersRequestRequestTypeDef = TypedDict(
     "ListUsersRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef = TypedDict(
-    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
-    {
-        "AssignmentStatus": assignmentStatusTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVirtualMFADevicesRequestRequestTypeDef = TypedDict(
     "ListVirtualMFADevicesRequestRequestTypeDef",
     {
         "AssignmentStatus": assignmentStatusTypeType,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PolicyDocumentStatementTypeDef = TypedDict(
+    "PolicyDocumentStatementTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Effect": str,
+        "Resource": Union[str, List[str]],
+        "Sid": str,
+        "Action": Union[str, List[str]],
     },
-    total=False,
 )
 
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "Line": int,
         "Column": int,
@@ -3233,33 +2450,20 @@
     "_OptionalResetServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class ResetServiceSpecificCredentialRequestRequestTypeDef(
     _RequiredResetServiceSpecificCredentialRequestRequestTypeDef,
     _OptionalResetServiceSpecificCredentialRequestRequestTypeDef,
 ):
     pass
 
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
 ResyncMFADeviceRequestMfaDeviceResyncTypeDef = TypedDict(
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     {
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
@@ -3279,36 +2483,14 @@
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
     total=False,
 )
 
-RoleLastUsedResponseMetadataTypeDef = TypedDict(
-    "RoleLastUsedResponseMetadataTypeDef",
-    {
-        "LastUsedDate": datetime,
-        "Region": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ServerCertificateMetadataResponseMetadataTypeDef = TypedDict(
-    "ServerCertificateMetadataResponseMetadataTypeDef",
-    {
-        "Path": str,
-        "ServerCertificateName": str,
-        "ServerCertificateId": str,
-        "Arn": str,
-        "UploadDate": datetime,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TrackedActionLastAccessedTypeDef = TypedDict(
     "TrackedActionLastAccessedTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
@@ -3438,21 +2620,19 @@
     "_OptionalUpdateAccessKeyRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class UpdateAccessKeyRequestRequestTypeDef(
     _RequiredUpdateAccessKeyRequestRequestTypeDef, _OptionalUpdateAccessKeyRequestRequestTypeDef
 ):
     pass
 
-
 UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef = TypedDict(
     "UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef",
     {
         "MinimumPasswordLength": int,
         "RequireSymbols": bool,
         "RequireNumbers": bool,
         "RequireUppercaseCharacters": bool,
@@ -3532,21 +2712,19 @@
     {
         "NewPath": str,
         "NewGroupName": str,
     },
     total=False,
 )
 
-
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
-
 UpdateLoginProfileRequestLoginProfileUpdateTypeDef = TypedDict(
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     {
         "Password": str,
         "PasswordResetRequired": bool,
     },
     total=False,
@@ -3563,22 +2741,20 @@
     {
         "Password": str,
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
-
 class UpdateLoginProfileRequestRequestTypeDef(
     _RequiredUpdateLoginProfileRequestRequestTypeDef,
     _OptionalUpdateLoginProfileRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef = TypedDict(
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "ThumbprintList": Sequence[str],
     },
 )
@@ -3602,21 +2778,19 @@
     {
         "Description": str,
         "MaxSessionDuration": int,
     },
     total=False,
 )
 
-
 class UpdateRoleRequestRequestTypeDef(
     _RequiredUpdateRoleRequestRequestTypeDef, _OptionalUpdateRoleRequestRequestTypeDef
 ):
     pass
 
-
 UpdateSAMLProviderRequestRequestTypeDef = TypedDict(
     "UpdateSAMLProviderRequestRequestTypeDef",
     {
         "SAMLMetadataDocument": str,
         "SAMLProviderArn": str,
     },
 )
@@ -3624,22 +2798,14 @@
 UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = TypedDict(
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
     {
         "SAMLMetadataDocument": str,
     },
 )
 
-UpdateSAMLProviderResponseTypeDef = TypedDict(
-    "UpdateSAMLProviderResponseTypeDef",
-    {
-        "SAMLProviderArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSSHPublicKeyRequestRequestTypeDef = TypedDict(
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
     },
@@ -3656,22 +2822,20 @@
     {
         "NewPath": str,
         "NewServerCertificateName": str,
     },
     total=False,
 )
 
-
 class UpdateServerCertificateRequestRequestTypeDef(
     _RequiredUpdateServerCertificateRequestRequestTypeDef,
     _OptionalUpdateServerCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateServerCertificateRequestServerCertificateUpdateTypeDef = TypedDict(
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     {
         "NewPath": str,
         "NewServerCertificateName": str,
     },
     total=False,
@@ -3688,22 +2852,20 @@
     "_OptionalUpdateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class UpdateServiceSpecificCredentialRequestRequestTypeDef(
     _RequiredUpdateServiceSpecificCredentialRequestRequestTypeDef,
     _OptionalUpdateServiceSpecificCredentialRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSigningCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSigningCertificateRequestRequestTypeDef",
     {
         "CertificateId": str,
         "Status": statusTypeType,
     },
 )
@@ -3711,22 +2873,20 @@
     "_OptionalUpdateSigningCertificateRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class UpdateSigningCertificateRequestRequestTypeDef(
     _RequiredUpdateSigningCertificateRequestRequestTypeDef,
     _OptionalUpdateSigningCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateSigningCertificateRequestSigningCertificateActivateTypeDef = TypedDict(
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     {
         "Status": statusTypeType,
     },
     total=False,
 )
@@ -3750,21 +2910,19 @@
     {
         "NewPath": str,
         "NewUserName": str,
     },
     total=False,
 )
 
-
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
-
 UpdateUserRequestUserUpdateTypeDef = TypedDict(
     "UpdateUserRequestUserUpdateTypeDef",
     {
         "NewPath": str,
         "NewUserName": str,
     },
     total=False,
@@ -3788,98 +2946,280 @@
     "_OptionalUploadSigningCertificateRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class UploadSigningCertificateRequestRequestTypeDef(
     _RequiredUploadSigningCertificateRequestRequestTypeDef,
     _OptionalUploadSigningCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef = TypedDict(
     "_RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     {
         "CertificateBody": str,
     },
 )
 _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef = TypedDict(
     "_OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-
 class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(
     _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
     _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
 ):
     pass
 
+AttachedPermissionsBoundaryResponseTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryResponseTypeDef",
+    {
+        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
+        "PermissionsBoundaryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessKeyResponseTypeDef = TypedDict(
+    "CreateAccessKeyResponseTypeDef",
+    {
+        "AccessKey": AccessKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
+    "DeleteServiceLinkedRoleResponseTypeDef",
+    {
+        "DeletionTaskId": str,
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
+GenerateCredentialReportResponseTypeDef = TypedDict(
+    "GenerateCredentialReportResponseTypeDef",
+    {
+        "State": ReportStateTypeType,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
+    "GenerateOrganizationsAccessReportResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetAccessKeyLastUsedResponseTypeDef = TypedDict(
     "GetAccessKeyLastUsedResponseTypeDef",
     {
         "UserName": str,
         "AccessKeyLastUsed": AccessKeyLastUsedTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSummaryResponseTypeDef = TypedDict(
+    "GetAccountSummaryResponseTypeDef",
+    {
+        "SummaryMap": Dict[summaryKeyTypeType, int],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContextKeysForPolicyResponseTypeDef = TypedDict(
+    "GetContextKeysForPolicyResponseTypeDef",
+    {
+        "ContextKeyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCredentialReportResponseTypeDef = TypedDict(
+    "GetCredentialReportResponseTypeDef",
+    {
+        "Content": bytes,
+        "ReportFormat": Literal["text/csv"],
+        "GeneratedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupPolicyResponseTypeDef = TypedDict(
+    "GetGroupPolicyResponseTypeDef",
+    {
+        "GroupName": str,
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMFADeviceResponseTypeDef = TypedDict(
+    "GetMFADeviceResponseTypeDef",
+    {
+        "UserName": str,
+        "SerialNumber": str,
+        "EnableDate": datetime,
+        "Certifications": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRolePolicyResponseTypeDef = TypedDict(
+    "GetRolePolicyResponseTypeDef",
+    {
+        "RoleName": str,
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserPolicyResponseTypeDef = TypedDict(
+    "GetUserPolicyResponseTypeDef",
+    {
+        "UserName": str,
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessKeysResponseTypeDef = TypedDict(
     "ListAccessKeysResponseTypeDef",
     {
         "AccessKeyMetadata": List[AccessKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAccessKeyResponseTypeDef = TypedDict(
-    "CreateAccessKeyResponseTypeDef",
+ListAccountAliasesResponseTypeDef = TypedDict(
+    "ListAccountAliasesResponseTypeDef",
     {
-        "AccessKey": AccessKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountAliases": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupPoliciesResponseTypeDef = TypedDict(
+    "ListGroupPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRolePoliciesResponseTypeDef = TypedDict(
+    "ListRolePoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUserPoliciesResponseTypeDef = TypedDict(
+    "ListUserPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RoleLastUsedResponseTypeDef = TypedDict(
+    "RoleLastUsedResponseTypeDef",
+    {
+        "LastUsedDate": datetime,
+        "Region": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerCertificateMetadataResponseTypeDef = TypedDict(
+    "ServerCertificateMetadataResponseTypeDef",
+    {
+        "Path": str,
+        "ServerCertificateName": str,
+        "ServerCertificateId": str,
+        "Arn": str,
+        "UploadDate": datetime,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSAMLProviderResponseTypeDef = TypedDict(
+    "UpdateSAMLProviderResponseTypeDef",
+    {
+        "SAMLProviderArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachedGroupPoliciesResponseTypeDef = TypedDict(
     "ListAttachedGroupPoliciesResponseTypeDef",
     {
         "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachedRolePoliciesResponseTypeDef = TypedDict(
     "ListAttachedRolePoliciesResponseTypeDef",
     {
         "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachedUserPoliciesResponseTypeDef = TypedDict(
     "ListAttachedUserPoliciesResponseTypeDef",
     {
         "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSimulateCustomPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSimulateCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
@@ -3898,52 +3238,20 @@
         "ResourceHandlingOption": str,
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class SimulateCustomPolicyRequestRequestTypeDef(
     _RequiredSimulateCustomPolicyRequestRequestTypeDef,
     _OptionalSimulateCustomPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
-    "_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
-    {
-        "PolicyInputList": Sequence[str],
-        "ActionNames": Sequence[str],
-    },
-)
-_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
-    "_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
-    {
-        "PermissionsBoundaryPolicyInputList": Sequence[str],
-        "ResourceArns": Sequence[str],
-        "ResourcePolicy": str,
-        "ResourceOwner": str,
-        "CallerArn": str,
-        "ContextEntries": Sequence[ContextEntryTypeDef],
-        "ResourceHandlingOption": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef(
-    _RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
-    _OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
-):
-    pass
-
-
 _RequiredSimulatePrincipalPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSimulatePrincipalPolicyRequestRequestTypeDef",
     {
         "PolicySourceArn": str,
         "ActionNames": Sequence[str],
     },
 )
@@ -3960,78 +3268,45 @@
         "ResourceHandlingOption": str,
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class SimulatePrincipalPolicyRequestRequestTypeDef(
     _RequiredSimulatePrincipalPolicyRequestRequestTypeDef,
     _OptionalSimulatePrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
-    "_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    {
-        "PolicySourceArn": str,
-        "ActionNames": Sequence[str],
-    },
-)
-_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
-    "_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    {
-        "PolicyInputList": Sequence[str],
-        "PermissionsBoundaryPolicyInputList": Sequence[str],
-        "ResourceArns": Sequence[str],
-        "ResourcePolicy": str,
-        "ResourceOwner": str,
-        "CallerArn": str,
-        "ContextEntries": Sequence[ContextEntryTypeDef],
-        "ResourceHandlingOption": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
-    _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-):
-    pass
-
-
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsForUserResponseTypeDef = TypedDict(
     "ListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
@@ -4042,22 +3317,20 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateInstanceProfileRequestRequestTypeDef(
     _RequiredCreateInstanceProfileRequestRequestTypeDef,
     _OptionalCreateInstanceProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     {
         "InstanceProfileName": str,
     },
 )
 _OptionalCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef = TypedDict(
@@ -4065,22 +3338,20 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef(
     _RequiredCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     _OptionalCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
 ):
     pass
 
-
 _RequiredCreateOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpenIDConnectProviderRequestRequestTypeDef",
     {
         "Url": str,
         "ThumbprintList": Sequence[str],
     },
 )
@@ -4089,28 +3360,26 @@
     {
         "ClientIDList": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpenIDConnectProviderRequestRequestTypeDef(
     _RequiredCreateOpenIDConnectProviderRequestRequestTypeDef,
     _OptionalCreateOpenIDConnectProviderRequestRequestTypeDef,
 ):
     pass
 
-
 CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
     "CreateOpenIDConnectProviderResponseTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
@@ -4123,21 +3392,19 @@
         "Path": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePolicyRequestRequestTypeDef(
     _RequiredCreatePolicyRequestRequestTypeDef, _OptionalCreatePolicyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreatePolicyRequestServiceResourceCreatePolicyTypeDef = TypedDict(
     "_RequiredCreatePolicyRequestServiceResourceCreatePolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -4147,22 +3414,20 @@
         "Path": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePolicyRequestServiceResourceCreatePolicyTypeDef(
     _RequiredCreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     _OptionalCreatePolicyRequestServiceResourceCreatePolicyTypeDef,
 ):
     pass
 
-
 _RequiredCreateRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRoleRequestRequestTypeDef",
     {
         "RoleName": str,
         "AssumeRolePolicyDocument": str,
     },
 )
@@ -4174,21 +3439,19 @@
         "MaxSessionDuration": int,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRoleRequestRequestTypeDef(
     _RequiredCreateRoleRequestRequestTypeDef, _OptionalCreateRoleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateRoleRequestServiceResourceCreateRoleTypeDef = TypedDict(
     "_RequiredCreateRoleRequestServiceResourceCreateRoleTypeDef",
     {
         "RoleName": str,
         "AssumeRolePolicyDocument": str,
     },
 )
@@ -4200,22 +3463,20 @@
         "MaxSessionDuration": int,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRoleRequestServiceResourceCreateRoleTypeDef(
     _RequiredCreateRoleRequestServiceResourceCreateRoleTypeDef,
     _OptionalCreateRoleRequestServiceResourceCreateRoleTypeDef,
 ):
     pass
 
-
 _RequiredCreateSAMLProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSAMLProviderRequestRequestTypeDef",
     {
         "SAMLMetadataDocument": str,
         "Name": str,
     },
 )
@@ -4223,22 +3484,20 @@
     "_OptionalCreateSAMLProviderRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSAMLProviderRequestRequestTypeDef(
     _RequiredCreateSAMLProviderRequestRequestTypeDef,
     _OptionalCreateSAMLProviderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef = TypedDict(
     "_RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef",
     {
         "SAMLMetadataDocument": str,
         "Name": str,
     },
 )
@@ -4246,28 +3505,26 @@
     "_OptionalCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef(
     _RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
     _OptionalCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
 ):
     pass
 
-
 CreateSAMLProviderResponseTypeDef = TypedDict(
     "CreateSAMLProviderResponseTypeDef",
     {
         "SAMLProviderArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
@@ -4279,21 +3536,19 @@
         "Path": str,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateUserRequestServiceResourceCreateUserTypeDef = TypedDict(
     "_RequiredCreateUserRequestServiceResourceCreateUserTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalCreateUserRequestServiceResourceCreateUserTypeDef = TypedDict(
@@ -4302,22 +3557,20 @@
         "Path": str,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserRequestServiceResourceCreateUserTypeDef(
     _RequiredCreateUserRequestServiceResourceCreateUserTypeDef,
     _OptionalCreateUserRequestServiceResourceCreateUserTypeDef,
 ):
     pass
 
-
 CreateUserRequestUserCreateTypeDef = TypedDict(
     "CreateUserRequestUserCreateTypeDef",
     {
         "Path": str,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -4335,22 +3588,20 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualMFADeviceRequestRequestTypeDef(
     _RequiredCreateVirtualMFADeviceRequestRequestTypeDef,
     _OptionalCreateVirtualMFADeviceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef = TypedDict(
     "_RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef",
     {
         "VirtualMFADeviceName": str,
     },
 )
 _OptionalCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef = TypedDict(
@@ -4358,122 +3609,120 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef(
     _RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
     _OptionalCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
 ):
     pass
 
-
 GetOpenIDConnectProviderResponseTypeDef = TypedDict(
     "GetOpenIDConnectProviderResponseTypeDef",
     {
         "Url": str,
         "ClientIDList": List[str],
         "ThumbprintList": List[str],
         "CreateDate": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSAMLProviderResponseTypeDef = TypedDict(
     "GetSAMLProviderResponseTypeDef",
     {
         "SAMLMetadataDocument": str,
         "CreateDate": datetime,
         "ValidUntil": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfileTagsResponseTypeDef = TypedDict(
     "ListInstanceProfileTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMFADeviceTagsResponseTypeDef = TypedDict(
     "ListMFADeviceTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpenIDConnectProviderTagsResponseTypeDef = TypedDict(
     "ListOpenIDConnectProviderTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyTagsResponseTypeDef = TypedDict(
     "ListPolicyTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoleTagsResponseTypeDef = TypedDict(
     "ListRoleTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSAMLProviderTagsResponseTypeDef = TypedDict(
     "ListSAMLProviderTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServerCertificateTagsResponseTypeDef = TypedDict(
     "ListServerCertificateTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserTagsResponseTypeDef = TypedDict(
     "ListUserTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyTypeDef = TypedDict(
     "PolicyTypeDef",
     {
         "PolicyName": str,
@@ -4570,22 +3819,20 @@
         "Path": str,
         "CertificateChain": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UploadServerCertificateRequestRequestTypeDef(
     _RequiredUploadServerCertificateRequestRequestTypeDef,
     _OptionalUploadServerCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef = TypedDict(
     "_RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
     {
         "ServerCertificateName": str,
         "CertificateBody": str,
         "PrivateKey": str,
     },
@@ -4596,34 +3843,32 @@
         "Path": str,
         "CertificateChain": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
-
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "Path": str,
@@ -4639,93 +3884,46 @@
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoginProfileResponseTypeDef = TypedDict(
     "GetLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
-    {
-        "PolicyVersion": PolicyVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
-    {
-        "PolicyVersion": PolicyVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyVersionsResponseTypeDef = TypedDict(
-    "ListPolicyVersionsResponseTypeDef",
-    {
-        "Versions": List[PolicyVersionTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ManagedPolicyDetailTypeDef = TypedDict(
-    "ManagedPolicyDetailTypeDef",
-    {
-        "PolicyName": str,
-        "PolicyId": str,
-        "Arn": str,
-        "Path": str,
-        "DefaultVersionId": str,
-        "AttachmentCount": int,
-        "PermissionsBoundaryUsageCount": int,
-        "IsAttachable": bool,
-        "Description": str,
-        "CreateDate": datetime,
-        "UpdateDate": datetime,
-        "PolicyVersionList": List[PolicyVersionTypeDef],
-    },
-    total=False,
-)
-
 CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
     "CreateServiceSpecificCredentialResponseTypeDef",
     {
         "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetServiceSpecificCredentialResponseTypeDef = TypedDict(
     "ResetServiceSpecificCredentialResponseTypeDef",
     {
         "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletionTaskFailureReasonTypeTypeDef = TypedDict(
     "DeletionTaskFailureReasonTypeTypeDef",
     {
         "Reason": str,
@@ -4744,40 +3942,603 @@
     "_OptionalEntityDetailsTypeDef",
     {
         "LastAuthenticated": datetime,
     },
     total=False,
 )
 
-
 class EntityDetailsTypeDef(_RequiredEntityDetailsTypeDef, _OptionalEntityDetailsTypeDef):
     pass
 
-
 GetOrganizationsAccessReportResponseTypeDef = TypedDict(
     "GetOrganizationsAccessReportResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
         "NumberOfServicesNotAccessed": int,
         "AccessDetails": List[AccessDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ErrorDetails": ErrorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef = TypedDict(
+    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+    {
+        "Filter": Sequence[EntityTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
+    "_RequiredGetGroupRequestGetGroupPaginateTypeDef",
+    {
+        "GroupName": str,
+    },
+)
+_OptionalGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
+    "_OptionalGetGroupRequestGetGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetGroupRequestGetGroupPaginateTypeDef(
+    _RequiredGetGroupRequestGetGroupPaginateTypeDef, _OptionalGetGroupRequestGetGroupPaginateTypeDef
+):
+    pass
+
+ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
+    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAccountAliasesRequestListAccountAliasesPaginateTypeDef = TypedDict(
+    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
+    {
+        "GroupName": str,
+    },
+)
+_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef(
+    _RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+    _OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef(
+    _RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+    _OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef(
+    _RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+    _OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
+    "_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
+    "_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
+    {
+        "EntityFilter": EntityTypeType,
+        "PathPrefix": str,
+        "PolicyUsageFilter": PolicyUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef(
+    _RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+    _OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
+    {
+        "GroupName": str,
+    },
+)
+_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef(
+    _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+    _OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupsForUserRequestListGroupsForUserPaginateTypeDef(
+    _RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+    _OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
+    {
+        "InstanceProfileName": str,
+    },
+)
+_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef(
+    _RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+    _OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
+    "_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
+    "_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef(
+    _RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+    _OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+):
+    pass
+
+ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
+    "_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
+    {
+        "SerialNumber": str,
+    },
+)
+_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
+    "_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef(
+    _RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+    _OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+):
+    pass
+
+ListMFADevicesRequestListMFADevicesPaginateTypeDef = TypedDict(
+    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
+        {
+            "OpenIDConnectProviderArn": str,
+        },
+    )
+)
+_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef(
+    _RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+    _OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+):
+    pass
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "Scope": policyScopeTypeType,
+        "OnlyAttached": bool,
+        "PathPrefix": str,
+        "PolicyUsageFilter": PolicyUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyTagsRequestListPolicyTagsPaginateTypeDef(
+    _RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+    _OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef(
+    _RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+    _OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRolePoliciesRequestListRolePoliciesPaginateTypeDef(
+    _RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+    _OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
+    "_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
+    "_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRoleTagsRequestListRoleTagsPaginateTypeDef(
+    _RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef,
+    _OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef,
+):
+    pass
+
+ListRolesRequestListRolesPaginateTypeDef = TypedDict(
+    "ListRolesRequestListRolesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
+    "_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
+    {
+        "SAMLProviderArn": str,
+    },
+)
+_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
+    "_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef(
+    _RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+    _OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+):
+    pass
+
+ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = TypedDict(
+    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
+    "_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
+    {
+        "ServerCertificateName": str,
+    },
+)
+_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
+    "_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef(
+    _RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+    _OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+):
+    pass
+
+ListServerCertificatesRequestListServerCertificatesPaginateTypeDef = TypedDict(
+    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef = TypedDict(
+    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUserPoliciesRequestListUserPoliciesPaginateTypeDef(
+    _RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+    _OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
+    "_RequiredListUserTagsRequestListUserTagsPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
+    "_OptionalListUserTagsRequestListUserTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUserTagsRequestListUserTagsPaginateTypeDef(
+    _RequiredListUserTagsRequestListUserTagsPaginateTypeDef,
+    _OptionalListUserTagsRequestListUserTagsPaginateTypeDef,
+):
+    pass
+
+ListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "ListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef = TypedDict(
+    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
+    {
+        "AssignmentStatus": assignmentStatusTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
+    "_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
+    {
+        "PolicyInputList": Sequence[str],
+        "ActionNames": Sequence[str],
+    },
+)
+_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
+    "_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
+    {
+        "PermissionsBoundaryPolicyInputList": Sequence[str],
+        "ResourceArns": Sequence[str],
+        "ResourcePolicy": str,
+        "ResourceOwner": str,
+        "CallerArn": str,
+        "ContextEntries": Sequence[ContextEntryTypeDef],
+        "ResourceHandlingOption": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef(
+    _RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+    _OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+):
+    pass
+
+_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
+    "_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
+    {
+        "PolicySourceArn": str,
+        "ActionNames": Sequence[str],
+    },
+)
+_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
+    "_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
+    {
+        "PolicyInputList": Sequence[str],
+        "PermissionsBoundaryPolicyInputList": Sequence[str],
+        "ResourceArns": Sequence[str],
+        "ResourcePolicy": str,
+        "ResourceOwner": str,
+        "CallerArn": str,
+        "ContextEntries": Sequence[ContextEntryTypeDef],
+        "ResourceHandlingOption": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
+    _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
+    _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
+):
+    pass
+
 GetAccountPasswordPolicyResponseTypeDef = TypedDict(
     "GetAccountPasswordPolicyResponseTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = TypedDict(
     "_RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
         "InstanceProfileName": str,
@@ -4787,87 +4548,81 @@
     "_OptionalGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef(
     _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     _OptionalGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetPolicyRequestPolicyExistsWaitTypeDef = TypedDict(
     "_RequiredGetPolicyRequestPolicyExistsWaitTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalGetPolicyRequestPolicyExistsWaitTypeDef = TypedDict(
     "_OptionalGetPolicyRequestPolicyExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPolicyRequestPolicyExistsWaitTypeDef(
     _RequiredGetPolicyRequestPolicyExistsWaitTypeDef,
     _OptionalGetPolicyRequestPolicyExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetRoleRequestRoleExistsWaitTypeDef = TypedDict(
     "_RequiredGetRoleRequestRoleExistsWaitTypeDef",
     {
         "RoleName": str,
     },
 )
 _OptionalGetRoleRequestRoleExistsWaitTypeDef = TypedDict(
     "_OptionalGetRoleRequestRoleExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetRoleRequestRoleExistsWaitTypeDef(
     _RequiredGetRoleRequestRoleExistsWaitTypeDef, _OptionalGetRoleRequestRoleExistsWaitTypeDef
 ):
     pass
 
-
 GetUserRequestUserExistsWaitTypeDef = TypedDict(
     "GetUserRequestUserExistsWaitTypeDef",
     {
         "UserName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 GetSSHPublicKeyResponseTypeDef = TypedDict(
     "GetSSHPublicKeyResponseTypeDef",
     {
         "SSHPublicKey": SSHPublicKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadSSHPublicKeyResponseTypeDef = TypedDict(
     "UploadSSHPublicKeyResponseTypeDef",
     {
         "SSHPublicKey": SSHPublicKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupDetailTypeDef = TypedDict(
     "GroupDetailTypeDef",
     {
         "Path": str,
@@ -4902,33 +4657,33 @@
     "ListEntitiesForPolicyResponseTypeDef",
     {
         "PolicyGroups": List[PolicyGroupTypeDef],
         "PolicyUsers": List[PolicyUserTypeDef],
         "PolicyRoles": List[PolicyRoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMFADevicesResponseTypeDef = TypedDict(
     "ListMFADevicesResponseTypeDef",
     {
         "MFADevices": List[MFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpenIDConnectProvidersResponseTypeDef = TypedDict(
     "ListOpenIDConnectProvidersResponseTypeDef",
     {
         "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
     "ListPoliciesGrantingServiceAccessEntryTypeDef",
     {
         "ServiceNamespace": str,
@@ -4937,35 +4692,35 @@
     total=False,
 )
 
 ListSAMLProvidersResponseTypeDef = TypedDict(
     "ListSAMLProvidersResponseTypeDef",
     {
         "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSSHPublicKeysResponseTypeDef = TypedDict(
     "ListSSHPublicKeysResponseTypeDef",
     {
         "SSHPublicKeys": List[SSHPublicKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServerCertificatesResponseTypeDef = TypedDict(
     "ListServerCertificatesResponseTypeDef",
     {
         "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredServerCertificateTypeDef = TypedDict(
     "_RequiredServerCertificateTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
@@ -4977,53 +4732,59 @@
     {
         "CertificateChain": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class ServerCertificateTypeDef(
     _RequiredServerCertificateTypeDef, _OptionalServerCertificateTypeDef
 ):
     pass
 
-
 UploadServerCertificateResponseTypeDef = TypedDict(
     "UploadServerCertificateResponseTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceSpecificCredentialsResponseTypeDef = TypedDict(
     "ListServiceSpecificCredentialsResponseTypeDef",
     {
         "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSigningCertificatesResponseTypeDef = TypedDict(
     "ListSigningCertificatesResponseTypeDef",
     {
         "Certificates": List[SigningCertificateTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadSigningCertificateResponseTypeDef = TypedDict(
     "UploadSigningCertificateResponseTypeDef",
     {
         "Certificate": SigningCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PolicyDocumentFixedTypeDef = TypedDict(
+    "PolicyDocumentFixedTypeDef",
+    {
+        "Version": str,
+        "Statement": List[PolicyDocumentStatementTypeDef],
     },
 )
 
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
     {
         "SourcePolicyId": str,
@@ -5053,19 +4814,17 @@
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
     total=False,
 )
 
-
 class RoleTypeDef(_RequiredRoleTypeDef, _OptionalRoleTypeDef):
     pass
 
-
 _RequiredServiceLastAccessedTypeDef = TypedDict(
     "_RequiredServiceLastAccessedTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
     },
 )
@@ -5077,81 +4836,79 @@
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
         "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
     },
     total=False,
 )
 
-
 class ServiceLastAccessedTypeDef(
     _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
 ):
     pass
 
-
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
         "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVirtualMFADeviceTypeDef = TypedDict(
     "_RequiredVirtualMFADeviceTypeDef",
     {
         "SerialNumber": str,
@@ -5165,60 +4922,69 @@
         "User": UserTypeDef,
         "EnableDate": datetime,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
     pass
 
-
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef = TypedDict(
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "EntityDetailsList": List[EntityDetailsTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "Error": ErrorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesGrantingServiceAccessResponseTypeDef = TypedDict(
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     {
         "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServerCertificateResponseTypeDef = TypedDict(
     "GetServerCertificateResponseTypeDef",
     {
         "ServerCertificate": ServerCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PolicyVersionTypeDef = TypedDict(
+    "PolicyVersionTypeDef",
+    {
+        "Document": PolicyDocumentFixedTypeDef,
+        "VersionId": str,
+        "IsDefaultVersion": bool,
+        "CreateDate": datetime,
+    },
+    total=False,
+)
+
 _RequiredResourceSpecificResultTypeDef = TypedDict(
     "_RequiredResourceSpecificResultTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
     },
 )
@@ -5229,42 +4995,40 @@
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
     },
     total=False,
 )
 
-
 class ResourceSpecificResultTypeDef(
     _RequiredResourceSpecificResultTypeDef, _OptionalResourceSpecificResultTypeDef
 ):
     pass
 
-
 CreateRoleResponseTypeDef = TypedDict(
     "CreateRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceLinkedRoleResponseTypeDef = TypedDict(
     "CreateServiceLinkedRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoleResponseTypeDef = TypedDict(
     "GetRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInstanceProfileTypeDef = TypedDict(
     "_RequiredInstanceProfileTypeDef",
     {
         "Path": str,
@@ -5279,70 +5043,113 @@
     "_OptionalInstanceProfileTypeDef",
     {
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class InstanceProfileTypeDef(_RequiredInstanceProfileTypeDef, _OptionalInstanceProfileTypeDef):
     pass
 
-
 ListRolesResponseTypeDef = TypedDict(
     "ListRolesResponseTypeDef",
     {
         "Roles": List[RoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoleDescriptionResponseTypeDef = TypedDict(
     "UpdateRoleDescriptionResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
     "GetServiceLastAccessedDetailsResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobType": AccessAdvisorUsageGranularityTypeType,
         "JobCreationDate": datetime,
         "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
         "Error": ErrorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVirtualMFADeviceResponseTypeDef = TypedDict(
     "CreateVirtualMFADeviceResponseTypeDef",
     {
         "VirtualMFADevice": VirtualMFADeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualMFADevicesResponseTypeDef = TypedDict(
     "ListVirtualMFADevicesResponseTypeDef",
     {
         "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
+    {
+        "PolicyVersion": PolicyVersionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
+    {
+        "PolicyVersion": PolicyVersionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyVersionsResponseTypeDef = TypedDict(
+    "ListPolicyVersionsResponseTypeDef",
+    {
+        "Versions": List[PolicyVersionTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ManagedPolicyDetailTypeDef = TypedDict(
+    "ManagedPolicyDetailTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyId": str,
+        "Arn": str,
+        "Path": str,
+        "DefaultVersionId": str,
+        "AttachmentCount": int,
+        "PermissionsBoundaryUsageCount": int,
+        "IsAttachable": bool,
+        "Description": str,
+        "CreateDate": datetime,
+        "UpdateDate": datetime,
+        "PolicyVersionList": List[PolicyVersionTypeDef],
+    },
+    total=False,
+)
+
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "EvalActionName": str,
         "EvalDecision": PolicyEvaluationDecisionTypeType,
     },
 )
@@ -5356,52 +5163,50 @@
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
     },
     total=False,
 )
 
-
 class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
     pass
 
-
 CreateInstanceProfileResponseTypeDef = TypedDict(
     "CreateInstanceProfileResponseTypeDef",
     {
         "InstanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceProfileResponseTypeDef = TypedDict(
     "GetInstanceProfileResponseTypeDef",
     {
         "InstanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfilesForRoleResponseTypeDef = TypedDict(
     "ListInstanceProfilesForRoleResponseTypeDef",
     {
         "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfilesResponseTypeDef = TypedDict(
     "ListInstanceProfilesResponseTypeDef",
     {
         "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RoleDetailTypeDef = TypedDict(
     "RoleDetailTypeDef",
     {
         "Path": str,
@@ -5422,23 +5227,23 @@
 
 SimulatePolicyResponseTypeDef = TypedDict(
     "SimulatePolicyResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountAuthorizationDetailsResponseTypeDef = TypedDict(
     "GetAccountAuthorizationDetailsResponseTypeDef",
     {
         "UserDetailList": List[UserDetailTypeDef],
         "GroupDetailList": List[GroupDetailTypeDef],
         "RoleDetailList": List[RoleDetailTypeDef],
         "Policies": List[ManagedPolicyDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/type_defs.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iam.type_defs import AccessDetailTypeDef
 
-    data: AccessDetailTypeDef = {...}
+    data: AccessDetailTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccessAdvisorUsageGranularityTypeType,
     ContextKeyTypeEnumType,
     DeletionTaskStatusTypeType,
     EntityTypeType,
     PolicyEvaluationDecisionTypeType,
@@ -41,14 +41,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessDetailTypeDef",
     "AccessKeyLastUsedTypeDef",
     "AccessKeyMetadataTypeDef",
     "AccessKeyTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
@@ -61,15 +62,15 @@
     "AttachGroupPolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachedPermissionsBoundaryTypeDef",
     "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
@@ -81,15 +82,14 @@
     "TagTypeDef",
     "CreateLoginProfileRequestLoginProfileCreateTypeDef",
     "CreateLoginProfileRequestRequestTypeDef",
     "CreateLoginProfileRequestUserCreateLoginProfileTypeDef",
     "LoginProfileTypeDef",
     "CreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "PolicyVersionTypeDef",
     "CreateServiceLinkedRoleRequestRequestTypeDef",
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     "ServiceSpecificCredentialTypeDef",
     "DeactivateMFADeviceRequestRequestTypeDef",
     "DeleteAccessKeyRequestRequestTypeDef",
     "DeleteAccountAliasRequestRequestTypeDef",
     "DeleteGroupPolicyRequestRequestTypeDef",
@@ -102,15 +102,14 @@
     "DeleteRolePermissionsBoundaryRequestRequestTypeDef",
     "DeleteRolePolicyRequestRequestTypeDef",
     "DeleteRoleRequestRequestTypeDef",
     "DeleteSAMLProviderRequestRequestTypeDef",
     "DeleteSSHPublicKeyRequestRequestTypeDef",
     "DeleteServerCertificateRequestRequestTypeDef",
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
-    "DeleteServiceLinkedRoleResponseTypeDef",
     "DeleteServiceSpecificCredentialRequestRequestTypeDef",
     "DeleteSigningCertificateRequestRequestTypeDef",
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     "DeleteUserPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
     "RoleUsageTypeTypeDef",
@@ -119,141 +118,95 @@
     "DetachGroupPolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestPolicyDetachRoleTypeDef",
     "DetachRolePolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestRoleDetachPolicyTypeDef",
     "DetachUserPolicyRequestPolicyDetachUserTypeDef",
     "DetachUserPolicyRequestRequestTypeDef",
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     "EnableMFADeviceRequestRequestTypeDef",
     "EnableMFADeviceRequestUserEnableMfaTypeDef",
     "EntityInfoTypeDef",
     "ErrorDetailsTypeDef",
     "OrganizationsDecisionDetailTypeDef",
     "PermissionsBoundaryDecisionDetailTypeDef",
-    "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportRequestRequestTypeDef",
-    "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsRequestRequestTypeDef",
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedRequestRequestTypeDef",
-    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
     "PasswordPolicyTypeDef",
-    "GetAccountSummaryResponseTypeDef",
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
-    "GetContextKeysForPolicyResponseTypeDef",
     "GetContextKeysForPrincipalPolicyRequestRequestTypeDef",
-    "GetCredentialReportResponseTypeDef",
     "GetGroupPolicyRequestRequestTypeDef",
-    "GetGroupPolicyResponseTypeDef",
-    "GetGroupRequestGetGroupPaginateTypeDef",
     "GetGroupRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetLoginProfileRequestRequestTypeDef",
     "GetMFADeviceRequestRequestTypeDef",
-    "GetMFADeviceResponseTypeDef",
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     "GetOrganizationsAccessReportRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
     "GetRolePolicyRequestRequestTypeDef",
-    "GetRolePolicyResponseTypeDef",
     "GetRoleRequestRequestTypeDef",
     "GetSAMLProviderRequestRequestTypeDef",
     "GetSSHPublicKeyRequestRequestTypeDef",
     "SSHPublicKeyTypeDef",
     "GetServerCertificateRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     "GetUserPolicyRequestRequestTypeDef",
-    "GetUserPolicyResponseTypeDef",
     "GetUserRequestRequestTypeDef",
     "PolicyDetailTypeDef",
-    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     "ListAccessKeysRequestRequestTypeDef",
-    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
     "ListAccountAliasesRequestRequestTypeDef",
-    "ListAccountAliasesResponseTypeDef",
-    "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
     "ListAttachedGroupPoliciesRequestRequestTypeDef",
-    "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
     "ListAttachedRolePoliciesRequestRequestTypeDef",
-    "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
     "ListAttachedUserPoliciesRequestRequestTypeDef",
-    "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
     "ListEntitiesForPolicyRequestRequestTypeDef",
     "PolicyGroupTypeDef",
     "PolicyRoleTypeDef",
     "PolicyUserTypeDef",
-    "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     "ListGroupPoliciesRequestRequestTypeDef",
-    "ListGroupPoliciesResponseTypeDef",
-    "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
     "ListGroupsForUserRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
     "ListInstanceProfileTagsRequestRequestTypeDef",
-    "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
     "ListInstanceProfilesForRoleRequestRequestTypeDef",
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
-    "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
     "ListMFADeviceTagsRequestRequestTypeDef",
-    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
     "ListMFADevicesRequestRequestTypeDef",
     "MFADeviceTypeDef",
-    "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
     "ListOpenIDConnectProviderTagsRequestRequestTypeDef",
     "OpenIDConnectProviderListEntryTypeDef",
     "PolicyGrantingServiceAccessTypeDef",
     "ListPoliciesGrantingServiceAccessRequestRequestTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
-    "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
     "ListPolicyTagsRequestRequestTypeDef",
-    "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
-    "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
     "ListRolePoliciesRequestRequestTypeDef",
-    "ListRolePoliciesResponseTypeDef",
-    "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
     "ListRoleTagsRequestRequestTypeDef",
-    "ListRolesRequestListRolesPaginateTypeDef",
     "ListRolesRequestRequestTypeDef",
-    "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
     "ListSAMLProviderTagsRequestRequestTypeDef",
     "SAMLProviderListEntryTypeDef",
-    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     "ListSSHPublicKeysRequestRequestTypeDef",
     "SSHPublicKeyMetadataTypeDef",
-    "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
     "ListServerCertificateTagsRequestRequestTypeDef",
-    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
     "ListServerCertificatesRequestRequestTypeDef",
     "ServerCertificateMetadataTypeDef",
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
     "ServiceSpecificCredentialMetadataTypeDef",
-    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
     "ListSigningCertificatesRequestRequestTypeDef",
     "SigningCertificateTypeDef",
-    "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     "ListUserPoliciesRequestRequestTypeDef",
-    "ListUserPoliciesResponseTypeDef",
-    "ListUserTagsRequestListUserTagsPaginateTypeDef",
     "ListUserTagsRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
     "ListVirtualMFADevicesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "PolicyDocumentStatementTypeDef",
     "PositionTypeDef",
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     "PutGroupPolicyRequestGroupPolicyPutTypeDef",
     "PutGroupPolicyRequestRequestTypeDef",
     "PutRolePermissionsBoundaryRequestRequestTypeDef",
     "PutRolePolicyRequestRequestTypeDef",
     "PutRolePolicyRequestRolePolicyPutTypeDef",
@@ -264,20 +217,17 @@
     "RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef",
     "RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef",
     "RemoveRoleFromInstanceProfileRequestRequestTypeDef",
     "RemoveUserFromGroupRequestGroupRemoveUserTypeDef",
     "RemoveUserFromGroupRequestRequestTypeDef",
     "RemoveUserFromGroupRequestUserRemoveGroupTypeDef",
     "ResetServiceSpecificCredentialRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     "ResyncMFADeviceRequestRequestTypeDef",
     "RoleLastUsedTypeDef",
-    "RoleLastUsedResponseMetadataTypeDef",
-    "ServerCertificateMetadataResponseMetadataTypeDef",
     "TrackedActionLastAccessedTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetSecurityTokenServicePreferencesRequestRequestTypeDef",
     "UntagInstanceProfileRequestRequestTypeDef",
     "UntagMFADeviceRequestRequestTypeDef",
     "UntagOpenIDConnectProviderRequestRequestTypeDef",
     "UntagPolicyRequestRequestTypeDef",
@@ -300,37 +250,54 @@
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     "UpdateLoginProfileRequestRequestTypeDef",
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     "UpdateRoleDescriptionRequestRequestTypeDef",
     "UpdateRoleRequestRequestTypeDef",
     "UpdateSAMLProviderRequestRequestTypeDef",
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
-    "UpdateSAMLProviderResponseTypeDef",
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     "UpdateServerCertificateRequestRequestTypeDef",
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     "UpdateServiceSpecificCredentialRequestRequestTypeDef",
     "UpdateSigningCertificateRequestRequestTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
+    "AttachedPermissionsBoundaryResponseTypeDef",
+    "CreateAccessKeyResponseTypeDef",
+    "DeleteServiceLinkedRoleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GenerateCredentialReportResponseTypeDef",
+    "GenerateOrganizationsAccessReportResponseTypeDef",
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedResponseTypeDef",
+    "GetAccountSummaryResponseTypeDef",
+    "GetContextKeysForPolicyResponseTypeDef",
+    "GetCredentialReportResponseTypeDef",
+    "GetGroupPolicyResponseTypeDef",
+    "GetMFADeviceResponseTypeDef",
+    "GetRolePolicyResponseTypeDef",
+    "GetUserPolicyResponseTypeDef",
     "ListAccessKeysResponseTypeDef",
-    "CreateAccessKeyResponseTypeDef",
+    "ListAccountAliasesResponseTypeDef",
+    "ListGroupPoliciesResponseTypeDef",
+    "ListRolePoliciesResponseTypeDef",
+    "ListUserPoliciesResponseTypeDef",
+    "RoleLastUsedResponseTypeDef",
+    "ServerCertificateMetadataResponseTypeDef",
+    "UpdateSAMLProviderResponseTypeDef",
     "ListAttachedGroupPoliciesResponseTypeDef",
     "ListAttachedRolePoliciesResponseTypeDef",
     "ListAttachedUserPoliciesResponseTypeDef",
     "SimulateCustomPolicyRequestRequestTypeDef",
-    "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
     "SimulatePrincipalPolicyRequestRequestTypeDef",
-    "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
     "CreateGroupResponseTypeDef",
     "ListGroupsForUserResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
     "CreateOpenIDConnectProviderResponseTypeDef",
@@ -363,27 +330,57 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
-    "UserResponseMetadataTypeDef",
+    "UserResponseTypeDef",
     "UserTypeDef",
     "CreateLoginProfileResponseTypeDef",
     "GetLoginProfileResponseTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "ListPolicyVersionsResponseTypeDef",
-    "ManagedPolicyDetailTypeDef",
     "CreateServiceSpecificCredentialResponseTypeDef",
     "ResetServiceSpecificCredentialResponseTypeDef",
     "DeletionTaskFailureReasonTypeTypeDef",
     "EntityDetailsTypeDef",
     "GetOrganizationsAccessReportResponseTypeDef",
+    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+    "GetGroupRequestGetGroupPaginateTypeDef",
+    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
+    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
+    "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
+    "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
+    "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
+    "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
+    "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
+    "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
+    "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
+    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
+    "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
+    "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
+    "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
+    "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
+    "ListRolesRequestListRolesPaginateTypeDef",
+    "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
+    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
+    "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
+    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
+    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
+    "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
+    "ListUserTagsRequestListUserTagsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
+    "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
+    "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
     "GetAccountPasswordPolicyResponseTypeDef",
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
     "GetSSHPublicKeyResponseTypeDef",
     "UploadSSHPublicKeyResponseTypeDef",
@@ -397,14 +394,15 @@
     "ListSSHPublicKeysResponseTypeDef",
     "ListServerCertificatesResponseTypeDef",
     "ServerCertificateTypeDef",
     "UploadServerCertificateResponseTypeDef",
     "ListServiceSpecificCredentialsResponseTypeDef",
     "ListSigningCertificatesResponseTypeDef",
     "UploadSigningCertificateResponseTypeDef",
+    "PolicyDocumentFixedTypeDef",
     "StatementTypeDef",
     "RoleTypeDef",
     "ServiceLastAccessedTypeDef",
     "CreatePolicyResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "CreateUserResponseTypeDef",
@@ -412,24 +410,29 @@
     "GetUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "VirtualMFADeviceTypeDef",
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     "GetServerCertificateResponseTypeDef",
+    "PolicyVersionTypeDef",
     "ResourceSpecificResultTypeDef",
     "CreateRoleResponseTypeDef",
     "CreateServiceLinkedRoleResponseTypeDef",
     "GetRoleResponseTypeDef",
     "InstanceProfileTypeDef",
     "ListRolesResponseTypeDef",
     "UpdateRoleDescriptionResponseTypeDef",
     "GetServiceLastAccessedDetailsResponseTypeDef",
     "CreateVirtualMFADeviceResponseTypeDef",
     "ListVirtualMFADevicesResponseTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "ListPolicyVersionsResponseTypeDef",
+    "ManagedPolicyDetailTypeDef",
     "EvaluationResultTypeDef",
     "CreateInstanceProfileResponseTypeDef",
     "GetInstanceProfileResponseTypeDef",
     "ListInstanceProfilesForRoleResponseTypeDef",
     "ListInstanceProfilesResponseTypeDef",
     "RoleDetailTypeDef",
     "SimulatePolicyResponseTypeDef",
@@ -450,17 +453,19 @@
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
     total=False,
 )
 
+
 class AccessDetailTypeDef(_RequiredAccessDetailTypeDef, _OptionalAccessDetailTypeDef):
     pass
 
+
 AccessKeyLastUsedTypeDef = TypedDict(
     "AccessKeyLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
@@ -490,17 +495,19 @@
     "_OptionalAccessKeyTypeDef",
     {
         "CreateDate": datetime,
     },
     total=False,
 )
 
+
 class AccessKeyTypeDef(_RequiredAccessKeyTypeDef, _OptionalAccessKeyTypeDef):
     pass
 
+
 AddClientIDToOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "ClientID": str,
     },
 )
@@ -604,20 +611,22 @@
 AttachUserPolicyRequestUserAttachPolicyTypeDef = TypedDict(
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
-        "PermissionsBoundaryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AttachedPermissionsBoundaryTypeDef = TypedDict(
     "AttachedPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
@@ -701,39 +710,43 @@
     "_OptionalCreateGroupRequestRequestTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef = TypedDict(
     "_RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef = TypedDict(
     "_OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
+
 class CreateGroupRequestServiceResourceCreateGroupTypeDef(
     _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef,
     _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef,
 ):
     pass
 
+
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
@@ -759,20 +772,22 @@
     "_OptionalCreateLoginProfileRequestLoginProfileCreateTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
+
 class CreateLoginProfileRequestLoginProfileCreateTypeDef(
     _RequiredCreateLoginProfileRequestLoginProfileCreateTypeDef,
     _OptionalCreateLoginProfileRequestLoginProfileCreateTypeDef,
 ):
     pass
 
+
 _RequiredCreateLoginProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLoginProfileRequestRequestTypeDef",
     {
         "UserName": str,
         "Password": str,
     },
 )
@@ -780,40 +795,44 @@
     "_OptionalCreateLoginProfileRequestRequestTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
+
 class CreateLoginProfileRequestRequestTypeDef(
     _RequiredCreateLoginProfileRequestRequestTypeDef,
     _OptionalCreateLoginProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef = TypedDict(
     "_RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef",
     {
         "Password": str,
     },
 )
 _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef = TypedDict(
     "_OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
+
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
+
 _RequiredLoginProfileTypeDef = TypedDict(
     "_RequiredLoginProfileTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
     },
 )
@@ -821,37 +840,41 @@
     "_OptionalLoginProfileTypeDef",
     {
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
+
 class LoginProfileTypeDef(_RequiredLoginProfileTypeDef, _OptionalLoginProfileTypeDef):
     pass
 
+
 _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "PolicyDocument": str,
     },
 )
 _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef = TypedDict(
     "_OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     {
         "SetAsDefault": bool,
     },
     total=False,
 )
 
+
 class CreatePolicyVersionRequestPolicyCreateVersionTypeDef(
     _RequiredCreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     _OptionalCreatePolicyVersionRequestPolicyCreateVersionTypeDef,
 ):
     pass
 
+
 _RequiredCreatePolicyVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestRequestTypeDef",
     {
         "PolicyArn": str,
         "PolicyDocument": str,
     },
 )
@@ -859,30 +882,21 @@
     "_OptionalCreatePolicyVersionRequestRequestTypeDef",
     {
         "SetAsDefault": bool,
     },
     total=False,
 )
 
+
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
-PolicyVersionTypeDef = TypedDict(
-    "PolicyVersionTypeDef",
-    {
-        "Document": str,
-        "VersionId": str,
-        "IsDefaultVersion": bool,
-        "CreateDate": datetime,
-    },
-    total=False,
-)
 
 _RequiredCreateServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceLinkedRoleRequestRequestTypeDef",
     {
         "AWSServiceName": str,
     },
 )
@@ -891,20 +905,22 @@
     {
         "Description": str,
         "CustomSuffix": str,
     },
     total=False,
 )
 
+
 class CreateServiceLinkedRoleRequestRequestTypeDef(
     _RequiredCreateServiceLinkedRoleRequestRequestTypeDef,
     _OptionalCreateServiceLinkedRoleRequestRequestTypeDef,
 ):
     pass
 
+
 CreateServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
 )
@@ -940,19 +956,21 @@
     "_OptionalDeleteAccessKeyRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class DeleteAccessKeyRequestRequestTypeDef(
     _RequiredDeleteAccessKeyRequestRequestTypeDef, _OptionalDeleteAccessKeyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteAccountAliasRequestRequestTypeDef = TypedDict(
     "DeleteAccountAliasRequestRequestTypeDef",
     {
         "AccountAlias": str,
     },
 )
 
@@ -1054,62 +1072,58 @@
 DeleteServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
-DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
-    "DeleteServiceLinkedRoleResponseTypeDef",
-    {
-        "DeletionTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef",
     {
         "ServiceSpecificCredentialId": str,
     },
 )
 _OptionalDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class DeleteServiceSpecificCredentialRequestRequestTypeDef(
     _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef,
     _OptionalDeleteServiceSpecificCredentialRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteSigningCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSigningCertificateRequestRequestTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalDeleteSigningCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSigningCertificateRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class DeleteSigningCertificateRequestRequestTypeDef(
     _RequiredDeleteSigningCertificateRequestRequestTypeDef,
     _OptionalDeleteSigningCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteUserPermissionsBoundaryRequestRequestTypeDef = TypedDict(
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
 
@@ -1206,21 +1220,14 @@
 DetachUserPolicyRequestUserDetachPolicyTypeDef = TypedDict(
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableMFADeviceRequestMfaDeviceAssociateTypeDef = TypedDict(
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     {
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
@@ -1257,17 +1264,19 @@
     "_OptionalEntityInfoTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
+
 class EntityInfoTypeDef(_RequiredEntityInfoTypeDef, _OptionalEntityInfoTypeDef):
     pass
 
+
 ErrorDetailsTypeDef = TypedDict(
     "ErrorDetailsTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
@@ -1284,50 +1293,35 @@
     "PermissionsBoundaryDecisionDetailTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
     total=False,
 )
 
-GenerateCredentialReportResponseTypeDef = TypedDict(
-    "GenerateCredentialReportResponseTypeDef",
-    {
-        "State": ReportStateTypeType,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef",
     {
         "EntityPath": str,
     },
 )
 _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef",
     {
         "OrganizationsPolicyId": str,
     },
     total=False,
 )
 
+
 class GenerateOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
-GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
-    "GenerateOrganizationsAccessReportResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
@@ -1335,40 +1329,35 @@
     "_OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef",
     {
         "Granularity": AccessAdvisorUsageGranularityTypeType,
     },
     total=False,
 )
 
+
 class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
-GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
-    "GenerateServiceLastAccessedDetailsResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetAccessKeyLastUsedRequestRequestTypeDef = TypedDict(
     "GetAccessKeyLastUsedRequestRequestTypeDef",
     {
         "AccessKeyId": str,
     },
 )
 
-GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef = TypedDict(
-    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filter": Sequence[EntityTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetAccountAuthorizationDetailsRequestRequestTypeDef = TypedDict(
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
     {
@@ -1392,104 +1381,51 @@
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
     total=False,
 )
 
-GetAccountSummaryResponseTypeDef = TypedDict(
-    "GetAccountSummaryResponseTypeDef",
-    {
-        "SummaryMap": Dict[summaryKeyTypeType, int],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContextKeysForCustomPolicyRequestRequestTypeDef = TypedDict(
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
 )
 
-GetContextKeysForPolicyResponseTypeDef = TypedDict(
-    "GetContextKeysForPolicyResponseTypeDef",
-    {
-        "ContextKeyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef",
     {
         "PolicySourceArn": str,
     },
 )
 _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
     total=False,
 )
 
+
 class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(
     _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
     _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetCredentialReportResponseTypeDef = TypedDict(
-    "GetCredentialReportResponseTypeDef",
-    {
-        "Content": bytes,
-        "ReportFormat": Literal["text/csv"],
-        "GeneratedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetGroupPolicyRequestRequestTypeDef = TypedDict(
     "GetGroupPolicyRequestRequestTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
     },
 )
 
-GetGroupPolicyResponseTypeDef = TypedDict(
-    "GetGroupPolicyResponseTypeDef",
-    {
-        "GroupName": str,
-        "PolicyName": str,
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
-    "_RequiredGetGroupRequestGetGroupPaginateTypeDef",
-    {
-        "GroupName": str,
-    },
-)
-_OptionalGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
-    "_OptionalGetGroupRequestGetGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetGroupRequestGetGroupPaginateTypeDef(
-    _RequiredGetGroupRequestGetGroupPaginateTypeDef, _OptionalGetGroupRequestGetGroupPaginateTypeDef
-):
-    pass
-
 _RequiredGetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetGroupRequestRequestTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalGetGroupRequestRequestTypeDef = TypedDict(
@@ -1497,19 +1433,21 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class GetGroupRequestRequestTypeDef(
     _RequiredGetGroupRequestRequestTypeDef, _OptionalGetGroupRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1539,29 +1477,20 @@
     "_OptionalGetMFADeviceRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class GetMFADeviceRequestRequestTypeDef(
     _RequiredGetMFADeviceRequestRequestTypeDef, _OptionalGetMFADeviceRequestRequestTypeDef
 ):
     pass
 
-GetMFADeviceResponseTypeDef = TypedDict(
-    "GetMFADeviceResponseTypeDef",
-    {
-        "UserName": str,
-        "SerialNumber": str,
-        "EnableDate": datetime,
-        "Certifications": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
     },
 )
@@ -1578,20 +1507,22 @@
         "MaxItems": int,
         "Marker": str,
         "SortKey": sortKeyTypeType,
     },
     total=False,
 )
 
+
 class GetOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGetOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGetOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
+
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
@@ -1607,24 +1538,14 @@
     "GetRolePolicyRequestRequestTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
     },
 )
 
-GetRolePolicyResponseTypeDef = TypedDict(
-    "GetRolePolicyResponseTypeDef",
-    {
-        "RoleName": str,
-        "PolicyName": str,
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRoleRequestRequestTypeDef = TypedDict(
     "GetRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
@@ -1658,17 +1579,19 @@
     "_OptionalSSHPublicKeyTypeDef",
     {
         "UploadDate": datetime,
     },
     total=False,
 )
 
+
 class SSHPublicKeyTypeDef(_RequiredSSHPublicKeyTypeDef, _OptionalSSHPublicKeyTypeDef):
     pass
 
+
 GetServerCertificateRequestRequestTypeDef = TypedDict(
     "GetServerCertificateRequestRequestTypeDef",
     {
         "ServerCertificateName": str,
     },
 )
 
@@ -1683,20 +1606,22 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGetServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGetServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     {
         "JobId": str,
         "ServiceNamespace": str,
     },
 )
@@ -1705,20 +1630,22 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef(
     _RequiredGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     _OptionalGetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
 ):
     pass
 
+
 GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     {
         "DeletionTaskId": str,
     },
 )
 
@@ -1726,24 +1653,14 @@
     "GetUserPolicyRequestRequestTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
     },
 )
 
-GetUserPolicyResponseTypeDef = TypedDict(
-    "GetUserPolicyResponseTypeDef",
-    {
-        "UserName": str,
-        "PolicyName": str,
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
@@ -1753,81 +1670,33 @@
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
     total=False,
 )
 
-ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
-    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAccessKeysRequestRequestTypeDef = TypedDict(
     "ListAccessKeysRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesRequestListAccountAliasesPaginateTypeDef = TypedDict(
-    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAccountAliasesRequestRequestTypeDef = TypedDict(
     "ListAccountAliasesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesResponseTypeDef = TypedDict(
-    "ListAccountAliasesResponseTypeDef",
-    {
-        "AccountAliases": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
-    {
-        "GroupName": str,
-    },
-)
-_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef(
-    _RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
-    _OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttachedGroupPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedGroupPoliciesRequestRequestTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalListAttachedGroupPoliciesRequestRequestTypeDef = TypedDict(
@@ -1836,40 +1705,21 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListAttachedGroupPoliciesRequestRequestTypeDef(
     _RequiredListAttachedGroupPoliciesRequestRequestTypeDef,
     _OptionalListAttachedGroupPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef(
-    _RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
-    _OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListAttachedRolePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedRolePoliciesRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
@@ -1879,40 +1729,21 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListAttachedRolePoliciesRequestRequestTypeDef(
     _RequiredListAttachedRolePoliciesRequestRequestTypeDef,
     _OptionalListAttachedRolePoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef(
-    _RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
-    _OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListAttachedUserPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedUserPoliciesRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
@@ -1922,42 +1753,21 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListAttachedUserPoliciesRequestRequestTypeDef(
     _RequiredListAttachedUserPoliciesRequestRequestTypeDef,
     _OptionalListAttachedUserPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
-    "_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
-    "_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
-    {
-        "EntityFilter": EntityTypeType,
-        "PathPrefix": str,
-        "PolicyUsageFilter": PolicyUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef(
-    _RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
-    _OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
-):
-    pass
 
 _RequiredListEntitiesForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesForPolicyRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
@@ -1969,20 +1779,22 @@
         "PolicyUsageFilter": PolicyUsageTypeType,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListEntitiesForPolicyRequestRequestTypeDef(
     _RequiredListEntitiesForPolicyRequestRequestTypeDef,
     _OptionalListEntitiesForPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 PolicyGroupTypeDef = TypedDict(
     "PolicyGroupTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
     total=False,
@@ -2002,34 +1814,14 @@
     {
         "UserName": str,
         "UserId": str,
     },
     total=False,
 )
 
-_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
-    {
-        "GroupName": str,
-    },
-)
-_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef(
-    _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
-    _OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupPoliciesRequestRequestTypeDef",
     {
         "GroupName": str,
     },
 )
 _OptionalListGroupPoliciesRequestRequestTypeDef = TypedDict(
@@ -2037,48 +1829,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListGroupPoliciesRequestRequestTypeDef(
     _RequiredListGroupPoliciesRequestRequestTypeDef, _OptionalListGroupPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListGroupPoliciesResponseTypeDef = TypedDict(
-    "ListGroupPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupsForUserRequestListGroupsForUserPaginateTypeDef(
-    _RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
-    _OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
-):
-    pass
 
 _RequiredListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsForUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
@@ -2087,58 +1851,31 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListGroupsForUserRequestRequestTypeDef(
     _RequiredListGroupsForUserRequestRequestTypeDef, _OptionalListGroupsForUserRequestRequestTypeDef
 ):
     pass
 
-ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
-    {
-        "InstanceProfileName": str,
-    },
-)
-_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef(
-    _RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
-    _OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListInstanceProfileTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceProfileTagsRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
     },
 )
 _OptionalListInstanceProfileTagsRequestRequestTypeDef = TypedDict(
@@ -2146,39 +1883,21 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListInstanceProfileTagsRequestRequestTypeDef(
     _RequiredListInstanceProfileTagsRequestRequestTypeDef,
     _OptionalListInstanceProfileTagsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
-    "_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
-    "_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef(
-    _RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
-    _OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
-):
-    pass
 
 _RequiredListInstanceProfilesForRoleRequestRequestTypeDef = TypedDict(
     "_RequiredListInstanceProfilesForRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
@@ -2187,59 +1906,32 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListInstanceProfilesForRoleRequestRequestTypeDef(
     _RequiredListInstanceProfilesForRoleRequestRequestTypeDef,
     _OptionalListInstanceProfilesForRoleRequestRequestTypeDef,
 ):
     pass
 
-ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
-    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListInstanceProfilesRequestRequestTypeDef = TypedDict(
     "ListInstanceProfilesRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
-    "_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
-    {
-        "SerialNumber": str,
-    },
-)
-_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
-    "_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef(
-    _RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
-    _OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMFADeviceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListMFADeviceTagsRequestRequestTypeDef",
     {
         "SerialNumber": str,
     },
 )
 _OptionalListMFADeviceTagsRequestRequestTypeDef = TypedDict(
@@ -2247,27 +1939,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListMFADeviceTagsRequestRequestTypeDef(
     _RequiredListMFADeviceTagsRequestRequestTypeDef, _OptionalListMFADeviceTagsRequestRequestTypeDef
 ):
     pass
 
-ListMFADevicesRequestListMFADevicesPaginateTypeDef = TypedDict(
-    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListMFADevicesRequestRequestTypeDef = TypedDict(
     "ListMFADevicesRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
@@ -2280,38 +1965,14 @@
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
     },
 )
 
-_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
-        {
-            "OpenIDConnectProviderArn": str,
-        },
-    )
-)
-_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef(
-    _RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
-    _OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
     },
 )
 _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef = TypedDict(
@@ -2319,20 +1980,22 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListOpenIDConnectProviderTagsRequestRequestTypeDef(
     _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef,
     _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef,
 ):
     pass
 
+
 OpenIDConnectProviderListEntryTypeDef = TypedDict(
     "OpenIDConnectProviderListEntryTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -2350,19 +2013,21 @@
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
     total=False,
 )
 
+
 class PolicyGrantingServiceAccessTypeDef(
     _RequiredPolicyGrantingServiceAccessTypeDef, _OptionalPolicyGrantingServiceAccessTypeDef
 ):
     pass
 
+
 _RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     {
         "Arn": str,
         "ServiceNamespaces": Sequence[str],
     },
 )
@@ -2370,65 +2035,35 @@
     "_OptionalListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListPoliciesGrantingServiceAccessRequestRequestTypeDef(
     _RequiredListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     _OptionalListPoliciesGrantingServiceAccessRequestRequestTypeDef,
 ):
     pass
 
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "Scope": policyScopeTypeType,
-        "OnlyAttached": bool,
-        "PathPrefix": str,
-        "PolicyUsageFilter": PolicyUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "Scope": policyScopeTypeType,
         "OnlyAttached": bool,
         "PathPrefix": str,
         "PolicyUsageFilter": PolicyUsageTypeType,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyTagsRequestListPolicyTagsPaginateTypeDef(
-    _RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
-    _OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPolicyTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyTagsRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalListPolicyTagsRequestRequestTypeDef = TypedDict(
@@ -2436,38 +2071,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListPolicyTagsRequestRequestTypeDef(
     _RequiredListPolicyTagsRequestRequestTypeDef, _OptionalListPolicyTagsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
-    {
-        "PolicyArn": str,
-    },
-)
-_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef(
-    _RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
-    _OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListPolicyVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyVersionsRequestRequestTypeDef",
     {
         "PolicyArn": str,
     },
 )
@@ -2476,39 +2093,21 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListPolicyVersionsRequestRequestTypeDef(
     _RequiredListPolicyVersionsRequestRequestTypeDef,
     _OptionalListPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRolePoliciesRequestListRolePoliciesPaginateTypeDef(
-    _RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
-    _OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListRolePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListRolePoliciesRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
@@ -2517,48 +2116,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListRolePoliciesRequestRequestTypeDef(
     _RequiredListRolePoliciesRequestRequestTypeDef, _OptionalListRolePoliciesRequestRequestTypeDef
 ):
     pass
 
-ListRolePoliciesResponseTypeDef = TypedDict(
-    "ListRolePoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
-    "_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef",
-    {
-        "RoleName": str,
-    },
-)
-_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
-    "_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRoleTagsRequestListRoleTagsPaginateTypeDef(
-    _RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef,
-    _OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef,
-):
-    pass
 
 _RequiredListRoleTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListRoleTagsRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
@@ -2567,58 +2138,31 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListRoleTagsRequestRequestTypeDef(
     _RequiredListRoleTagsRequestRequestTypeDef, _OptionalListRoleTagsRequestRequestTypeDef
 ):
     pass
 
-ListRolesRequestListRolesPaginateTypeDef = TypedDict(
-    "ListRolesRequestListRolesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListRolesRequestRequestTypeDef = TypedDict(
     "ListRolesRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
-    "_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
-    {
-        "SAMLProviderArn": str,
-    },
-)
-_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
-    "_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef(
-    _RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
-    _OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSAMLProviderTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListSAMLProviderTagsRequestRequestTypeDef",
     {
         "SAMLProviderArn": str,
     },
 )
 _OptionalListSAMLProviderTagsRequestRequestTypeDef = TypedDict(
@@ -2626,39 +2170,32 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListSAMLProviderTagsRequestRequestTypeDef(
     _RequiredListSAMLProviderTagsRequestRequestTypeDef,
     _OptionalListSAMLProviderTagsRequestRequestTypeDef,
 ):
     pass
 
+
 SAMLProviderListEntryTypeDef = TypedDict(
     "SAMLProviderListEntryTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
     total=False,
 )
 
-ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = TypedDict(
-    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSSHPublicKeysRequestRequestTypeDef = TypedDict(
     "ListSSHPublicKeysRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -2671,34 +2208,14 @@
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
 )
 
-_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
-    "_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
-    {
-        "ServerCertificateName": str,
-    },
-)
-_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
-    "_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef(
-    _RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
-    _OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredListServerCertificateTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListServerCertificateTagsRequestRequestTypeDef",
     {
         "ServerCertificateName": str,
     },
 )
 _OptionalListServerCertificateTagsRequestRequestTypeDef = TypedDict(
@@ -2706,28 +2223,21 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListServerCertificateTagsRequestRequestTypeDef(
     _RequiredListServerCertificateTagsRequestRequestTypeDef,
     _OptionalListServerCertificateTagsRequestRequestTypeDef,
 ):
     pass
 
-ListServerCertificatesRequestListServerCertificatesPaginateTypeDef = TypedDict(
-    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListServerCertificatesRequestRequestTypeDef = TypedDict(
     "ListServerCertificatesRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
@@ -2749,19 +2259,21 @@
     {
         "UploadDate": datetime,
         "Expiration": datetime,
     },
     total=False,
 )
 
+
 class ServerCertificateMetadataTypeDef(
     _RequiredServerCertificateMetadataTypeDef, _OptionalServerCertificateMetadataTypeDef
 ):
     pass
 
+
 ListServiceSpecificCredentialsRequestRequestTypeDef = TypedDict(
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
@@ -2775,23 +2287,14 @@
         "ServiceUserName": str,
         "CreateDate": datetime,
         "ServiceSpecificCredentialId": str,
         "ServiceName": str,
     },
 )
 
-ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef = TypedDict(
-    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
-    {
-        "UserName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningCertificatesRequestRequestTypeDef = TypedDict(
     "ListSigningCertificatesRequestRequestTypeDef",
     {
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -2811,38 +2314,20 @@
     "_OptionalSigningCertificateTypeDef",
     {
         "UploadDate": datetime,
     },
     total=False,
 )
 
+
 class SigningCertificateTypeDef(
     _RequiredSigningCertificateTypeDef, _OptionalSigningCertificateTypeDef
 ):
     pass
 
-_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUserPoliciesRequestListUserPoliciesPaginateTypeDef(
-    _RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
-    _OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListUserPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoliciesRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
@@ -2851,48 +2336,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListUserPoliciesRequestRequestTypeDef(
     _RequiredListUserPoliciesRequestRequestTypeDef, _OptionalListUserPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListUserPoliciesResponseTypeDef = TypedDict(
-    "ListUserPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
-    "_RequiredListUserTagsRequestListUserTagsPaginateTypeDef",
-    {
-        "UserName": str,
-    },
-)
-_OptionalListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
-    "_OptionalListUserTagsRequestListUserTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUserTagsRequestListUserTagsPaginateTypeDef(
-    _RequiredListUserTagsRequestListUserTagsPaginateTypeDef,
-    _OptionalListUserTagsRequestListUserTagsPaginateTypeDef,
-):
-    pass
 
 _RequiredListUserTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserTagsRequestRequestTypeDef",
     {
         "UserName": str,
     },
 )
@@ -2901,65 +2358,49 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListUserTagsRequestRequestTypeDef(
     _RequiredListUserTagsRequestRequestTypeDef, _OptionalListUserTagsRequestRequestTypeDef
 ):
     pass
 
-ListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "ListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PathPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListUsersRequestRequestTypeDef = TypedDict(
     "ListUsersRequestRequestTypeDef",
     {
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef = TypedDict(
-    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
-    {
-        "AssignmentStatus": assignmentStatusTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVirtualMFADevicesRequestRequestTypeDef = TypedDict(
     "ListVirtualMFADevicesRequestRequestTypeDef",
     {
         "AssignmentStatus": assignmentStatusTypeType,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PolicyDocumentStatementTypeDef = TypedDict(
+    "PolicyDocumentStatementTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Effect": str,
+        "Resource": Union[str, List[str]],
+        "Sid": str,
+        "Action": Union[str, List[str]],
     },
-    total=False,
 )
 
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "Line": int,
         "Column": int,
@@ -3102,30 +2543,21 @@
     "_OptionalResetServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class ResetServiceSpecificCredentialRequestRequestTypeDef(
     _RequiredResetServiceSpecificCredentialRequestRequestTypeDef,
     _OptionalResetServiceSpecificCredentialRequestRequestTypeDef,
 ):
     pass
 
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
 
 ResyncMFADeviceRequestMfaDeviceResyncTypeDef = TypedDict(
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     {
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
@@ -3146,36 +2578,14 @@
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
     total=False,
 )
 
-RoleLastUsedResponseMetadataTypeDef = TypedDict(
-    "RoleLastUsedResponseMetadataTypeDef",
-    {
-        "LastUsedDate": datetime,
-        "Region": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ServerCertificateMetadataResponseMetadataTypeDef = TypedDict(
-    "ServerCertificateMetadataResponseMetadataTypeDef",
-    {
-        "Path": str,
-        "ServerCertificateName": str,
-        "ServerCertificateId": str,
-        "Arn": str,
-        "UploadDate": datetime,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TrackedActionLastAccessedTypeDef = TypedDict(
     "TrackedActionLastAccessedTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
@@ -3305,19 +2715,21 @@
     "_OptionalUpdateAccessKeyRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class UpdateAccessKeyRequestRequestTypeDef(
     _RequiredUpdateAccessKeyRequestRequestTypeDef, _OptionalUpdateAccessKeyRequestRequestTypeDef
 ):
     pass
 
+
 UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef = TypedDict(
     "UpdateAccountPasswordPolicyRequestAccountPasswordPolicyUpdateTypeDef",
     {
         "MinimumPasswordLength": int,
         "RequireSymbols": bool,
         "RequireNumbers": bool,
         "RequireUppercaseCharacters": bool,
@@ -3397,19 +2809,21 @@
     {
         "NewPath": str,
         "NewGroupName": str,
     },
     total=False,
 )
 
+
 class UpdateGroupRequestRequestTypeDef(
     _RequiredUpdateGroupRequestRequestTypeDef, _OptionalUpdateGroupRequestRequestTypeDef
 ):
     pass
 
+
 UpdateLoginProfileRequestLoginProfileUpdateTypeDef = TypedDict(
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     {
         "Password": str,
         "PasswordResetRequired": bool,
     },
     total=False,
@@ -3426,20 +2840,22 @@
     {
         "Password": str,
         "PasswordResetRequired": bool,
     },
     total=False,
 )
 
+
 class UpdateLoginProfileRequestRequestTypeDef(
     _RequiredUpdateLoginProfileRequestRequestTypeDef,
     _OptionalUpdateLoginProfileRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef = TypedDict(
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "ThumbprintList": Sequence[str],
     },
 )
@@ -3463,19 +2879,21 @@
     {
         "Description": str,
         "MaxSessionDuration": int,
     },
     total=False,
 )
 
+
 class UpdateRoleRequestRequestTypeDef(
     _RequiredUpdateRoleRequestRequestTypeDef, _OptionalUpdateRoleRequestRequestTypeDef
 ):
     pass
 
+
 UpdateSAMLProviderRequestRequestTypeDef = TypedDict(
     "UpdateSAMLProviderRequestRequestTypeDef",
     {
         "SAMLMetadataDocument": str,
         "SAMLProviderArn": str,
     },
 )
@@ -3483,22 +2901,14 @@
 UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = TypedDict(
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
     {
         "SAMLMetadataDocument": str,
     },
 )
 
-UpdateSAMLProviderResponseTypeDef = TypedDict(
-    "UpdateSAMLProviderResponseTypeDef",
-    {
-        "SAMLProviderArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSSHPublicKeyRequestRequestTypeDef = TypedDict(
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
     },
@@ -3515,20 +2925,22 @@
     {
         "NewPath": str,
         "NewServerCertificateName": str,
     },
     total=False,
 )
 
+
 class UpdateServerCertificateRequestRequestTypeDef(
     _RequiredUpdateServerCertificateRequestRequestTypeDef,
     _OptionalUpdateServerCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateServerCertificateRequestServerCertificateUpdateTypeDef = TypedDict(
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     {
         "NewPath": str,
         "NewServerCertificateName": str,
     },
     total=False,
@@ -3545,20 +2957,22 @@
     "_OptionalUpdateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class UpdateServiceSpecificCredentialRequestRequestTypeDef(
     _RequiredUpdateServiceSpecificCredentialRequestRequestTypeDef,
     _OptionalUpdateServiceSpecificCredentialRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSigningCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSigningCertificateRequestRequestTypeDef",
     {
         "CertificateId": str,
         "Status": statusTypeType,
     },
 )
@@ -3566,20 +2980,22 @@
     "_OptionalUpdateSigningCertificateRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class UpdateSigningCertificateRequestRequestTypeDef(
     _RequiredUpdateSigningCertificateRequestRequestTypeDef,
     _OptionalUpdateSigningCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateSigningCertificateRequestSigningCertificateActivateTypeDef = TypedDict(
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     {
         "Status": statusTypeType,
     },
     total=False,
 )
@@ -3603,19 +3019,21 @@
     {
         "NewPath": str,
         "NewUserName": str,
     },
     total=False,
 )
 
+
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+
 UpdateUserRequestUserUpdateTypeDef = TypedDict(
     "UpdateUserRequestUserUpdateTypeDef",
     {
         "NewPath": str,
         "NewUserName": str,
     },
     total=False,
@@ -3639,94 +3057,284 @@
     "_OptionalUploadSigningCertificateRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class UploadSigningCertificateRequestRequestTypeDef(
     _RequiredUploadSigningCertificateRequestRequestTypeDef,
     _OptionalUploadSigningCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef = TypedDict(
     "_RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     {
         "CertificateBody": str,
     },
 )
 _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef = TypedDict(
     "_OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
+
 class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(
     _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
     _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
 ):
     pass
 
+
+AttachedPermissionsBoundaryResponseTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryResponseTypeDef",
+    {
+        "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
+        "PermissionsBoundaryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAccessKeyResponseTypeDef = TypedDict(
+    "CreateAccessKeyResponseTypeDef",
+    {
+        "AccessKey": AccessKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
+    "DeleteServiceLinkedRoleResponseTypeDef",
+    {
+        "DeletionTaskId": str,
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
+GenerateCredentialReportResponseTypeDef = TypedDict(
+    "GenerateCredentialReportResponseTypeDef",
+    {
+        "State": ReportStateTypeType,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
+    "GenerateOrganizationsAccessReportResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAccessKeyLastUsedResponseTypeDef = TypedDict(
     "GetAccessKeyLastUsedResponseTypeDef",
     {
         "UserName": str,
         "AccessKeyLastUsed": AccessKeyLastUsedTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSummaryResponseTypeDef = TypedDict(
+    "GetAccountSummaryResponseTypeDef",
+    {
+        "SummaryMap": Dict[summaryKeyTypeType, int],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContextKeysForPolicyResponseTypeDef = TypedDict(
+    "GetContextKeysForPolicyResponseTypeDef",
+    {
+        "ContextKeyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCredentialReportResponseTypeDef = TypedDict(
+    "GetCredentialReportResponseTypeDef",
+    {
+        "Content": bytes,
+        "ReportFormat": Literal["text/csv"],
+        "GeneratedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupPolicyResponseTypeDef = TypedDict(
+    "GetGroupPolicyResponseTypeDef",
+    {
+        "GroupName": str,
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMFADeviceResponseTypeDef = TypedDict(
+    "GetMFADeviceResponseTypeDef",
+    {
+        "UserName": str,
+        "SerialNumber": str,
+        "EnableDate": datetime,
+        "Certifications": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRolePolicyResponseTypeDef = TypedDict(
+    "GetRolePolicyResponseTypeDef",
+    {
+        "RoleName": str,
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserPolicyResponseTypeDef = TypedDict(
+    "GetUserPolicyResponseTypeDef",
+    {
+        "UserName": str,
+        "PolicyName": str,
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessKeysResponseTypeDef = TypedDict(
     "ListAccessKeysResponseTypeDef",
     {
         "AccessKeyMetadata": List[AccessKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAccessKeyResponseTypeDef = TypedDict(
-    "CreateAccessKeyResponseTypeDef",
+ListAccountAliasesResponseTypeDef = TypedDict(
+    "ListAccountAliasesResponseTypeDef",
     {
-        "AccessKey": AccessKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountAliases": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupPoliciesResponseTypeDef = TypedDict(
+    "ListGroupPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRolePoliciesResponseTypeDef = TypedDict(
+    "ListRolePoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListUserPoliciesResponseTypeDef = TypedDict(
+    "ListUserPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RoleLastUsedResponseTypeDef = TypedDict(
+    "RoleLastUsedResponseTypeDef",
+    {
+        "LastUsedDate": datetime,
+        "Region": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerCertificateMetadataResponseTypeDef = TypedDict(
+    "ServerCertificateMetadataResponseTypeDef",
+    {
+        "Path": str,
+        "ServerCertificateName": str,
+        "ServerCertificateId": str,
+        "Arn": str,
+        "UploadDate": datetime,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSAMLProviderResponseTypeDef = TypedDict(
+    "UpdateSAMLProviderResponseTypeDef",
+    {
+        "SAMLProviderArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachedGroupPoliciesResponseTypeDef = TypedDict(
     "ListAttachedGroupPoliciesResponseTypeDef",
     {
         "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachedRolePoliciesResponseTypeDef = TypedDict(
     "ListAttachedRolePoliciesResponseTypeDef",
     {
         "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachedUserPoliciesResponseTypeDef = TypedDict(
     "ListAttachedUserPoliciesResponseTypeDef",
     {
         "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSimulateCustomPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSimulateCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
@@ -3745,47 +3353,21 @@
         "ResourceHandlingOption": str,
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class SimulateCustomPolicyRequestRequestTypeDef(
     _RequiredSimulateCustomPolicyRequestRequestTypeDef,
     _OptionalSimulateCustomPolicyRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
-    "_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
-    {
-        "PolicyInputList": Sequence[str],
-        "ActionNames": Sequence[str],
-    },
-)
-_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
-    "_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
-    {
-        "PermissionsBoundaryPolicyInputList": Sequence[str],
-        "ResourceArns": Sequence[str],
-        "ResourcePolicy": str,
-        "ResourceOwner": str,
-        "CallerArn": str,
-        "ContextEntries": Sequence[ContextEntryTypeDef],
-        "ResourceHandlingOption": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef(
-    _RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
-    _OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
-):
-    pass
 
 _RequiredSimulatePrincipalPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSimulatePrincipalPolicyRequestRequestTypeDef",
     {
         "PolicySourceArn": str,
         "ActionNames": Sequence[str],
     },
@@ -3803,74 +3385,47 @@
         "ResourceHandlingOption": str,
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class SimulatePrincipalPolicyRequestRequestTypeDef(
     _RequiredSimulatePrincipalPolicyRequestRequestTypeDef,
     _OptionalSimulatePrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
-    "_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    {
-        "PolicySourceArn": str,
-        "ActionNames": Sequence[str],
-    },
-)
-_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
-    "_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    {
-        "PolicyInputList": Sequence[str],
-        "PermissionsBoundaryPolicyInputList": Sequence[str],
-        "ResourceArns": Sequence[str],
-        "ResourcePolicy": str,
-        "ResourceOwner": str,
-        "CallerArn": str,
-        "ContextEntries": Sequence[ContextEntryTypeDef],
-        "ResourceHandlingOption": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
-    _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-):
-    pass
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsForUserResponseTypeDef = TypedDict(
     "ListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestRequestTypeDef",
     {
         "InstanceProfileName": str,
@@ -3881,20 +3436,22 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateInstanceProfileRequestRequestTypeDef(
     _RequiredCreateInstanceProfileRequestRequestTypeDef,
     _OptionalCreateInstanceProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef = TypedDict(
     "_RequiredCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     {
         "InstanceProfileName": str,
     },
 )
 _OptionalCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef = TypedDict(
@@ -3902,20 +3459,22 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef(
     _RequiredCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     _OptionalCreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
 ):
     pass
 
+
 _RequiredCreateOpenIDConnectProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpenIDConnectProviderRequestRequestTypeDef",
     {
         "Url": str,
         "ThumbprintList": Sequence[str],
     },
 )
@@ -3924,26 +3483,28 @@
     {
         "ClientIDList": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpenIDConnectProviderRequestRequestTypeDef(
     _RequiredCreateOpenIDConnectProviderRequestRequestTypeDef,
     _OptionalCreateOpenIDConnectProviderRequestRequestTypeDef,
 ):
     pass
 
+
 CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
     "CreateOpenIDConnectProviderResponseTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
@@ -3956,19 +3517,21 @@
         "Path": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePolicyRequestRequestTypeDef(
     _RequiredCreatePolicyRequestRequestTypeDef, _OptionalCreatePolicyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreatePolicyRequestServiceResourceCreatePolicyTypeDef = TypedDict(
     "_RequiredCreatePolicyRequestServiceResourceCreatePolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -3978,20 +3541,22 @@
         "Path": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePolicyRequestServiceResourceCreatePolicyTypeDef(
     _RequiredCreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     _OptionalCreatePolicyRequestServiceResourceCreatePolicyTypeDef,
 ):
     pass
 
+
 _RequiredCreateRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRoleRequestRequestTypeDef",
     {
         "RoleName": str,
         "AssumeRolePolicyDocument": str,
     },
 )
@@ -4003,19 +3568,21 @@
         "MaxSessionDuration": int,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRoleRequestRequestTypeDef(
     _RequiredCreateRoleRequestRequestTypeDef, _OptionalCreateRoleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateRoleRequestServiceResourceCreateRoleTypeDef = TypedDict(
     "_RequiredCreateRoleRequestServiceResourceCreateRoleTypeDef",
     {
         "RoleName": str,
         "AssumeRolePolicyDocument": str,
     },
 )
@@ -4027,20 +3594,22 @@
         "MaxSessionDuration": int,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRoleRequestServiceResourceCreateRoleTypeDef(
     _RequiredCreateRoleRequestServiceResourceCreateRoleTypeDef,
     _OptionalCreateRoleRequestServiceResourceCreateRoleTypeDef,
 ):
     pass
 
+
 _RequiredCreateSAMLProviderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSAMLProviderRequestRequestTypeDef",
     {
         "SAMLMetadataDocument": str,
         "Name": str,
     },
 )
@@ -4048,20 +3617,22 @@
     "_OptionalCreateSAMLProviderRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSAMLProviderRequestRequestTypeDef(
     _RequiredCreateSAMLProviderRequestRequestTypeDef,
     _OptionalCreateSAMLProviderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef = TypedDict(
     "_RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef",
     {
         "SAMLMetadataDocument": str,
         "Name": str,
     },
 )
@@ -4069,26 +3640,28 @@
     "_OptionalCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef(
     _RequiredCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
     _OptionalCreateSAMLProviderRequestServiceResourceCreateSamlProviderTypeDef,
 ):
     pass
 
+
 CreateSAMLProviderResponseTypeDef = TypedDict(
     "CreateSAMLProviderResponseTypeDef",
     {
         "SAMLProviderArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "UserName": str,
@@ -4100,19 +3673,21 @@
         "Path": str,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateUserRequestServiceResourceCreateUserTypeDef = TypedDict(
     "_RequiredCreateUserRequestServiceResourceCreateUserTypeDef",
     {
         "UserName": str,
     },
 )
 _OptionalCreateUserRequestServiceResourceCreateUserTypeDef = TypedDict(
@@ -4121,20 +3696,22 @@
         "Path": str,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserRequestServiceResourceCreateUserTypeDef(
     _RequiredCreateUserRequestServiceResourceCreateUserTypeDef,
     _OptionalCreateUserRequestServiceResourceCreateUserTypeDef,
 ):
     pass
 
+
 CreateUserRequestUserCreateTypeDef = TypedDict(
     "CreateUserRequestUserCreateTypeDef",
     {
         "Path": str,
         "PermissionsBoundary": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -4152,20 +3729,22 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVirtualMFADeviceRequestRequestTypeDef(
     _RequiredCreateVirtualMFADeviceRequestRequestTypeDef,
     _OptionalCreateVirtualMFADeviceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef = TypedDict(
     "_RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef",
     {
         "VirtualMFADeviceName": str,
     },
 )
 _OptionalCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef = TypedDict(
@@ -4173,120 +3752,122 @@
     {
         "Path": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef(
     _RequiredCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
     _OptionalCreateVirtualMFADeviceRequestServiceResourceCreateVirtualMfaDeviceTypeDef,
 ):
     pass
 
+
 GetOpenIDConnectProviderResponseTypeDef = TypedDict(
     "GetOpenIDConnectProviderResponseTypeDef",
     {
         "Url": str,
         "ClientIDList": List[str],
         "ThumbprintList": List[str],
         "CreateDate": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSAMLProviderResponseTypeDef = TypedDict(
     "GetSAMLProviderResponseTypeDef",
     {
         "SAMLMetadataDocument": str,
         "CreateDate": datetime,
         "ValidUntil": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfileTagsResponseTypeDef = TypedDict(
     "ListInstanceProfileTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMFADeviceTagsResponseTypeDef = TypedDict(
     "ListMFADeviceTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpenIDConnectProviderTagsResponseTypeDef = TypedDict(
     "ListOpenIDConnectProviderTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyTagsResponseTypeDef = TypedDict(
     "ListPolicyTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoleTagsResponseTypeDef = TypedDict(
     "ListRoleTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSAMLProviderTagsResponseTypeDef = TypedDict(
     "ListSAMLProviderTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServerCertificateTagsResponseTypeDef = TypedDict(
     "ListServerCertificateTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserTagsResponseTypeDef = TypedDict(
     "ListUserTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyTypeDef = TypedDict(
     "PolicyTypeDef",
     {
         "PolicyName": str,
@@ -4383,20 +3964,22 @@
         "Path": str,
         "CertificateChain": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UploadServerCertificateRequestRequestTypeDef(
     _RequiredUploadServerCertificateRequestRequestTypeDef,
     _OptionalUploadServerCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef = TypedDict(
     "_RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
     {
         "ServerCertificateName": str,
         "CertificateBody": str,
         "PrivateKey": str,
     },
@@ -4407,32 +3990,34 @@
         "Path": str,
         "CertificateChain": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "Path": str,
@@ -4448,91 +4033,48 @@
         "PasswordLastUsed": datetime,
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
+
 CreateLoginProfileResponseTypeDef = TypedDict(
     "CreateLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoginProfileResponseTypeDef = TypedDict(
     "GetLoginProfileResponseTypeDef",
     {
         "LoginProfile": LoginProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
-    {
-        "PolicyVersion": PolicyVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
-    {
-        "PolicyVersion": PolicyVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyVersionsResponseTypeDef = TypedDict(
-    "ListPolicyVersionsResponseTypeDef",
-    {
-        "Versions": List[PolicyVersionTypeDef],
-        "IsTruncated": bool,
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ManagedPolicyDetailTypeDef = TypedDict(
-    "ManagedPolicyDetailTypeDef",
-    {
-        "PolicyName": str,
-        "PolicyId": str,
-        "Arn": str,
-        "Path": str,
-        "DefaultVersionId": str,
-        "AttachmentCount": int,
-        "PermissionsBoundaryUsageCount": int,
-        "IsAttachable": bool,
-        "Description": str,
-        "CreateDate": datetime,
-        "UpdateDate": datetime,
-        "PolicyVersionList": List[PolicyVersionTypeDef],
-    },
-    total=False,
-)
-
 CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
     "CreateServiceSpecificCredentialResponseTypeDef",
     {
         "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetServiceSpecificCredentialResponseTypeDef = TypedDict(
     "ResetServiceSpecificCredentialResponseTypeDef",
     {
         "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletionTaskFailureReasonTypeTypeDef = TypedDict(
     "DeletionTaskFailureReasonTypeTypeDef",
     {
         "Reason": str,
@@ -4551,38 +4093,647 @@
     "_OptionalEntityDetailsTypeDef",
     {
         "LastAuthenticated": datetime,
     },
     total=False,
 )
 
+
 class EntityDetailsTypeDef(_RequiredEntityDetailsTypeDef, _OptionalEntityDetailsTypeDef):
     pass
 
+
 GetOrganizationsAccessReportResponseTypeDef = TypedDict(
     "GetOrganizationsAccessReportResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
         "NumberOfServicesNotAccessed": int,
         "AccessDetails": List[AccessDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ErrorDetails": ErrorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef = TypedDict(
+    "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
+    {
+        "Filter": Sequence[EntityTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
+    "_RequiredGetGroupRequestGetGroupPaginateTypeDef",
+    {
+        "GroupName": str,
+    },
+)
+_OptionalGetGroupRequestGetGroupPaginateTypeDef = TypedDict(
+    "_OptionalGetGroupRequestGetGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetGroupRequestGetGroupPaginateTypeDef(
+    _RequiredGetGroupRequestGetGroupPaginateTypeDef, _OptionalGetGroupRequestGetGroupPaginateTypeDef
+):
+    pass
+
+
+ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
+    "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAccountAliasesRequestListAccountAliasesPaginateTypeDef = TypedDict(
+    "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
+    {
+        "GroupName": str,
+    },
+)
+_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef(
+    _RequiredListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+    _OptionalListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef(
+    _RequiredListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+    _OptionalListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef(
+    _RequiredListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+    _OptionalListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
+    "_RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef = TypedDict(
+    "_OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
+    {
+        "EntityFilter": EntityTypeType,
+        "PathPrefix": str,
+        "PolicyUsageFilter": PolicyUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef(
+    _RequiredListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+    _OptionalListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
+    {
+        "GroupName": str,
+    },
+)
+_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef(
+    _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+    _OptionalListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupsForUserRequestListGroupsForUserPaginateTypeDef(
+    _RequiredListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+    _OptionalListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+
+ListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
+    {
+        "InstanceProfileName": str,
+    },
+)
+_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef(
+    _RequiredListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+    _OptionalListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
+    "_RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef = TypedDict(
+    "_OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef(
+    _RequiredListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+    _OptionalListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+):
+    pass
+
+
+ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
+    "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
+    "_RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
+    {
+        "SerialNumber": str,
+    },
+)
+_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef = TypedDict(
+    "_OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef(
+    _RequiredListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+    _OptionalListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+):
+    pass
+
+
+ListMFADevicesRequestListMFADevicesPaginateTypeDef = TypedDict(
+    "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
+        {
+            "OpenIDConnectProviderArn": str,
+        },
+    )
+)
+_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef(
+    _RequiredListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+    _OptionalListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+):
+    pass
+
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "Scope": policyScopeTypeType,
+        "OnlyAttached": bool,
+        "PathPrefix": str,
+        "PolicyUsageFilter": PolicyUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPolicyTagsRequestListPolicyTagsPaginateTypeDef(
+    _RequiredListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+    _OptionalListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef(
+    _RequiredListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+    _OptionalListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRolePoliciesRequestListRolePoliciesPaginateTypeDef(
+    _RequiredListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+    _OptionalListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
+    "_RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef",
+    {
+        "RoleName": str,
+    },
+)
+_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef = TypedDict(
+    "_OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRoleTagsRequestListRoleTagsPaginateTypeDef(
+    _RequiredListRoleTagsRequestListRoleTagsPaginateTypeDef,
+    _OptionalListRoleTagsRequestListRoleTagsPaginateTypeDef,
+):
+    pass
+
+
+ListRolesRequestListRolesPaginateTypeDef = TypedDict(
+    "ListRolesRequestListRolesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
+    "_RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
+    {
+        "SAMLProviderArn": str,
+    },
+)
+_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef = TypedDict(
+    "_OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef(
+    _RequiredListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+    _OptionalListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+):
+    pass
+
+
+ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef = TypedDict(
+    "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
+    "_RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
+    {
+        "ServerCertificateName": str,
+    },
+)
+_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef = TypedDict(
+    "_OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef(
+    _RequiredListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+    _OptionalListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+):
+    pass
+
+
+ListServerCertificatesRequestListServerCertificatesPaginateTypeDef = TypedDict(
+    "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef = TypedDict(
+    "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
+    {
+        "UserName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUserPoliciesRequestListUserPoliciesPaginateTypeDef(
+    _RequiredListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+    _OptionalListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
+    "_RequiredListUserTagsRequestListUserTagsPaginateTypeDef",
+    {
+        "UserName": str,
+    },
+)
+_OptionalListUserTagsRequestListUserTagsPaginateTypeDef = TypedDict(
+    "_OptionalListUserTagsRequestListUserTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUserTagsRequestListUserTagsPaginateTypeDef(
+    _RequiredListUserTagsRequestListUserTagsPaginateTypeDef,
+    _OptionalListUserTagsRequestListUserTagsPaginateTypeDef,
+):
+    pass
+
+
+ListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "ListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PathPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef = TypedDict(
+    "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
+    {
+        "AssignmentStatus": assignmentStatusTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
+    "_RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
+    {
+        "PolicyInputList": Sequence[str],
+        "ActionNames": Sequence[str],
+    },
+)
+_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef = TypedDict(
+    "_OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
+    {
+        "PermissionsBoundaryPolicyInputList": Sequence[str],
+        "ResourceArns": Sequence[str],
+        "ResourcePolicy": str,
+        "ResourceOwner": str,
+        "CallerArn": str,
+        "ContextEntries": Sequence[ContextEntryTypeDef],
+        "ResourceHandlingOption": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef(
+    _RequiredSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+    _OptionalSimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
+    "_RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
+    {
+        "PolicySourceArn": str,
+        "ActionNames": Sequence[str],
+    },
+)
+_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef = TypedDict(
+    "_OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
+    {
+        "PolicyInputList": Sequence[str],
+        "PermissionsBoundaryPolicyInputList": Sequence[str],
+        "ResourceArns": Sequence[str],
+        "ResourcePolicy": str,
+        "ResourceOwner": str,
+        "CallerArn": str,
+        "ContextEntries": Sequence[ContextEntryTypeDef],
+        "ResourceHandlingOption": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
+    _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
+    _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
+):
+    pass
+
+
 GetAccountPasswordPolicyResponseTypeDef = TypedDict(
     "GetAccountPasswordPolicyResponseTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = TypedDict(
     "_RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
         "InstanceProfileName": str,
@@ -4592,81 +4743,87 @@
     "_OptionalGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef(
     _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     _OptionalGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetPolicyRequestPolicyExistsWaitTypeDef = TypedDict(
     "_RequiredGetPolicyRequestPolicyExistsWaitTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalGetPolicyRequestPolicyExistsWaitTypeDef = TypedDict(
     "_OptionalGetPolicyRequestPolicyExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPolicyRequestPolicyExistsWaitTypeDef(
     _RequiredGetPolicyRequestPolicyExistsWaitTypeDef,
     _OptionalGetPolicyRequestPolicyExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetRoleRequestRoleExistsWaitTypeDef = TypedDict(
     "_RequiredGetRoleRequestRoleExistsWaitTypeDef",
     {
         "RoleName": str,
     },
 )
 _OptionalGetRoleRequestRoleExistsWaitTypeDef = TypedDict(
     "_OptionalGetRoleRequestRoleExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetRoleRequestRoleExistsWaitTypeDef(
     _RequiredGetRoleRequestRoleExistsWaitTypeDef, _OptionalGetRoleRequestRoleExistsWaitTypeDef
 ):
     pass
 
+
 GetUserRequestUserExistsWaitTypeDef = TypedDict(
     "GetUserRequestUserExistsWaitTypeDef",
     {
         "UserName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 GetSSHPublicKeyResponseTypeDef = TypedDict(
     "GetSSHPublicKeyResponseTypeDef",
     {
         "SSHPublicKey": SSHPublicKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadSSHPublicKeyResponseTypeDef = TypedDict(
     "UploadSSHPublicKeyResponseTypeDef",
     {
         "SSHPublicKey": SSHPublicKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupDetailTypeDef = TypedDict(
     "GroupDetailTypeDef",
     {
         "Path": str,
@@ -4701,33 +4858,33 @@
     "ListEntitiesForPolicyResponseTypeDef",
     {
         "PolicyGroups": List[PolicyGroupTypeDef],
         "PolicyUsers": List[PolicyUserTypeDef],
         "PolicyRoles": List[PolicyRoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMFADevicesResponseTypeDef = TypedDict(
     "ListMFADevicesResponseTypeDef",
     {
         "MFADevices": List[MFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpenIDConnectProvidersResponseTypeDef = TypedDict(
     "ListOpenIDConnectProvidersResponseTypeDef",
     {
         "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
     "ListPoliciesGrantingServiceAccessEntryTypeDef",
     {
         "ServiceNamespace": str,
@@ -4736,35 +4893,35 @@
     total=False,
 )
 
 ListSAMLProvidersResponseTypeDef = TypedDict(
     "ListSAMLProvidersResponseTypeDef",
     {
         "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSSHPublicKeysResponseTypeDef = TypedDict(
     "ListSSHPublicKeysResponseTypeDef",
     {
         "SSHPublicKeys": List[SSHPublicKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServerCertificatesResponseTypeDef = TypedDict(
     "ListServerCertificatesResponseTypeDef",
     {
         "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredServerCertificateTypeDef = TypedDict(
     "_RequiredServerCertificateTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
@@ -4776,51 +4933,61 @@
     {
         "CertificateChain": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class ServerCertificateTypeDef(
     _RequiredServerCertificateTypeDef, _OptionalServerCertificateTypeDef
 ):
     pass
 
+
 UploadServerCertificateResponseTypeDef = TypedDict(
     "UploadServerCertificateResponseTypeDef",
     {
         "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceSpecificCredentialsResponseTypeDef = TypedDict(
     "ListServiceSpecificCredentialsResponseTypeDef",
     {
         "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSigningCertificatesResponseTypeDef = TypedDict(
     "ListSigningCertificatesResponseTypeDef",
     {
         "Certificates": List[SigningCertificateTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UploadSigningCertificateResponseTypeDef = TypedDict(
     "UploadSigningCertificateResponseTypeDef",
     {
         "Certificate": SigningCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PolicyDocumentFixedTypeDef = TypedDict(
+    "PolicyDocumentFixedTypeDef",
+    {
+        "Version": str,
+        "Statement": List[PolicyDocumentStatementTypeDef],
     },
 )
 
 StatementTypeDef = TypedDict(
     "StatementTypeDef",
     {
         "SourcePolicyId": str,
@@ -4850,17 +5017,19 @@
         "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagTypeDef],
         "RoleLastUsed": RoleLastUsedTypeDef,
     },
     total=False,
 )
 
+
 class RoleTypeDef(_RequiredRoleTypeDef, _OptionalRoleTypeDef):
     pass
 
+
 _RequiredServiceLastAccessedTypeDef = TypedDict(
     "_RequiredServiceLastAccessedTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
     },
 )
@@ -4872,79 +5041,81 @@
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
         "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
     },
     total=False,
 )
 
+
 class ServiceLastAccessedTypeDef(
     _RequiredServiceLastAccessedTypeDef, _OptionalServiceLastAccessedTypeDef
 ):
     pass
 
+
 CreatePolicyResponseTypeDef = TypedDict(
     "CreatePolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
         "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVirtualMFADeviceTypeDef = TypedDict(
     "_RequiredVirtualMFADeviceTypeDef",
     {
         "SerialNumber": str,
@@ -4958,56 +5129,69 @@
         "User": UserTypeDef,
         "EnableDate": datetime,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class VirtualMFADeviceTypeDef(_RequiredVirtualMFADeviceTypeDef, _OptionalVirtualMFADeviceTypeDef):
     pass
 
+
 GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
     "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
         "Reason": DeletionTaskFailureReasonTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef = TypedDict(
     "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "EntityDetailsList": List[EntityDetailsTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "Error": ErrorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesGrantingServiceAccessResponseTypeDef = TypedDict(
     "ListPoliciesGrantingServiceAccessResponseTypeDef",
     {
         "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServerCertificateResponseTypeDef = TypedDict(
     "GetServerCertificateResponseTypeDef",
     {
         "ServerCertificate": ServerCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PolicyVersionTypeDef = TypedDict(
+    "PolicyVersionTypeDef",
+    {
+        "Document": PolicyDocumentFixedTypeDef,
+        "VersionId": str,
+        "IsDefaultVersion": bool,
+        "CreateDate": datetime,
     },
+    total=False,
 )
 
 _RequiredResourceSpecificResultTypeDef = TypedDict(
     "_RequiredResourceSpecificResultTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
@@ -5020,40 +5204,42 @@
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
     },
     total=False,
 )
 
+
 class ResourceSpecificResultTypeDef(
     _RequiredResourceSpecificResultTypeDef, _OptionalResourceSpecificResultTypeDef
 ):
     pass
 
+
 CreateRoleResponseTypeDef = TypedDict(
     "CreateRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceLinkedRoleResponseTypeDef = TypedDict(
     "CreateServiceLinkedRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoleResponseTypeDef = TypedDict(
     "GetRoleResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInstanceProfileTypeDef = TypedDict(
     "_RequiredInstanceProfileTypeDef",
     {
         "Path": str,
@@ -5068,66 +5254,113 @@
     "_OptionalInstanceProfileTypeDef",
     {
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class InstanceProfileTypeDef(_RequiredInstanceProfileTypeDef, _OptionalInstanceProfileTypeDef):
     pass
 
+
 ListRolesResponseTypeDef = TypedDict(
     "ListRolesResponseTypeDef",
     {
         "Roles": List[RoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoleDescriptionResponseTypeDef = TypedDict(
     "UpdateRoleDescriptionResponseTypeDef",
     {
         "Role": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
     "GetServiceLastAccessedDetailsResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobType": AccessAdvisorUsageGranularityTypeType,
         "JobCreationDate": datetime,
         "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
         "Error": ErrorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVirtualMFADeviceResponseTypeDef = TypedDict(
     "CreateVirtualMFADeviceResponseTypeDef",
     {
         "VirtualMFADevice": VirtualMFADeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualMFADevicesResponseTypeDef = TypedDict(
     "ListVirtualMFADevicesResponseTypeDef",
     {
         "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
+    {
+        "PolicyVersion": PolicyVersionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
+    {
+        "PolicyVersion": PolicyVersionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyVersionsResponseTypeDef = TypedDict(
+    "ListPolicyVersionsResponseTypeDef",
+    {
+        "Versions": List[PolicyVersionTypeDef],
+        "IsTruncated": bool,
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ManagedPolicyDetailTypeDef = TypedDict(
+    "ManagedPolicyDetailTypeDef",
+    {
+        "PolicyName": str,
+        "PolicyId": str,
+        "Arn": str,
+        "Path": str,
+        "DefaultVersionId": str,
+        "AttachmentCount": int,
+        "PermissionsBoundaryUsageCount": int,
+        "IsAttachable": bool,
+        "Description": str,
+        "CreateDate": datetime,
+        "UpdateDate": datetime,
+        "PolicyVersionList": List[PolicyVersionTypeDef],
     },
+    total=False,
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "EvalActionName": str,
         "EvalDecision": PolicyEvaluationDecisionTypeType,
@@ -5143,50 +5376,52 @@
         "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
         "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
     },
     total=False,
 )
 
+
 class EvaluationResultTypeDef(_RequiredEvaluationResultTypeDef, _OptionalEvaluationResultTypeDef):
     pass
 
+
 CreateInstanceProfileResponseTypeDef = TypedDict(
     "CreateInstanceProfileResponseTypeDef",
     {
         "InstanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceProfileResponseTypeDef = TypedDict(
     "GetInstanceProfileResponseTypeDef",
     {
         "InstanceProfile": InstanceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfilesForRoleResponseTypeDef = TypedDict(
     "ListInstanceProfilesForRoleResponseTypeDef",
     {
         "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceProfilesResponseTypeDef = TypedDict(
     "ListInstanceProfilesResponseTypeDef",
     {
         "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RoleDetailTypeDef = TypedDict(
     "RoleDetailTypeDef",
     {
         "Path": str,
@@ -5207,23 +5442,23 @@
 
 SimulatePolicyResponseTypeDef = TypedDict(
     "SimulatePolicyResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountAuthorizationDetailsResponseTypeDef = TypedDict(
     "GetAccountAuthorizationDetailsResponseTypeDef",
     {
         "UserDetailList": List[UserDetailTypeDef],
         "GroupDetailList": List[GroupDetailTypeDef],
         "RoleDetailList": List[RoleDetailTypeDef],
         "Policies": List[ManagedPolicyDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/waiter.py` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam/waiter.pyi` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/PKG-INFO` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iam
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IAM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iam type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iam type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iam"></a>
 
 # types-aiobotocore-iam
 
 [![PyPI - types-aiobotocore-iam](https://img.shields.io/pypi/v/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iam?color=blue)](https://pypistats.org/packages/types-aiobotocore-iam)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iam)](https://pepy.tech/project/types-aiobotocore-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IAM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
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
 [types-aiobotocore-iam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -637,20 +636,20 @@
 )
 
 
 def check_value(value: AccessAdvisorUsageGranularityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iam.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iam.type_defs import (
     AccessDetailTypeDef,
     AccessKeyLastUsedTypeDef,
     AccessKeyMetadataTypeDef,
     AccessKeyTypeDef,
@@ -665,15 +664,15 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
-    AttachedPermissionsBoundaryResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     AttachedPermissionsBoundaryTypeDef,
     AttachedPolicyTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
@@ -685,15 +684,14 @@
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     LoginProfileTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
     ServiceSpecificCredentialTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
@@ -706,15 +704,14 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
     RoleUsageTypeTypeDef,
@@ -723,141 +720,95 @@
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
     EntityInfoTypeDef,
     ErrorDetailsTypeDef,
     OrganizationsDecisionDetailTypeDef,
     PermissionsBoundaryDecisionDetailTypeDef,
-    GenerateCredentialReportResponseTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
-    GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
     PasswordPolicyTypeDef,
-    GetAccountSummaryResponseTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseTypeDef,
-    GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
     SSHPublicKeyTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseTypeDef,
     GetUserRequestRequestTypeDef,
     PolicyDetailTypeDef,
-    ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
-    ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseTypeDef,
-    ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
-    ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
-    ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
-    ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
     PolicyGroupTypeDef,
     PolicyRoleTypeDef,
     PolicyUserTypeDef,
-    ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseTypeDef,
-    ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
-    ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
-    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
-    ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
-    ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
     MFADeviceTypeDef,
-    ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
     OpenIDConnectProviderListEntryTypeDef,
     PolicyGrantingServiceAccessTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
-    ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
-    ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseTypeDef,
-    ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
-    ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
-    ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
     SAMLProviderListEntryTypeDef,
-    ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
     SSHPublicKeyMetadataTypeDef,
-    ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
-    ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
     ServerCertificateMetadataTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
     ServiceSpecificCredentialMetadataTypeDef,
-    ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
     SigningCertificateTypeDef,
-    ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseTypeDef,
-    ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PolicyDocumentStatementTypeDef,
     PositionTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
@@ -868,20 +819,17 @@
     RemoveClientIDFromOpenIDConnectProviderRequestRequestTypeDef,
     RemoveRoleFromInstanceProfileRequestInstanceProfileRemoveRoleTypeDef,
     RemoveRoleFromInstanceProfileRequestRequestTypeDef,
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
     RoleLastUsedTypeDef,
-    RoleLastUsedResponseMetadataTypeDef,
-    ServerCertificateMetadataResponseMetadataTypeDef,
     TrackedActionLastAccessedTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
@@ -904,37 +852,54 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
+    AttachedPermissionsBoundaryResponseTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GenerateCredentialReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedResponseTypeDef,
+    GetAccountSummaryResponseTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
+    GetCredentialReportResponseTypeDef,
+    GetGroupPolicyResponseTypeDef,
+    GetMFADeviceResponseTypeDef,
+    GetRolePolicyResponseTypeDef,
+    GetUserPolicyResponseTypeDef,
     ListAccessKeysResponseTypeDef,
-    CreateAccessKeyResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    RoleLastUsedResponseTypeDef,
+    ServerCertificateMetadataResponseTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     ListAttachedGroupPoliciesResponseTypeDef,
     ListAttachedRolePoliciesResponseTypeDef,
     ListAttachedUserPoliciesResponseTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
-    SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
-    SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     CreateGroupResponseTypeDef,
     ListGroupsForUserResponseTypeDef,
     ListGroupsResponseTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
     CreateOpenIDConnectProviderResponseTypeDef,
@@ -967,27 +932,57 @@
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CreateLoginProfileResponseTypeDef,
     GetLoginProfileResponseTypeDef,
-    CreatePolicyVersionResponseTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    ListPolicyVersionsResponseTypeDef,
-    ManagedPolicyDetailTypeDef,
     CreateServiceSpecificCredentialResponseTypeDef,
     ResetServiceSpecificCredentialResponseTypeDef,
     DeletionTaskFailureReasonTypeTypeDef,
     EntityDetailsTypeDef,
     GetOrganizationsAccessReportResponseTypeDef,
+    GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
+    GetGroupRequestGetGroupPaginateTypeDef,
+    ListAccessKeysRequestListAccessKeysPaginateTypeDef,
+    ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
+    ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
+    ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
+    ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
+    ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
+    ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
+    ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
+    ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
+    ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
+    ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
+    ListMFADevicesRequestListMFADevicesPaginateTypeDef,
+    ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
+    ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
+    ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
+    ListRoleTagsRequestListRoleTagsPaginateTypeDef,
+    ListRolesRequestListRolesPaginateTypeDef,
+    ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
+    ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
+    ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
+    ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
+    ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
+    ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
+    ListUserTagsRequestListUserTagsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
+    SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
+    SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     GetAccountPasswordPolicyResponseTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
     GetSSHPublicKeyResponseTypeDef,
     UploadSSHPublicKeyResponseTypeDef,
@@ -1001,14 +996,15 @@
     ListSSHPublicKeysResponseTypeDef,
     ListServerCertificatesResponseTypeDef,
     ServerCertificateTypeDef,
     UploadServerCertificateResponseTypeDef,
     ListServiceSpecificCredentialsResponseTypeDef,
     ListSigningCertificatesResponseTypeDef,
     UploadSigningCertificateResponseTypeDef,
+    PolicyDocumentFixedTypeDef,
     StatementTypeDef,
     RoleTypeDef,
     ServiceLastAccessedTypeDef,
     CreatePolicyResponseTypeDef,
     GetPolicyResponseTypeDef,
     ListPoliciesResponseTypeDef,
     CreateUserResponseTypeDef,
@@ -1016,36 +1012,41 @@
     GetUserResponseTypeDef,
     ListUsersResponseTypeDef,
     VirtualMFADeviceTypeDef,
     GetServiceLinkedRoleDeletionStatusResponseTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
     ListPoliciesGrantingServiceAccessResponseTypeDef,
     GetServerCertificateResponseTypeDef,
+    PolicyVersionTypeDef,
     ResourceSpecificResultTypeDef,
     CreateRoleResponseTypeDef,
     CreateServiceLinkedRoleResponseTypeDef,
     GetRoleResponseTypeDef,
     InstanceProfileTypeDef,
     ListRolesResponseTypeDef,
     UpdateRoleDescriptionResponseTypeDef,
     GetServiceLastAccessedDetailsResponseTypeDef,
     CreateVirtualMFADeviceResponseTypeDef,
     ListVirtualMFADevicesResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ManagedPolicyDetailTypeDef,
     EvaluationResultTypeDef,
     CreateInstanceProfileResponseTypeDef,
     GetInstanceProfileResponseTypeDef,
     ListInstanceProfilesForRoleResponseTypeDef,
     ListInstanceProfilesResponseTypeDef,
     RoleDetailTypeDef,
     SimulatePolicyResponseTypeDef,
     GetAccountAuthorizationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessDetailTypeDef:
+def get_value() -> AccessDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iam-2.5.2/types_aiobotocore_iam.egg-info/SOURCES.txt` & `types-aiobotocore-iam-2.5.2.post1/types_aiobotocore_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*


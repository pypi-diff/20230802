# Comparing `tmp/types-aiobotocore-managedblockchain-2.5.2.tar.gz` & `tmp/types-aiobotocore-managedblockchain-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-managedblockchain-2.5.2.tar", last modified: Sat Jul  8 01:43:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-managedblockchain-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:37 2023, max compression
```

## Comparing `types-aiobotocore-managedblockchain-2.5.2.tar` & `types-aiobotocore-managedblockchain-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:57.266501 types-aiobotocore-managedblockchain-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-07-08 01:43:57.266501 types-aiobotocore-managedblockchain-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:57.266501 types-aiobotocore-managedblockchain-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:57.266501 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26482 2023-07-08 01:34:37.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26453 2023-07-08 01:34:37.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:36.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:57.266501 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-07-08 01:43:57.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:57.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:57.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:57.000000 types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26824 2023-08-02 14:42:49.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/LICENSE` & `types-aiobotocore-managedblockchain-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2/PKG-INFO` & `types-aiobotocore-managedblockchain-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore managedblockchain type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-managedblockchain"></a>
 
 # types-aiobotocore-managedblockchain
 
 [![PyPI - types-aiobotocore-managedblockchain](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-managedblockchain?color=blue)](https://pypistats.org/packages/types-aiobotocore-managedblockchain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ManagedBlockchain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
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
@@ -317,93 +316,95 @@
 )
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_managedblockchain.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
     InviteActionTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
-    PaginatorConfigTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    ListAccessorsOutputTypeDef,
-    GetAccessorOutputTypeDef,
     VotingPolicyTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
+    GetAccessorOutputTypeDef,
+    ListAccessorsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
+    ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
-    CreateProposalInputRequestTypeDef,
     ProposalTypeDef,
+    CreateProposalInputRequestTypeDef,
+    ProposalActionsUnionTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
     MemberConfigurationTypeDef,
     MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
@@ -414,15 +415,15 @@
     CreateNetworkInputRequestTypeDef,
     GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
     GetNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AccessorSummaryTypeDef:
+def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/README.md` & `types-aiobotocore-managedblockchain-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-managedblockchain"></a>
 
 # types-aiobotocore-managedblockchain
 
 [![PyPI - types-aiobotocore-managedblockchain](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-managedblockchain?color=blue)](https://pypistats.org/packages/types-aiobotocore-managedblockchain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ManagedBlockchain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
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
@@ -284,93 +284,95 @@
 )
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_managedblockchain.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
     InviteActionTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
-    PaginatorConfigTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    ListAccessorsOutputTypeDef,
-    GetAccessorOutputTypeDef,
     VotingPolicyTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
+    GetAccessorOutputTypeDef,
+    ListAccessorsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
+    ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
-    CreateProposalInputRequestTypeDef,
     ProposalTypeDef,
+    CreateProposalInputRequestTypeDef,
+    ProposalActionsUnionTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
     MemberConfigurationTypeDef,
     MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
@@ -381,15 +383,15 @@
     CreateNetworkInputRequestTypeDef,
     GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
     GetNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AccessorSummaryTypeDef:
+def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/setup.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-managedblockchain",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with"
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
-        "aiobotocore managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore managedblockchain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_managedblockchain": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/"
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/__init__.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/__init__.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/__main__.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ManagedBlockchain 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ManagedBlockchain 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/client.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsTypeDef,
+    ProposalActionsUnionTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -187,15 +187,15 @@
 
     async def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: ProposalActionsTypeDef,
+        Actions: ProposalActionsUnionTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/client.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsTypeDef,
+    ProposalActionsUnionTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -176,15 +176,15 @@
         """
     async def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: ProposalActionsTypeDef,
+        Actions: ProposalActionsUnionTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/literals.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/literals.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/paginator.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListAccessorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/paginator.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListAccessorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain.Paginator.ListAccessors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/paginators/#listaccessorspaginator)
         """
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/type_defs.py` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_managedblockchain.type_defs import AccessorSummaryTypeDef
 
-    data: AccessorSummaryTypeDef = {...}
+    data: AccessorSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
     MemberStatusType,
@@ -40,80 +40,82 @@
 
 
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
-    "CreateAccessorOutputTypeDef",
-    "CreateMemberOutputTypeDef",
-    "CreateNetworkOutputTypeDef",
-    "CreateNodeOutputTypeDef",
-    "CreateProposalOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
     "InviteActionTypeDef",
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
     "ListNodesInputRequestTypeDef",
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
-    "ListAccessorsOutputTypeDef",
-    "GetAccessorOutputTypeDef",
     "VotingPolicyTypeDef",
+    "CreateAccessorOutputTypeDef",
+    "CreateMemberOutputTypeDef",
+    "CreateNetworkOutputTypeDef",
+    "CreateNodeOutputTypeDef",
+    "CreateProposalOutputTypeDef",
+    "GetAccessorOutputTypeDef",
+    "ListAccessorsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
+    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "CreateProposalInputRequestTypeDef",
     "ProposalTypeDef",
+    "CreateProposalInputRequestTypeDef",
+    "ProposalActionsUnionTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -181,53 +183,22 @@
 
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
 
-CreateAccessorOutputTypeDef = TypedDict(
-    "CreateAccessorOutputTypeDef",
-    {
-        "AccessorId": str,
-        "BillingToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMemberOutputTypeDef = TypedDict(
-    "CreateMemberOutputTypeDef",
-    {
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkOutputTypeDef = TypedDict(
-    "CreateNetworkOutputTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNodeOutputTypeDef = TypedDict(
-    "CreateNodeOutputTypeDef",
-    {
-        "NodeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProposalOutputTypeDef = TypedDict(
-    "CreateProposalOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProposalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
@@ -334,18 +305,20 @@
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
-ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
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
 
 ListAccessorsInputRequestTypeDef = TypedDict(
     "ListAccessorsInputRequestTypeDef",
     {
@@ -525,22 +498,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -600,49 +565,28 @@
     {
         "PeerEndpoint": str,
         "PeerEventEndpoint": str,
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
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
 RejectInvitationInputRequestTypeDef = TypedDict(
     "RejectInvitationInputRequestTypeDef",
     {
         "InvitationId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -661,37 +605,87 @@
         "NetworkId": str,
         "ProposalId": str,
         "VoterMemberId": str,
         "Vote": VoteValueType,
     },
 )
 
-ListAccessorsOutputTypeDef = TypedDict(
-    "ListAccessorsOutputTypeDef",
+VotingPolicyTypeDef = TypedDict(
+    "VotingPolicyTypeDef",
     {
-        "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+    },
+    total=False,
+)
+
+CreateAccessorOutputTypeDef = TypedDict(
+    "CreateAccessorOutputTypeDef",
+    {
+        "AccessorId": str,
+        "BillingToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberOutputTypeDef = TypedDict(
+    "CreateMemberOutputTypeDef",
+    {
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkOutputTypeDef = TypedDict(
+    "CreateNetworkOutputTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeOutputTypeDef = TypedDict(
+    "CreateNodeOutputTypeDef",
+    {
+        "NodeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProposalOutputTypeDef = TypedDict(
+    "CreateProposalOutputTypeDef",
+    {
+        "ProposalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessorOutputTypeDef = TypedDict(
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VotingPolicyTypeDef = TypedDict(
-    "VotingPolicyTypeDef",
+ListAccessorsOutputTypeDef = TypedDict(
+    "ListAccessorsOutputTypeDef",
     {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+        "Accessors": List[AccessorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 InvitationTypeDef = TypedDict(
     "InvitationTypeDef",
     {
         "InvitationId": str,
         "CreationDate": datetime,
@@ -704,51 +698,59 @@
 )
 
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
@@ -794,29 +796,38 @@
     {
         "Fabric": NodeFabricAttributesTypeDef,
         "Ethereum": NodeEthereumAttributesTypeDef,
     },
     total=False,
 )
 
+ProposalActionsOutputTypeDef = TypedDict(
+    "ProposalActionsOutputTypeDef",
+    {
+        "Invitations": List[InviteActionTypeDef],
+        "Removals": List[RemoveActionTypeDef],
+    },
+    total=False,
+)
+
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": Sequence[InviteActionTypeDef],
         "Removals": Sequence[RemoveActionTypeDef],
     },
     total=False,
 )
 
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
@@ -848,14 +859,35 @@
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
 
+ProposalTypeDef = TypedDict(
+    "ProposalTypeDef",
+    {
+        "ProposalId": str,
+        "NetworkId": str,
+        "Description": str,
+        "Actions": ProposalActionsOutputTypeDef,
+        "ProposedByMemberId": str,
+        "ProposedByMemberName": str,
+        "Status": ProposalStatusType,
+        "CreationDate": datetime,
+        "ExpirationDate": datetime,
+        "YesVoteCount": int,
+        "NoVoteCount": int,
+        "OutstandingVoteCount": int,
+        "Tags": Dict[str, str],
+        "Arn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateProposalInputRequestTypeDef = TypedDict(
     "_RequiredCreateProposalInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "MemberId": str,
         "Actions": ProposalActionsTypeDef,
@@ -873,35 +905,15 @@
 
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
 
-ProposalTypeDef = TypedDict(
-    "ProposalTypeDef",
-    {
-        "ProposalId": str,
-        "NetworkId": str,
-        "Description": str,
-        "Actions": ProposalActionsTypeDef,
-        "ProposedByMemberId": str,
-        "ProposedByMemberName": str,
-        "Status": ProposalStatusType,
-        "CreationDate": datetime,
-        "ExpirationDate": datetime,
-        "YesVoteCount": int,
-        "NoVoteCount": int,
-        "OutstandingVoteCount": int,
-        "Tags": Dict[str, str],
-        "Arn": str,
-    },
-    total=False,
-)
-
+ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -914,23 +926,23 @@
     total=False,
 )
 
 GetNetworkOutputTypeDef = TypedDict(
     "GetNetworkOutputTypeDef",
     {
         "Network": NetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProposalOutputTypeDef = TypedDict(
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
@@ -1099,15 +1111,15 @@
     pass
 
 
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
@@ -1131,10 +1143,10 @@
     pass
 
 
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain/type_defs.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_managedblockchain.type_defs import AccessorSummaryTypeDef
 
-    data: AccessorSummaryTypeDef = {...}
+    data: AccessorSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
     MemberStatusType,
@@ -39,80 +39,82 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
-    "CreateAccessorOutputTypeDef",
-    "CreateMemberOutputTypeDef",
-    "CreateNetworkOutputTypeDef",
-    "CreateNodeOutputTypeDef",
-    "CreateProposalOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
     "DeleteMemberInputRequestTypeDef",
     "DeleteNodeInputRequestTypeDef",
     "GetAccessorInputRequestTypeDef",
     "GetMemberInputRequestTypeDef",
     "GetNetworkInputRequestTypeDef",
     "GetNodeInputRequestTypeDef",
     "GetProposalInputRequestTypeDef",
     "NetworkSummaryTypeDef",
     "InviteActionTypeDef",
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessorsInputRequestTypeDef",
     "ListInvitationsInputRequestTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
     "ListNetworksInputRequestTypeDef",
     "ListNodesInputRequestTypeDef",
     "NodeSummaryTypeDef",
     "ListProposalVotesInputRequestTypeDef",
     "VoteSummaryTypeDef",
     "ListProposalsInputRequestTypeDef",
     "ProposalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "LogConfigurationTypeDef",
     "MemberFabricAttributesTypeDef",
     "MemberFabricConfigurationTypeDef",
     "NetworkEthereumAttributesTypeDef",
     "NetworkFabricAttributesTypeDef",
     "NetworkFabricConfigurationTypeDef",
     "NodeEthereumAttributesTypeDef",
     "NodeFabricAttributesTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveActionTypeDef",
     "RejectInvitationInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VoteOnProposalInputRequestTypeDef",
-    "ListAccessorsOutputTypeDef",
-    "GetAccessorOutputTypeDef",
     "VotingPolicyTypeDef",
+    "CreateAccessorOutputTypeDef",
+    "CreateMemberOutputTypeDef",
+    "CreateNetworkOutputTypeDef",
+    "CreateNodeOutputTypeDef",
+    "CreateProposalOutputTypeDef",
+    "GetAccessorOutputTypeDef",
+    "ListAccessorsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "InvitationTypeDef",
     "ListNetworksOutputTypeDef",
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListNodesOutputTypeDef",
     "ListProposalVotesOutputTypeDef",
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
+    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "CreateProposalInputRequestTypeDef",
     "ProposalTypeDef",
+    "CreateProposalInputRequestTypeDef",
+    "ProposalActionsUnionTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -178,53 +180,22 @@
 )
 
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
-CreateAccessorOutputTypeDef = TypedDict(
-    "CreateAccessorOutputTypeDef",
-    {
-        "AccessorId": str,
-        "BillingToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMemberOutputTypeDef = TypedDict(
-    "CreateMemberOutputTypeDef",
-    {
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNetworkOutputTypeDef = TypedDict(
-    "CreateNetworkOutputTypeDef",
-    {
-        "NetworkId": str,
-        "MemberId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateNodeOutputTypeDef = TypedDict(
-    "CreateNodeOutputTypeDef",
-    {
-        "NodeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateProposalOutputTypeDef = TypedDict(
-    "CreateProposalOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ProposalId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteAccessorInputRequestTypeDef = TypedDict(
     "DeleteAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
@@ -327,18 +298,20 @@
 InviteActionTypeDef = TypedDict(
     "InviteActionTypeDef",
     {
         "Principal": str,
     },
 )
 
-ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
-    "ListAccessorsInputListAccessorsPaginateTypeDef",
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
 
 ListAccessorsInputRequestTypeDef = TypedDict(
     "ListAccessorsInputRequestTypeDef",
     {
@@ -510,22 +483,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LogConfigurationTypeDef = TypedDict(
     "LogConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -585,49 +550,28 @@
     {
         "PeerEndpoint": str,
         "PeerEventEndpoint": str,
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
 RemoveActionTypeDef = TypedDict(
     "RemoveActionTypeDef",
     {
         "MemberId": str,
     },
 )
 
 RejectInvitationInputRequestTypeDef = TypedDict(
     "RejectInvitationInputRequestTypeDef",
     {
         "InvitationId": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -646,37 +590,87 @@
         "NetworkId": str,
         "ProposalId": str,
         "VoterMemberId": str,
         "Vote": VoteValueType,
     },
 )
 
-ListAccessorsOutputTypeDef = TypedDict(
-    "ListAccessorsOutputTypeDef",
+VotingPolicyTypeDef = TypedDict(
+    "VotingPolicyTypeDef",
     {
-        "Accessors": List[AccessorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+    },
+    total=False,
+)
+
+CreateAccessorOutputTypeDef = TypedDict(
+    "CreateAccessorOutputTypeDef",
+    {
+        "AccessorId": str,
+        "BillingToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberOutputTypeDef = TypedDict(
+    "CreateMemberOutputTypeDef",
+    {
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkOutputTypeDef = TypedDict(
+    "CreateNetworkOutputTypeDef",
+    {
+        "NetworkId": str,
+        "MemberId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeOutputTypeDef = TypedDict(
+    "CreateNodeOutputTypeDef",
+    {
+        "NodeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProposalOutputTypeDef = TypedDict(
+    "CreateProposalOutputTypeDef",
+    {
+        "ProposalId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessorOutputTypeDef = TypedDict(
     "GetAccessorOutputTypeDef",
     {
         "Accessor": AccessorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VotingPolicyTypeDef = TypedDict(
-    "VotingPolicyTypeDef",
+ListAccessorsOutputTypeDef = TypedDict(
+    "ListAccessorsOutputTypeDef",
     {
-        "ApprovalThresholdPolicy": ApprovalThresholdPolicyTypeDef,
+        "Accessors": List[AccessorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 InvitationTypeDef = TypedDict(
     "InvitationTypeDef",
     {
         "InvitationId": str,
         "CreationDate": datetime,
@@ -689,51 +683,59 @@
 )
 
 ListNetworksOutputTypeDef = TypedDict(
     "ListNetworksOutputTypeDef",
     {
         "Networks": List[NetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAccessorsInputListAccessorsPaginateTypeDef = TypedDict(
+    "ListAccessorsInputListAccessorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "Members": List[MemberSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesOutputTypeDef = TypedDict(
     "ListNodesOutputTypeDef",
     {
         "Nodes": List[NodeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalVotesOutputTypeDef = TypedDict(
     "ListProposalVotesOutputTypeDef",
     {
         "ProposalVotes": List[VoteSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProposalsOutputTypeDef = TypedDict(
     "ListProposalsOutputTypeDef",
     {
         "Proposals": List[ProposalSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LogConfigurationsTypeDef = TypedDict(
     "LogConfigurationsTypeDef",
     {
         "Cloudwatch": LogConfigurationTypeDef,
@@ -779,29 +781,38 @@
     {
         "Fabric": NodeFabricAttributesTypeDef,
         "Ethereum": NodeEthereumAttributesTypeDef,
     },
     total=False,
 )
 
+ProposalActionsOutputTypeDef = TypedDict(
+    "ProposalActionsOutputTypeDef",
+    {
+        "Invitations": List[InviteActionTypeDef],
+        "Removals": List[RemoveActionTypeDef],
+    },
+    total=False,
+)
+
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": Sequence[InviteActionTypeDef],
         "Removals": Sequence[RemoveActionTypeDef],
     },
     total=False,
 )
 
 ListInvitationsOutputTypeDef = TypedDict(
     "ListInvitationsOutputTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MemberFabricLogPublishingConfigurationTypeDef = TypedDict(
     "MemberFabricLogPublishingConfigurationTypeDef",
     {
         "CaLogs": LogConfigurationsTypeDef,
@@ -833,14 +844,35 @@
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
 
+ProposalTypeDef = TypedDict(
+    "ProposalTypeDef",
+    {
+        "ProposalId": str,
+        "NetworkId": str,
+        "Description": str,
+        "Actions": ProposalActionsOutputTypeDef,
+        "ProposedByMemberId": str,
+        "ProposedByMemberName": str,
+        "Status": ProposalStatusType,
+        "CreationDate": datetime,
+        "ExpirationDate": datetime,
+        "YesVoteCount": int,
+        "NoVoteCount": int,
+        "OutstandingVoteCount": int,
+        "Tags": Dict[str, str],
+        "Arn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateProposalInputRequestTypeDef = TypedDict(
     "_RequiredCreateProposalInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "MemberId": str,
         "Actions": ProposalActionsTypeDef,
@@ -856,35 +888,15 @@
 )
 
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
-ProposalTypeDef = TypedDict(
-    "ProposalTypeDef",
-    {
-        "ProposalId": str,
-        "NetworkId": str,
-        "Description": str,
-        "Actions": ProposalActionsTypeDef,
-        "ProposedByMemberId": str,
-        "ProposedByMemberName": str,
-        "Status": ProposalStatusType,
-        "CreationDate": datetime,
-        "ExpirationDate": datetime,
-        "YesVoteCount": int,
-        "NoVoteCount": int,
-        "OutstandingVoteCount": int,
-        "Tags": Dict[str, str],
-        "Arn": str,
-    },
-    total=False,
-)
-
+ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -897,23 +909,23 @@
     total=False,
 )
 
 GetNetworkOutputTypeDef = TypedDict(
     "GetNetworkOutputTypeDef",
     {
         "Network": NetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProposalOutputTypeDef = TypedDict(
     "GetProposalOutputTypeDef",
     {
         "Proposal": ProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMemberConfigurationTypeDef = TypedDict(
     "_RequiredMemberConfigurationTypeDef",
     {
         "Name": str,
@@ -1072,15 +1084,15 @@
 ):
     pass
 
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateNodeInputRequestTypeDef",
     {
         "ClientRequestToken": str,
@@ -1102,10 +1114,10 @@
 ):
     pass
 
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/PKG-INFO` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-managedblockchain
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore managedblockchain type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore managedblockchain type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-managedblockchain"></a>
 
 # types-aiobotocore-managedblockchain
 
 [![PyPI - types-aiobotocore-managedblockchain](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-managedblockchain?color=blue)](https://pypistats.org/packages/types-aiobotocore-managedblockchain)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-managedblockchain)](https://pepy.tech/project/types-aiobotocore-managedblockchain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ManagedBlockchain 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain)
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
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
@@ -317,93 +316,95 @@
 )
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_managedblockchain.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_managedblockchain.type_defs import (
     AccessorSummaryTypeDef,
     AccessorTypeDef,
     ApprovalThresholdPolicyTypeDef,
     CreateAccessorInputRequestTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteAccessorInputRequestTypeDef,
     DeleteMemberInputRequestTypeDef,
     DeleteNodeInputRequestTypeDef,
     GetAccessorInputRequestTypeDef,
     GetMemberInputRequestTypeDef,
     GetNetworkInputRequestTypeDef,
     GetNodeInputRequestTypeDef,
     GetProposalInputRequestTypeDef,
     NetworkSummaryTypeDef,
     InviteActionTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessorsInputRequestTypeDef,
     ListInvitationsInputRequestTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
     ListNetworksInputRequestTypeDef,
     ListNodesInputRequestTypeDef,
     NodeSummaryTypeDef,
     ListProposalVotesInputRequestTypeDef,
     VoteSummaryTypeDef,
     ListProposalsInputRequestTypeDef,
     ProposalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     LogConfigurationTypeDef,
     MemberFabricAttributesTypeDef,
     MemberFabricConfigurationTypeDef,
     NetworkEthereumAttributesTypeDef,
     NetworkFabricAttributesTypeDef,
     NetworkFabricConfigurationTypeDef,
     NodeEthereumAttributesTypeDef,
     NodeFabricAttributesTypeDef,
-    PaginatorConfigTypeDef,
     RemoveActionTypeDef,
     RejectInvitationInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VoteOnProposalInputRequestTypeDef,
-    ListAccessorsOutputTypeDef,
-    GetAccessorOutputTypeDef,
     VotingPolicyTypeDef,
+    CreateAccessorOutputTypeDef,
+    CreateMemberOutputTypeDef,
+    CreateNetworkOutputTypeDef,
+    CreateNodeOutputTypeDef,
+    CreateProposalOutputTypeDef,
+    GetAccessorOutputTypeDef,
+    ListAccessorsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     InvitationTypeDef,
     ListNetworksOutputTypeDef,
+    ListAccessorsInputListAccessorsPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListNodesOutputTypeDef,
     ListProposalVotesOutputTypeDef,
     ListProposalsOutputTypeDef,
     LogConfigurationsTypeDef,
     MemberFrameworkAttributesTypeDef,
     MemberFrameworkConfigurationTypeDef,
     NetworkFrameworkAttributesTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeFrameworkAttributesTypeDef,
+    ProposalActionsOutputTypeDef,
     ProposalActionsTypeDef,
     ListInvitationsOutputTypeDef,
     MemberFabricLogPublishingConfigurationTypeDef,
     NodeFabricLogPublishingConfigurationTypeDef,
     NetworkTypeDef,
-    CreateProposalInputRequestTypeDef,
     ProposalTypeDef,
+    CreateProposalInputRequestTypeDef,
+    ProposalActionsUnionTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
     GetNetworkOutputTypeDef,
     GetProposalOutputTypeDef,
     MemberConfigurationTypeDef,
     MemberTypeDef,
     UpdateMemberInputRequestTypeDef,
@@ -414,15 +415,15 @@
     CreateNetworkInputRequestTypeDef,
     GetMemberOutputTypeDef,
     CreateNodeInputRequestTypeDef,
     GetNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AccessorSummaryTypeDef:
+def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt` & `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*


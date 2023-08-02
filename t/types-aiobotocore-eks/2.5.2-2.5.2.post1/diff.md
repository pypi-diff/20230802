# Comparing `tmp/types-aiobotocore-eks-2.5.2.tar.gz` & `tmp/types-aiobotocore-eks-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-eks-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-eks-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-eks-2.5.2.tar` & `types-aiobotocore-eks-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.186085 types-aiobotocore-eks-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-07-08 01:43:35.186085 types-aiobotocore-eks-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.186085 types-aiobotocore-eks-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.182085 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-07-08 01:30:16.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35095 2023-07-08 01:30:16.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-07-08 01:30:17.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-08 01:30:17.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-08 01:30:16.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-08 01:30:16.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50700 2023-07-08 01:30:18.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50627 2023-07-08 01:30:17.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:15.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-08 01:30:17.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-08 01:30:17.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.186085 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21115 2023-07-08 01:43:35.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:35.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:35.000000 types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.561594 types-aiobotocore-eks-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-08-02 14:52:14.557594 types-aiobotocore-eks-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.561594 types-aiobotocore-eks-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.557594 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35204 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-02 14:38:04.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52219 2023-08-02 14:38:06.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52146 2023-08-02 14:38:04.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.557594 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-eks-2.5.2/LICENSE` & `types-aiobotocore-eks-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/PKG-INFO` & `types-aiobotocore-eks-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-eks
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore eks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore eks type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-eks"></a>
 
 # types-aiobotocore-eks
 
 [![PyPI - types-aiobotocore-eks](https://img.shields.io/pypi/v/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-eks?color=blue)](https://pypistats.org/packages/types-aiobotocore-eks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EKS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [types-aiobotocore-eks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/).
 
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
@@ -400,161 +399,170 @@
 )
 
 
 def check_value(value: AMITypesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_eks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
+    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
-    FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    FargateProfileSelectorTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
-    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
-    ListUpdatesResponseTypeDef,
+    LogSetupOutputTypeDef,
     LogSetupTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RemoteAccessConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListNodegroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
-    CreateFargateProfileRequestRequestTypeDef,
-    FargateProfileTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    EncryptionConfigUnionTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateFargateProfileRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
-    CreateClusterRequestRequestTypeDef,
+    LoggingUnionTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
     CreateAddonResponseTypeDef,
     DeleteAddonResponseTypeDef,
     DescribeAddonResponseTypeDef,
     DescribeAddonVersionsResponseTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
     CreateNodegroupResponseTypeDef,
     DeleteNodegroupResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeregisterClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     RegisterClusterResponseTypeDef,
 )
 
 
-def get_structure() -> AddonIssueTypeDef:
+def get_value() -> AddonIssueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-eks-2.5.2/README.md` & `types-aiobotocore-eks-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-eks"></a>
 
 # types-aiobotocore-eks
 
 [![PyPI - types-aiobotocore-eks](https://img.shields.io/pypi/v/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-eks?color=blue)](https://pypistats.org/packages/types-aiobotocore-eks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EKS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [types-aiobotocore-eks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/).
 
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
@@ -367,161 +367,170 @@
 )
 
 
 def check_value(value: AMITypesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_eks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
+    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
-    FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    FargateProfileSelectorTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
-    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
-    ListUpdatesResponseTypeDef,
+    LogSetupOutputTypeDef,
     LogSetupTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RemoteAccessConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListNodegroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
-    CreateFargateProfileRequestRequestTypeDef,
-    FargateProfileTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    EncryptionConfigUnionTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateFargateProfileRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
-    CreateClusterRequestRequestTypeDef,
+    LoggingUnionTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
     CreateAddonResponseTypeDef,
     DeleteAddonResponseTypeDef,
     DescribeAddonResponseTypeDef,
     DescribeAddonVersionsResponseTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
     CreateNodegroupResponseTypeDef,
     DeleteNodegroupResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeregisterClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     RegisterClusterResponseTypeDef,
 )
 
 
-def get_structure() -> AddonIssueTypeDef:
+def get_value() -> AddonIssueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-eks-2.5.2/setup.py` & `types-aiobotocore-eks-2.5.2.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-eks",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore eks type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore eks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_eks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/__init__.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/__init__.pyi` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/__main__.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EKS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.EKS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
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

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/client.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,33 +48,33 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
-    EncryptionConfigTypeDef,
-    FargateProfileSelectorTypeDef,
+    EncryptionConfigUnionTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
-    LoggingTypeDef,
+    LoggingUnionTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
-    RemoteAccessConfigTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
@@ -143,15 +143,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#exceptions)
         """
 
     async def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef],
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_encryption_config)
@@ -211,18 +211,18 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_cluster)
@@ -231,15 +231,15 @@
     async def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
+        selectors: Sequence[FargateProfileSelectorUnionTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -253,15 +253,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: RemoteAccessConfigTypeDef = ...,
+        remoteAccess: RemoteAccessConfigUnionTypeDef = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -566,15 +566,15 @@
         """
 
     async def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_cluster_config)
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/client.pyi` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,33 +48,33 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
-    EncryptionConfigTypeDef,
-    FargateProfileSelectorTypeDef,
+    EncryptionConfigUnionTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
-    LoggingTypeDef,
+    LoggingUnionTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
-    RemoteAccessConfigTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
@@ -138,15 +138,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#exceptions)
         """
     async def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef],
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_encryption_config)
@@ -201,18 +201,18 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
+        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_cluster)
@@ -220,15 +220,15 @@
     async def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
+        selectors: Sequence[FargateProfileSelectorUnionTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -241,15 +241,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: RemoteAccessConfigTypeDef = ...,
+        remoteAccess: RemoteAccessConfigUnionTypeDef = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -527,15 +527,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_addon)
         """
     async def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: LoggingTypeDef = ...,
+        logging: LoggingUnionTypeDef = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_cluster_config)
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/literals.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/literals.pyi` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/paginator.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,133 +54,124 @@
     "ListClustersPaginator",
     "ListFargateProfilesPaginator",
     "ListIdentityProviderConfigsPaginator",
     "ListNodegroupsPaginator",
     "ListUpdatesPaginator",
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
 class DescribeAddonVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#describeaddonversionspaginator)
     """
 
     def paginate(
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#describeaddonversionspaginator)
         """
 
-
 class ListAddonsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listaddonspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAddonsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listaddonspaginator)
         """
 
-
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, include: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, include: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listclusterspaginator)
         """
 
-
 class ListFargateProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listfargateprofilespaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFargateProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listfargateprofilespaginator)
         """
 
-
 class ListIdentityProviderConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listidentityproviderconfigspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityProviderConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listidentityproviderconfigspaginator)
         """
 
-
 class ListNodegroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listnodegroupspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNodegroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listnodegroupspaginator)
         """
 
-
 class ListUpdatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/paginator.pyi` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,124 +54,133 @@
     "ListClustersPaginator",
     "ListFargateProfilesPaginator",
     "ListIdentityProviderConfigsPaginator",
     "ListNodegroupsPaginator",
     "ListUpdatesPaginator",
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
 class DescribeAddonVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#describeaddonversionspaginator)
     """
 
     def paginate(
         self,
         *,
         kubernetesVersion: str = ...,
         addonName: str = ...,
         types: Sequence[str] = ...,
         publishers: Sequence[str] = ...,
         owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAddonVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.DescribeAddonVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#describeaddonversionspaginator)
         """
 
+
 class ListAddonsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listaddonspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAddonsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListAddons.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listaddonspaginator)
         """
 
+
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, include: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, include: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listclusterspaginator)
         """
 
+
 class ListFargateProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listfargateprofilespaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFargateProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListFargateProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listfargateprofilespaginator)
         """
 
+
 class ListIdentityProviderConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listidentityproviderconfigspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentityProviderConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListIdentityProviderConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listidentityproviderconfigspaginator)
         """
 
+
 class ListNodegroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listnodegroupspaginator)
     """
 
     def paginate(
-        self, *, clusterName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNodegroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListNodegroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listnodegroupspaginator)
         """
 
+
 class ListUpdatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         name: str,
         nodegroupName: str = ...,
         addonName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Paginator.ListUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/paginators/#listupdatespaginator)
         """
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/type_defs.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_eks.type_defs import AddonIssueTypeDef
 
-    data: AddonIssueTypeDef = {...}
+    data: AddonIssueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AddonIssueCodeType,
     AddonStatusType,
     AMITypesType,
     CapacityTypesType,
     ClusterIssueCodeType,
@@ -43,137 +43,146 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
+    "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "CertificateTypeDef",
     "ClusterIssueTypeDef",
     "ConnectorConfigResponseTypeDef",
     "KubernetesNetworkConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
-    "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteFargateProfileRequestRequestTypeDef",
     "DeleteNodegroupRequestRequestTypeDef",
     "DeregisterClusterRequestRequestTypeDef",
     "DescribeAddonConfigurationRequestRequestTypeDef",
-    "DescribeAddonConfigurationResponseTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAddonRequestRequestTypeDef",
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
+    "FargateProfileSelectorTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
-    "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
-    "ListAddonsResponseTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
-    "ListFargateProfilesResponseTypeDef",
-    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
-    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
-    "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
-    "ListUpdatesResponseTypeDef",
+    "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "RemoteAccessConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
     "AddonVersionInfoTypeDef",
+    "DescribeAddonConfigurationResponseTypeDef",
+    "ListAddonsResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListFargateProfilesResponseTypeDef",
+    "ListNodegroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
-    "CreateFargateProfileRequestRequestTypeDef",
-    "FargateProfileTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "ListAddonsRequestListAddonsPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "FargateProfileTypeDef",
+    "FargateProfileSelectorUnionTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
+    "LoggingOutputTypeDef",
     "LoggingTypeDef",
+    "RemoteAccessConfigUnionTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "EncryptionConfigUnionTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateFargateProfileRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
-    "CreateClusterRequestRequestTypeDef",
+    "LoggingUnionTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
     "DescribeUpdateResponseTypeDef",
     "DisassociateIdentityProviderConfigResponseTypeDef",
     "UpdateAddonResponseTypeDef",
     "UpdateClusterConfigResponseTypeDef",
     "UpdateClusterVersionResponseTypeDef",
     "UpdateNodegroupConfigResponseTypeDef",
     "UpdateNodegroupVersionResponseTypeDef",
     "CreateAddonResponseTypeDef",
     "DeleteAddonResponseTypeDef",
     "DescribeAddonResponseTypeDef",
     "DescribeAddonVersionsResponseTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateClusterRequestRequestTypeDef",
     "CreateNodegroupResponseTypeDef",
     "DeleteNodegroupResponseTypeDef",
     "DescribeNodegroupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeregisterClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -205,14 +214,25 @@
         "clusterVersion": str,
         "platformVersions": List[str],
         "defaultVersion": bool,
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
 _RequiredOidcIdentityProviderConfigRequestTypeDef = TypedDict(
     "_RequiredOidcIdentityProviderConfigRequestTypeDef",
     {
         "identityProviderConfigName": str,
         "issuerUrl": str,
         "clientId": str,
     },
@@ -367,23 +387,14 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
-FargateProfileSelectorTypeDef = TypedDict(
-    "FargateProfileSelectorTypeDef",
-    {
-        "namespace": str,
-        "labels": Mapping[str, str],
-    },
-    total=False,
-)
-
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "name": str,
         "version": str,
         "id": str,
     },
@@ -484,24 +495,14 @@
     "DescribeAddonConfigurationRequestRequestTypeDef",
     {
         "addonName": str,
         "addonVersion": str,
     },
 )
 
-DescribeAddonConfigurationResponseTypeDef = TypedDict(
-    "DescribeAddonConfigurationResponseTypeDef",
-    {
-        "addonName": str,
-        "addonVersion": str,
-        "configurationSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -511,23 +512,20 @@
     "DescribeAddonRequestRequestTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
 
-DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "kubernetesVersion": str,
-        "addonName": str,
-        "types": Sequence[str],
-        "publishers": Sequence[str],
-        "owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAddonVersionsRequestRequestTypeDef = TypedDict(
     "DescribeAddonVersionsRequestRequestTypeDef",
     {
@@ -610,14 +608,32 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorTypeDef = TypedDict(
+    "FargateProfileSelectorTypeDef",
+    {
+        "namespace": str,
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -647,36 +663,14 @@
         "code": NodegroupIssueCodeType,
         "message": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
-_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAddonsRequestListAddonsPaginateTypeDef(
-    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
-    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAddonsRequestRequestTypeDef = TypedDict(
     "_RequiredListAddonsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestRequestTypeDef = TypedDict(
@@ -691,73 +685,24 @@
 
 class ListAddonsRequestRequestTypeDef(
     _RequiredListAddonsRequestRequestTypeDef, _OptionalListAddonsRequestRequestTypeDef
 ):
     pass
 
 
-ListAddonsResponseTypeDef = TypedDict(
-    "ListAddonsResponseTypeDef",
-    {
-        "addons": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "include": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "include": Sequence[str],
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusters": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
-    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFargateProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListFargateProfilesRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListFargateProfilesRequestRequestTypeDef = TypedDict(
@@ -773,45 +718,14 @@
 class ListFargateProfilesRequestRequestTypeDef(
     _RequiredListFargateProfilesRequestRequestTypeDef,
     _OptionalListFargateProfilesRequestRequestTypeDef,
 ):
     pass
 
 
-ListFargateProfilesResponseTypeDef = TypedDict(
-    "ListFargateProfilesResponseTypeDef",
-    {
-        "fargateProfileNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
-    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProviderConfigsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
@@ -827,36 +741,14 @@
 class ListIdentityProviderConfigsRequestRequestTypeDef(
     _RequiredListIdentityProviderConfigsRequestRequestTypeDef,
     _OptionalListIdentityProviderConfigsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
-    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListNodegroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListNodegroupsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListNodegroupsRequestRequestTypeDef = TypedDict(
@@ -871,62 +763,21 @@
 
 class ListNodegroupsRequestRequestTypeDef(
     _RequiredListNodegroupsRequestRequestTypeDef, _OptionalListNodegroupsRequestRequestTypeDef
 ):
     pass
 
 
-ListNodegroupsResponseTypeDef = TypedDict(
-    "ListNodegroupsResponseTypeDef",
-    {
-        "nodegroups": List[str],
-        "nextToken": str,
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
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "nodegroupName": str,
-        "addonName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUpdatesRequestListUpdatesPaginateTypeDef(
-    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
-    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUpdatesRequestRequestTypeDef = TypedDict(
     "_RequiredListUpdatesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListUpdatesRequestRequestTypeDef = TypedDict(
@@ -943,53 +794,41 @@
 
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
 
-ListUpdatesResponseTypeDef = TypedDict(
-    "ListUpdatesResponseTypeDef",
+LogSetupOutputTypeDef = TypedDict(
+    "LogSetupOutputTypeDef",
     {
-        "updateIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "types": List[LogTypeType],
+        "enabled": bool,
     },
+    total=False,
 )
 
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RemoteAccessConfigOutputTypeDef = TypedDict(
+    "RemoteAccessConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ec2SshKey": str,
+        "sourceSecurityGroups": List[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1084,14 +923,77 @@
         "architecture": List[str],
         "compatibilities": List[CompatibilityTypeDef],
         "requiresConfiguration": bool,
     },
     total=False,
 )
 
+DescribeAddonConfigurationResponseTypeDef = TypedDict(
+    "DescribeAddonConfigurationResponseTypeDef",
+    {
+        "addonName": str,
+        "addonVersion": str,
+        "configurationSchema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAddonsResponseTypeDef = TypedDict(
+    "ListAddonsResponseTypeDef",
+    {
+        "addons": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusters": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFargateProfilesResponseTypeDef = TypedDict(
+    "ListFargateProfilesResponseTypeDef",
+    {
+        "fargateProfileNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNodegroupsResponseTypeDef = TypedDict(
+    "ListNodegroupsResponseTypeDef",
+    {
+        "nodegroups": List[str],
+        "nextToken": str,
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
+ListUpdatesResponseTypeDef = TypedDict(
+    "ListUpdatesResponseTypeDef",
+    {
+        "updateIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "oidc": OidcIdentityProviderConfigRequestTypeDef,
     },
 )
@@ -1192,57 +1094,14 @@
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
 
-_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFargateProfileRequestRequestTypeDef",
-    {
-        "fargateProfileName": str,
-        "clusterName": str,
-        "podExecutionRoleArn": str,
-    },
-)
-_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFargateProfileRequestRequestTypeDef",
-    {
-        "subnets": Sequence[str],
-        "selectors": Sequence[FargateProfileSelectorTypeDef],
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateFargateProfileRequestRequestTypeDef(
-    _RequiredCreateFargateProfileRequestRequestTypeDef,
-    _OptionalCreateFargateProfileRequestRequestTypeDef,
-):
-    pass
-
-
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1490,14 +1349,148 @@
 class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
 ):
     pass
 
 
+DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    {
+        "kubernetesVersion": str,
+        "addonName": str,
+        "types": Sequence[str],
+        "publishers": Sequence[str],
+        "owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAddonsRequestListAddonsPaginateTypeDef(
+    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
+    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
+):
+    pass
+
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "include": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
+    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
+    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
+    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "nodegroupName": str,
+        "addonName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUpdatesRequestListUpdatesPaginateTypeDef(
+    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
+    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
+):
+    pass
+
+
 DescribeIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "identityProviderConfig": IdentityProviderConfigTypeDef,
     },
 )
@@ -1526,27 +1519,55 @@
 
 
 ListIdentityProviderConfigsResponseTypeDef = TypedDict(
     "ListIdentityProviderConfigsResponseTypeDef",
     {
         "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "resources": List[str],
+        "provider": ProviderTypeDef,
+    },
+    total=False,
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorUnionTypeDef = Union[
+    FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef
+]
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1563,22 +1584,31 @@
     "NodegroupHealthTypeDef",
     {
         "issues": List[IssueTypeDef],
     },
     total=False,
 )
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "clusterLogging": List[LogSetupOutputTypeDef],
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
 
+RemoteAccessConfigUnionTypeDef = Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef]
 UpdateTypeDef = TypedDict(
     "UpdateTypeDef",
     {
         "id": str,
         "status": UpdateStatusType,
         "type": UpdateTypeType,
         "params": List[UpdateParamTypeDef],
@@ -1618,38 +1648,14 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1669,42 +1675,71 @@
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+EncryptionConfigUnionTypeDef = Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
     {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+    {
+        "fargateProfileName": str,
         "clusterName": str,
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "podExecutionRoleArn": str,
     },
 )
-_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFargateProfileRequestRequestTypeDef",
     {
+        "subnets": Sequence[str],
+        "selectors": Sequence[FargateProfileSelectorUnionTypeDef],
         "clientRequestToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class AssociateEncryptionConfigRequestRequestTypeDef(
-    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
-    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+class CreateFargateProfileRequestRequestTypeDef(
+    _RequiredCreateFargateProfileRequestRequestTypeDef,
+    _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodegroupTypeDef = TypedDict(
     "NodegroupTypeDef",
     {
         "nodegroupName": str,
@@ -1715,15 +1750,15 @@
         "createdAt": datetime,
         "modifiedAt": datetime,
         "status": NodegroupStatusType,
         "capacityType": CapacityTypesType,
         "scalingConfig": NodegroupScalingConfigTypeDef,
         "instanceTypes": List[str],
         "subnets": List[str],
-        "remoteAccess": RemoteAccessConfigTypeDef,
+        "remoteAccess": RemoteAccessConfigOutputTypeDef,
         "amiType": AMITypesType,
         "nodeRole": str,
         "labels": Dict[str, str],
         "taints": List[TaintTypeDef],
         "resources": NodegroupResourcesTypeDef,
         "diskSize": int,
         "health": NodegroupHealthTypeDef,
@@ -1741,59 +1776,31 @@
         "arn": str,
         "createdAt": datetime,
         "version": str,
         "endpoint": str,
         "roleArn": str,
         "resourcesVpcConfig": VpcConfigResponseTypeDef,
         "kubernetesNetworkConfig": KubernetesNetworkConfigResponseTypeDef,
-        "logging": LoggingTypeDef,
+        "logging": LoggingOutputTypeDef,
         "identity": IdentityTypeDef,
         "status": ClusterStatusType,
         "certificateAuthority": CertificateTypeDef,
         "clientRequestToken": str,
         "platformVersion": str,
         "tags": Dict[str, str],
-        "encryptionConfig": List[EncryptionConfigTypeDef],
+        "encryptionConfig": List[EncryptionConfigOutputTypeDef],
         "connectorConfig": ConnectorConfigResponseTypeDef,
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "resourcesVpcConfig": VpcConfigRequestTypeDef,
-    },
-)
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
-    {
-        "version": str,
-        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
-        "logging": LoggingTypeDef,
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
-        "outpostConfig": OutpostConfigRequestTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
-):
-    pass
-
-
+LoggingUnionTypeDef = Union[LoggingTypeDef, LoggingOutputTypeDef]
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1814,172 +1821,224 @@
     pass
 
 
 AssociateEncryptionConfigResponseTypeDef = TypedDict(
     "AssociateEncryptionConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "AssociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateResponseTypeDef = TypedDict(
     "DescribeUpdateResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "DisassociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAddonResponseTypeDef = TypedDict(
     "UpdateAddonResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterConfigResponseTypeDef = TypedDict(
     "UpdateClusterConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterVersionResponseTypeDef = TypedDict(
     "UpdateClusterVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupConfigResponseTypeDef = TypedDict(
     "UpdateNodegroupConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupVersionResponseTypeDef = TypedDict(
     "UpdateNodegroupVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAddonResponseTypeDef = TypedDict(
     "CreateAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAddonResponseTypeDef = TypedDict(
     "DeleteAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonResponseTypeDef = TypedDict(
     "DescribeAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonVersionsResponseTypeDef = TypedDict(
     "DescribeAddonVersionsResponseTypeDef",
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clusterName": str,
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
     },
 )
+_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class AssociateEncryptionConfigRequestRequestTypeDef(
+    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
+    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "resourcesVpcConfig": VpcConfigRequestTypeDef,
+    },
+)
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
+    {
+        "version": str,
+        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
+        "logging": LoggingTypeDef,
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+        "outpostConfig": OutpostConfigRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
+    pass
+
 
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNodegroupResponseTypeDef = TypedDict(
     "DeleteNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNodegroupResponseTypeDef = TypedDict(
     "DescribeNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterClusterResponseTypeDef = TypedDict(
     "DeregisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterClusterResponseTypeDef = TypedDict(
     "RegisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/type_defs.pyi` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_eks.type_defs import AddonIssueTypeDef
 
-    data: AddonIssueTypeDef = {...}
+    data: AddonIssueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AddonIssueCodeType,
     AddonStatusType,
     AMITypesType,
     CapacityTypesType,
     ClusterIssueCodeType,
@@ -42,137 +42,146 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddonIssueTypeDef",
     "MarketplaceInformationTypeDef",
     "CompatibilityTypeDef",
+    "ResponseMetadataTypeDef",
     "OidcIdentityProviderConfigRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "CertificateTypeDef",
     "ClusterIssueTypeDef",
     "ConnectorConfigResponseTypeDef",
     "KubernetesNetworkConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
-    "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteFargateProfileRequestRequestTypeDef",
     "DeleteNodegroupRequestRequestTypeDef",
     "DeregisterClusterRequestRequestTypeDef",
     "DescribeAddonConfigurationRequestRequestTypeDef",
-    "DescribeAddonConfigurationResponseTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAddonRequestRequestTypeDef",
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAddonVersionsRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
+    "FargateProfileSelectorOutputTypeDef",
+    "FargateProfileSelectorTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
-    "ListAddonsRequestListAddonsPaginateTypeDef",
     "ListAddonsRequestRequestTypeDef",
-    "ListAddonsResponseTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListClustersResponseTypeDef",
-    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
-    "ListFargateProfilesResponseTypeDef",
-    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
-    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
-    "ListNodegroupsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "ListUpdatesRequestRequestTypeDef",
-    "ListUpdatesResponseTypeDef",
+    "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "RemoteAccessConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
     "AddonVersionInfoTypeDef",
+    "DescribeAddonConfigurationResponseTypeDef",
+    "ListAddonsResponseTypeDef",
+    "ListClustersResponseTypeDef",
+    "ListFargateProfilesResponseTypeDef",
+    "ListNodegroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
-    "CreateFargateProfileRequestRequestTypeDef",
-    "FargateProfileTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef",
     "DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef",
     "DescribeNodegroupRequestNodegroupActiveWaitTypeDef",
     "DescribeNodegroupRequestNodegroupDeletedWaitTypeDef",
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    "ListAddonsRequestListAddonsPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
+    "FargateProfileTypeDef",
+    "FargateProfileSelectorUnionTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
+    "LoggingOutputTypeDef",
     "LoggingTypeDef",
+    "RemoteAccessConfigUnionTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "EncryptionConfigUnionTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateFargateProfileRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
-    "CreateClusterRequestRequestTypeDef",
+    "LoggingUnionTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
     "DescribeUpdateResponseTypeDef",
     "DisassociateIdentityProviderConfigResponseTypeDef",
     "UpdateAddonResponseTypeDef",
     "UpdateClusterConfigResponseTypeDef",
     "UpdateClusterVersionResponseTypeDef",
     "UpdateNodegroupConfigResponseTypeDef",
     "UpdateNodegroupVersionResponseTypeDef",
     "CreateAddonResponseTypeDef",
     "DeleteAddonResponseTypeDef",
     "DescribeAddonResponseTypeDef",
     "DescribeAddonVersionsResponseTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
+    "CreateClusterRequestRequestTypeDef",
     "CreateNodegroupResponseTypeDef",
     "DeleteNodegroupResponseTypeDef",
     "DescribeNodegroupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeregisterClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -204,14 +213,25 @@
         "clusterVersion": str,
         "platformVersions": List[str],
         "defaultVersion": bool,
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
 _RequiredOidcIdentityProviderConfigRequestTypeDef = TypedDict(
     "_RequiredOidcIdentityProviderConfigRequestTypeDef",
     {
         "identityProviderConfigName": str,
         "issuerUrl": str,
         "clientId": str,
     },
@@ -362,23 +382,14 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
-FargateProfileSelectorTypeDef = TypedDict(
-    "FargateProfileSelectorTypeDef",
-    {
-        "namespace": str,
-        "labels": Mapping[str, str],
-    },
-    total=False,
-)
-
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "name": str,
         "version": str,
         "id": str,
     },
@@ -477,24 +488,14 @@
     "DescribeAddonConfigurationRequestRequestTypeDef",
     {
         "addonName": str,
         "addonVersion": str,
     },
 )
 
-DescribeAddonConfigurationResponseTypeDef = TypedDict(
-    "DescribeAddonConfigurationResponseTypeDef",
-    {
-        "addonName": str,
-        "addonVersion": str,
-        "configurationSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -504,23 +505,20 @@
     "DescribeAddonRequestRequestTypeDef",
     {
         "clusterName": str,
         "addonName": str,
     },
 )
 
-DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
-    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "kubernetesVersion": str,
-        "addonName": str,
-        "types": Sequence[str],
-        "publishers": Sequence[str],
-        "owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeAddonVersionsRequestRequestTypeDef = TypedDict(
     "DescribeAddonVersionsRequestRequestTypeDef",
     {
@@ -601,14 +599,32 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
+FargateProfileSelectorOutputTypeDef = TypedDict(
+    "FargateProfileSelectorOutputTypeDef",
+    {
+        "namespace": str,
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorTypeDef = TypedDict(
+    "FargateProfileSelectorTypeDef",
+    {
+        "namespace": str,
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -638,34 +654,14 @@
         "code": NodegroupIssueCodeType,
         "message": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
-_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
-    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAddonsRequestListAddonsPaginateTypeDef(
-    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
-    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAddonsRequestRequestTypeDef = TypedDict(
     "_RequiredListAddonsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListAddonsRequestRequestTypeDef = TypedDict(
@@ -678,71 +674,24 @@
 )
 
 class ListAddonsRequestRequestTypeDef(
     _RequiredListAddonsRequestRequestTypeDef, _OptionalListAddonsRequestRequestTypeDef
 ):
     pass
 
-ListAddonsResponseTypeDef = TypedDict(
-    "ListAddonsResponseTypeDef",
-    {
-        "addons": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "include": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "include": Sequence[str],
     },
     total=False,
 )
 
-ListClustersResponseTypeDef = TypedDict(
-    "ListClustersResponseTypeDef",
-    {
-        "clusters": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
-    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
-    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFargateProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListFargateProfilesRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListFargateProfilesRequestRequestTypeDef = TypedDict(
@@ -756,43 +705,14 @@
 
 class ListFargateProfilesRequestRequestTypeDef(
     _RequiredListFargateProfilesRequestRequestTypeDef,
     _OptionalListFargateProfilesRequestRequestTypeDef,
 ):
     pass
 
-ListFargateProfilesResponseTypeDef = TypedDict(
-    "ListFargateProfilesResponseTypeDef",
-    {
-        "fargateProfileNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
-    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
-):
-    pass
-
 _RequiredListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProviderConfigsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListIdentityProviderConfigsRequestRequestTypeDef = TypedDict(
@@ -806,34 +726,14 @@
 
 class ListIdentityProviderConfigsRequestRequestTypeDef(
     _RequiredListIdentityProviderConfigsRequestRequestTypeDef,
     _OptionalListIdentityProviderConfigsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "clusterName": str,
-    },
-)
-_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
-    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
-    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
-    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListNodegroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListNodegroupsRequestRequestTypeDef",
     {
         "clusterName": str,
     },
 )
 _OptionalListNodegroupsRequestRequestTypeDef = TypedDict(
@@ -846,60 +746,21 @@
 )
 
 class ListNodegroupsRequestRequestTypeDef(
     _RequiredListNodegroupsRequestRequestTypeDef, _OptionalListNodegroupsRequestRequestTypeDef
 ):
     pass
 
-ListNodegroupsResponseTypeDef = TypedDict(
-    "ListNodegroupsResponseTypeDef",
-    {
-        "nodegroups": List[str],
-        "nextToken": str,
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
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
-    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
-    {
-        "nodegroupName": str,
-        "addonName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUpdatesRequestListUpdatesPaginateTypeDef(
-    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
-    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListUpdatesRequestRequestTypeDef = TypedDict(
     "_RequiredListUpdatesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListUpdatesRequestRequestTypeDef = TypedDict(
@@ -914,53 +775,41 @@
 )
 
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
-ListUpdatesResponseTypeDef = TypedDict(
-    "ListUpdatesResponseTypeDef",
+LogSetupOutputTypeDef = TypedDict(
+    "LogSetupOutputTypeDef",
     {
-        "updateIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "types": List[LogTypeType],
+        "enabled": bool,
     },
+    total=False,
 )
 
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RemoteAccessConfigOutputTypeDef = TypedDict(
+    "RemoteAccessConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ec2SshKey": str,
+        "sourceSecurityGroups": List[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1051,14 +900,77 @@
         "architecture": List[str],
         "compatibilities": List[CompatibilityTypeDef],
         "requiresConfiguration": bool,
     },
     total=False,
 )
 
+DescribeAddonConfigurationResponseTypeDef = TypedDict(
+    "DescribeAddonConfigurationResponseTypeDef",
+    {
+        "addonName": str,
+        "addonVersion": str,
+        "configurationSchema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAddonsResponseTypeDef = TypedDict(
+    "ListAddonsResponseTypeDef",
+    {
+        "addons": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClustersResponseTypeDef = TypedDict(
+    "ListClustersResponseTypeDef",
+    {
+        "clusters": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFargateProfilesResponseTypeDef = TypedDict(
+    "ListFargateProfilesResponseTypeDef",
+    {
+        "fargateProfileNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNodegroupsResponseTypeDef = TypedDict(
+    "ListNodegroupsResponseTypeDef",
+    {
+        "nodegroups": List[str],
+        "nextToken": str,
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
+ListUpdatesResponseTypeDef = TypedDict(
+    "ListUpdatesResponseTypeDef",
+    {
+        "updateIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAssociateIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "oidc": OidcIdentityProviderConfigRequestTypeDef,
     },
 )
@@ -1151,55 +1063,14 @@
 )
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
-_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFargateProfileRequestRequestTypeDef",
-    {
-        "fargateProfileName": str,
-        "clusterName": str,
-        "podExecutionRoleArn": str,
-    },
-)
-_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFargateProfileRequestRequestTypeDef",
-    {
-        "subnets": Sequence[str],
-        "selectors": Sequence[FargateProfileSelectorTypeDef],
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateFargateProfileRequestRequestTypeDef(
-    _RequiredCreateFargateProfileRequestRequestTypeDef,
-    _OptionalCreateFargateProfileRequestRequestTypeDef,
-):
-    pass
-
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1427,14 +1298,138 @@
 
 class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(
     _RequiredDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
     _OptionalDescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
 ):
     pass
 
+DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef = TypedDict(
+    "DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef",
+    {
+        "kubernetesVersion": str,
+        "addonName": str,
+        "types": Sequence[str],
+        "publishers": Sequence[str],
+        "owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_RequiredListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListAddonsRequestListAddonsPaginateTypeDef = TypedDict(
+    "_OptionalListAddonsRequestListAddonsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAddonsRequestListAddonsPaginateTypeDef(
+    _RequiredListAddonsRequestListAddonsPaginateTypeDef,
+    _OptionalListAddonsRequestListAddonsPaginateTypeDef,
+):
+    pass
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "include": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef = TypedDict(
+    "_OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(
+    _RequiredListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    _OptionalListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+):
+    pass
+
+_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(
+    _RequiredListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    _OptionalListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+):
+    pass
+
+_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "clusterName": str,
+    },
+)
+_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef = TypedDict(
+    "_OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListNodegroupsRequestListNodegroupsPaginateTypeDef(
+    _RequiredListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    _OptionalListNodegroupsRequestListNodegroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_RequiredListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListUpdatesRequestListUpdatesPaginateTypeDef = TypedDict(
+    "_OptionalListUpdatesRequestListUpdatesPaginateTypeDef",
+    {
+        "nodegroupName": str,
+        "addonName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUpdatesRequestListUpdatesPaginateTypeDef(
+    _RequiredListUpdatesRequestListUpdatesPaginateTypeDef,
+    _OptionalListUpdatesRequestListUpdatesPaginateTypeDef,
+):
+    pass
+
 DescribeIdentityProviderConfigRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "identityProviderConfig": IdentityProviderConfigTypeDef,
     },
 )
@@ -1461,27 +1456,55 @@
     pass
 
 ListIdentityProviderConfigsResponseTypeDef = TypedDict(
     "ListIdentityProviderConfigsResponseTypeDef",
     {
         "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EncryptionConfigOutputTypeDef = TypedDict(
+    "EncryptionConfigOutputTypeDef",
+    {
+        "resources": List[str],
+        "provider": ProviderTypeDef,
+    },
+    total=False,
+)
+
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorOutputTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+FargateProfileSelectorUnionTypeDef = Union[
+    FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef
+]
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1498,22 +1521,31 @@
     "NodegroupHealthTypeDef",
     {
         "issues": List[IssueTypeDef],
     },
     total=False,
 )
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "clusterLogging": List[LogSetupOutputTypeDef],
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
 
+RemoteAccessConfigUnionTypeDef = Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef]
 UpdateTypeDef = TypedDict(
     "UpdateTypeDef",
     {
         "id": str,
         "status": UpdateStatusType,
         "type": UpdateTypeType,
         "params": List[UpdateParamTypeDef],
@@ -1553,38 +1585,14 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1602,40 +1610,69 @@
 
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+EncryptionConfigUnionTypeDef = Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFargateProfileRequestRequestTypeDef",
     {
+        "fargateProfileName": str,
         "clusterName": str,
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "podExecutionRoleArn": str,
     },
 )
-_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFargateProfileRequestRequestTypeDef",
     {
+        "subnets": Sequence[str],
+        "selectors": Sequence[FargateProfileSelectorUnionTypeDef],
         "clientRequestToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class AssociateEncryptionConfigRequestRequestTypeDef(
-    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
-    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+class CreateFargateProfileRequestRequestTypeDef(
+    _RequiredCreateFargateProfileRequestRequestTypeDef,
+    _OptionalCreateFargateProfileRequestRequestTypeDef,
 ):
     pass
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodegroupTypeDef = TypedDict(
     "NodegroupTypeDef",
     {
         "nodegroupName": str,
@@ -1646,15 +1683,15 @@
         "createdAt": datetime,
         "modifiedAt": datetime,
         "status": NodegroupStatusType,
         "capacityType": CapacityTypesType,
         "scalingConfig": NodegroupScalingConfigTypeDef,
         "instanceTypes": List[str],
         "subnets": List[str],
-        "remoteAccess": RemoteAccessConfigTypeDef,
+        "remoteAccess": RemoteAccessConfigOutputTypeDef,
         "amiType": AMITypesType,
         "nodeRole": str,
         "labels": Dict[str, str],
         "taints": List[TaintTypeDef],
         "resources": NodegroupResourcesTypeDef,
         "diskSize": int,
         "health": NodegroupHealthTypeDef,
@@ -1672,57 +1709,31 @@
         "arn": str,
         "createdAt": datetime,
         "version": str,
         "endpoint": str,
         "roleArn": str,
         "resourcesVpcConfig": VpcConfigResponseTypeDef,
         "kubernetesNetworkConfig": KubernetesNetworkConfigResponseTypeDef,
-        "logging": LoggingTypeDef,
+        "logging": LoggingOutputTypeDef,
         "identity": IdentityTypeDef,
         "status": ClusterStatusType,
         "certificateAuthority": CertificateTypeDef,
         "clientRequestToken": str,
         "platformVersion": str,
         "tags": Dict[str, str],
-        "encryptionConfig": List[EncryptionConfigTypeDef],
+        "encryptionConfig": List[EncryptionConfigOutputTypeDef],
         "connectorConfig": ConnectorConfigResponseTypeDef,
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "resourcesVpcConfig": VpcConfigRequestTypeDef,
-    },
-)
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
-    {
-        "version": str,
-        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
-        "logging": LoggingTypeDef,
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
-        "outpostConfig": OutpostConfigRequestTypeDef,
-    },
-    total=False,
-)
-
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
-):
-    pass
-
+LoggingUnionTypeDef = Union[LoggingTypeDef, LoggingOutputTypeDef]
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1741,172 +1752,220 @@
 ):
     pass
 
 AssociateEncryptionConfigResponseTypeDef = TypedDict(
     "AssociateEncryptionConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "AssociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateResponseTypeDef = TypedDict(
     "DescribeUpdateResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateIdentityProviderConfigResponseTypeDef = TypedDict(
     "DisassociateIdentityProviderConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAddonResponseTypeDef = TypedDict(
     "UpdateAddonResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterConfigResponseTypeDef = TypedDict(
     "UpdateClusterConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterVersionResponseTypeDef = TypedDict(
     "UpdateClusterVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupConfigResponseTypeDef = TypedDict(
     "UpdateNodegroupConfigResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNodegroupVersionResponseTypeDef = TypedDict(
     "UpdateNodegroupVersionResponseTypeDef",
     {
         "update": UpdateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAddonResponseTypeDef = TypedDict(
     "CreateAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAddonResponseTypeDef = TypedDict(
     "DeleteAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonResponseTypeDef = TypedDict(
     "DescribeAddonResponseTypeDef",
     {
         "addon": AddonTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddonVersionsResponseTypeDef = TypedDict(
     "DescribeAddonVersionsResponseTypeDef",
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clusterName": str,
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+    },
+)
+_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+class AssociateEncryptionConfigRequestRequestTypeDef(
+    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
+    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "resourcesVpcConfig": VpcConfigRequestTypeDef,
+    },
+)
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
+    {
+        "version": str,
+        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
+        "logging": LoggingTypeDef,
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
+        "outpostConfig": OutpostConfigRequestTypeDef,
     },
+    total=False,
 )
 
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
+    pass
+
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNodegroupResponseTypeDef = TypedDict(
     "DeleteNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNodegroupResponseTypeDef = TypedDict(
     "DescribeNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterClusterResponseTypeDef = TypedDict(
     "DeregisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterClusterResponseTypeDef = TypedDict(
     "RegisterClusterResponseTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/waiter.py` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks/waiter.pyi` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/PKG-INFO` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-eks
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore eks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore eks type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-eks"></a>
 
 # types-aiobotocore-eks
 
 [![PyPI - types-aiobotocore-eks](https://img.shields.io/pypi/v/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-eks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-eks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-eks?color=blue)](https://pypistats.org/packages/types-aiobotocore-eks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-eks)](https://pepy.tech/project/types-aiobotocore-eks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EKS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
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
 [types-aiobotocore-eks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/).
 
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
@@ -400,161 +399,170 @@
 )
 
 
 def check_value(value: AMITypesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_eks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_eks.type_defs import (
     AddonIssueTypeDef,
     MarketplaceInformationTypeDef,
     CompatibilityTypeDef,
+    ResponseMetadataTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     AutoScalingGroupTypeDef,
     CertificateTypeDef,
     ClusterIssueTypeDef,
     ConnectorConfigResponseTypeDef,
     KubernetesNetworkConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     ConnectorConfigRequestTypeDef,
     ControlPlanePlacementRequestTypeDef,
     ControlPlanePlacementResponseTypeDef,
     CreateAddonRequestRequestTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     VpcConfigRequestTypeDef,
-    FargateProfileSelectorTypeDef,
     LaunchTemplateSpecificationTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     RemoteAccessConfigTypeDef,
     TaintTypeDef,
     DeleteAddonRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteFargateProfileRequestRequestTypeDef,
     DeleteNodegroupRequestRequestTypeDef,
     DeregisterClusterRequestRequestTypeDef,
     DescribeAddonConfigurationRequestRequestTypeDef,
-    DescribeAddonConfigurationResponseTypeDef,
     WaiterConfigTypeDef,
     DescribeAddonRequestRequestTypeDef,
-    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddonVersionsRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeFargateProfileRequestRequestTypeDef,
     IdentityProviderConfigTypeDef,
     DescribeNodegroupRequestRequestTypeDef,
     DescribeUpdateRequestRequestTypeDef,
     ProviderTypeDef,
     ErrorDetailTypeDef,
+    FargateProfileSelectorOutputTypeDef,
+    FargateProfileSelectorTypeDef,
     OidcIdentityProviderConfigTypeDef,
     OIDCTypeDef,
     IssueTypeDef,
-    ListAddonsRequestListAddonsPaginateTypeDef,
     ListAddonsRequestRequestTypeDef,
-    ListAddonsResponseTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListClustersResponseTypeDef,
-    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
     ListFargateProfilesRequestRequestTypeDef,
-    ListFargateProfilesResponseTypeDef,
-    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
     ListIdentityProviderConfigsRequestRequestTypeDef,
-    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
     ListNodegroupsRequestRequestTypeDef,
-    ListNodegroupsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUpdatesRequestListUpdatesPaginateTypeDef,
     ListUpdatesRequestRequestTypeDef,
-    ListUpdatesResponseTypeDef,
+    LogSetupOutputTypeDef,
     LogSetupTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RemoteAccessConfigOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddonRequestRequestTypeDef,
     UpdateClusterVersionRequestRequestTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateParamTypeDef,
     AddonHealthTypeDef,
     AddonVersionInfoTypeDef,
+    DescribeAddonConfigurationResponseTypeDef,
+    ListAddonsResponseTypeDef,
+    ListClustersResponseTypeDef,
+    ListFargateProfilesResponseTypeDef,
+    ListNodegroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUpdatesResponseTypeDef,
     AssociateIdentityProviderConfigRequestRequestTypeDef,
     NodegroupResourcesTypeDef,
     ClusterHealthTypeDef,
     RegisterClusterRequestRequestTypeDef,
     OutpostConfigRequestTypeDef,
     OutpostConfigResponseTypeDef,
-    CreateFargateProfileRequestRequestTypeDef,
-    FargateProfileTypeDef,
     UpdateNodegroupVersionRequestRequestTypeDef,
     CreateNodegroupRequestRequestTypeDef,
     UpdateTaintsPayloadTypeDef,
     DescribeAddonRequestAddonActiveWaitTypeDef,
     DescribeAddonRequestAddonDeletedWaitTypeDef,
     DescribeClusterRequestClusterActiveWaitTypeDef,
     DescribeClusterRequestClusterDeletedWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef,
     DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef,
     DescribeNodegroupRequestNodegroupActiveWaitTypeDef,
     DescribeNodegroupRequestNodegroupDeletedWaitTypeDef,
+    DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef,
+    ListAddonsRequestListAddonsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListFargateProfilesRequestListFargateProfilesPaginateTypeDef,
+    ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef,
+    ListNodegroupsRequestListNodegroupsPaginateTypeDef,
+    ListUpdatesRequestListUpdatesPaginateTypeDef,
     DescribeIdentityProviderConfigRequestRequestTypeDef,
     DisassociateIdentityProviderConfigRequestRequestTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
+    FargateProfileTypeDef,
+    FargateProfileSelectorUnionTypeDef,
     IdentityProviderConfigResponseTypeDef,
     IdentityTypeDef,
     NodegroupHealthTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
+    RemoteAccessConfigUnionTypeDef,
     UpdateTypeDef,
     AddonTypeDef,
     AddonInfoTypeDef,
+    UpdateNodegroupConfigRequestRequestTypeDef,
+    EncryptionConfigUnionTypeDef,
     CreateFargateProfileResponseTypeDef,
     DeleteFargateProfileResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
-    UpdateNodegroupConfigRequestRequestTypeDef,
-    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateFargateProfileRequestRequestTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     NodegroupTypeDef,
     ClusterTypeDef,
-    CreateClusterRequestRequestTypeDef,
+    LoggingUnionTypeDef,
     UpdateClusterConfigRequestRequestTypeDef,
     AssociateEncryptionConfigResponseTypeDef,
     AssociateIdentityProviderConfigResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
     CreateAddonResponseTypeDef,
     DeleteAddonResponseTypeDef,
     DescribeAddonResponseTypeDef,
     DescribeAddonVersionsResponseTypeDef,
+    AssociateEncryptionConfigRequestRequestTypeDef,
+    CreateClusterRequestRequestTypeDef,
     CreateNodegroupResponseTypeDef,
     DeleteNodegroupResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeregisterClusterResponseTypeDef,
     DescribeClusterResponseTypeDef,
     RegisterClusterResponseTypeDef,
 )
 
 
-def get_structure() -> AddonIssueTypeDef:
+def get_value() -> AddonIssueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-eks-2.5.2/types_aiobotocore_eks.egg-info/SOURCES.txt` & `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


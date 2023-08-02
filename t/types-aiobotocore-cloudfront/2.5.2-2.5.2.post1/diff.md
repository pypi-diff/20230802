# Comparing `tmp/types-aiobotocore-cloudfront-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudfront-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudfront-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudfront-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
```

## Comparing `types-aiobotocore-cloudfront-2.5.2.tar` & `types-aiobotocore-cloudfront-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31189 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29612 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83274 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83152 2023-07-08 01:27:03.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   138536 2023-07-08 01:27:07.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   138273 2023-07-08 01:27:05.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:02.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-08 01:27:04.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.477824 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31189 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:21.000000 types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    34119 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32589 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.029637 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83226 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83104 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174495 2023-08-02 14:34:39.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174134 2023-08-02 14:34:36.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:33.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-02 14:34:34.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.033637 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34119 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:51:59.000000 types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/LICENSE` & `types-aiobotocore-cloudfront-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/PKG-INFO` & `types-aiobotocore-cloudfront-2.5.2.post1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudfront
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudfront type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudfront"></a>
 
 # types-aiobotocore-cloudfront
 
 [![PyPI - types-aiobotocore-cloudfront](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudfront?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudfront)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [types-aiobotocore-cloudfront docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/).
 
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
@@ -395,46 +394,57 @@
 )
 
 
 def check_value(value: CachePolicyCookieBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudfront.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
+    AliasesOutputTypeDef,
     AliasesTypeDef,
+    CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    BlobTypeDef,
+    TrustedKeyGroupsOutputTypeDef,
+    TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
+    CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
     ContentTypeProfileTypeDef,
+    StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
     CustomErrorResponseTypeDef,
     OriginCustomHeaderTypeDef,
+    OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
     DeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     DeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
@@ -447,20 +457,22 @@
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
-    EmptyResponseMetadataTypeDef,
+    FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
     KinesisStreamConfigTypeDef,
+    QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
     FunctionAssociationTypeDef,
     FunctionMetadataTypeDef,
+    GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigRequestRequestTypeDef,
     GetContinuousDeploymentPolicyRequestRequestTypeDef,
@@ -468,271 +480,332 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
-    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
+    KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
+    PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
+    StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
     OriginGroupMemberTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
-    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
     QueryArgProfileTypeDef,
+    ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
+    ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
+    ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
+    ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
-    ResponseMetadataTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
-    TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    TestFunctionRequestRequestTypeDef,
+    CachePolicyCookiesConfigOutputTypeDef,
+    CookiePreferenceOutputTypeDef,
+    OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
+    CachePolicyHeadersConfigOutputTypeDef,
+    OriginRequestPolicyHeadersConfigOutputTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
+    CachePolicyQueryStringsConfigOutputTypeDef,
+    OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
+    ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
-    GetKeyGroupConfigResultTypeDef,
-    KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
     GetOriginAccessControlConfigResultTypeDef,
     OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
     GetPublicKeyConfigResultTypeDef,
     PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
+    CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
+    CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
+    CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
+    EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
     EndPointTypeDef,
+    FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
+    RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
+    GetKeyGroupConfigResultTypeDef,
+    KeyGroupConfigUnionTypeDef,
+    KeyGroupTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
+    LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
+    OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
+    OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
+    QueryArgProfilesOutputTypeDef,
     QueryArgProfilesTypeDef,
+    ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
+    ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
+    ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
+    ForwardedValuesOutputTypeDef,
     ForwardedValuesTypeDef,
+    ParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     ParametersInCacheKeyAndForwardedToOriginTypeDef,
     OriginRequestPolicyConfigTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
+    ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
     TrafficConfigTypeDef,
-    CreateKeyGroupResultTypeDef,
-    GetKeyGroupResultTypeDef,
-    KeyGroupSummaryTypeDef,
-    UpdateKeyGroupResultTypeDef,
     CreateOriginAccessControlResultTypeDef,
     GetOriginAccessControlResultTypeDef,
     UpdateOriginAccessControlResultTypeDef,
     CreatePublicKeyResultTypeDef,
     GetPublicKeyResultTypeDef,
     UpdatePublicKeyResultTypeDef,
+    OriginOutputTypeDef,
     OriginTypeDef,
+    EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
     CreateRealtimeLogConfigRequestRequestTypeDef,
     RealtimeLogConfigTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
-    CreateInvalidationRequestRequestTypeDef,
+    CreateKeyGroupResultTypeDef,
+    GetKeyGroupResultTypeDef,
+    KeyGroupSummaryTypeDef,
+    UpdateKeyGroupResultTypeDef,
     InvalidationTypeDef,
+    CreateInvalidationRequestRequestTypeDef,
+    InvalidationBatchUnionTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
     CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
     ListOriginAccessControlsResultTypeDef,
+    OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
+    QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
-    CreateStreamingDistributionRequestRequestTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
+    CreateStreamingDistributionRequestRequestTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsUnionTypeDef,
+    CacheBehaviorOutputTypeDef,
+    DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
-    CachePolicyConfigTypeDef,
-    CreateOriginRequestPolicyRequestRequestTypeDef,
+    CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
+    CachePolicyConfigTypeDef,
+    CreateOriginRequestPolicyRequestRequestTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
-    KeyGroupListTypeDef,
+    OriginsOutputTypeDef,
     OriginsTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     RealtimeLogConfigsTypeDef,
     UpdateRealtimeLogConfigResultTypeDef,
     ListFunctionsResultTypeDef,
     TestFunctionResultTypeDef,
+    KeyGroupListTypeDef,
     CreateInvalidationResultTypeDef,
     GetInvalidationResultTypeDef,
     StreamingDistributionTypeDef,
+    OriginGroupsOutputTypeDef,
     OriginGroupsTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
-    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
+    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
+    CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
-    CreateCachePolicyRequestRequestTypeDef,
     GetCachePolicyConfigResultTypeDef,
-    UpdateCachePolicyRequestRequestTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CachePolicyConfigUnionTypeDef,
+    CreateCachePolicyRequestRequestTypeDef,
+    UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
-    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
-    ListKeyGroupsResultTypeDef,
-    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
-    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
+    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
+    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
+    ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
-    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
-    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionListTypeDef,
+    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
+    DistributionConfigTypeDef,
     CachePolicySummaryTypeDef,
     CreateCachePolicyResultTypeDef,
     GetCachePolicyResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     OriginRequestPolicyListTypeDef,
     ContinuousDeploymentPolicySummaryTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
@@ -743,40 +816,41 @@
     UpdateFieldLevelEncryptionProfileResultTypeDef,
     ListFieldLevelEncryptionProfilesResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
     GetFieldLevelEncryptionResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
-    CreateDistributionRequestRequestTypeDef,
-    DistributionConfigWithTagsTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
-    UpdateDistributionRequestRequestTypeDef,
     DistributionListTypeDef,
+    CreateDistributionRequestRequestTypeDef,
+    DistributionConfigUnionTypeDef,
+    DistributionConfigWithTagsTypeDef,
+    UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
-    CreateDistributionWithTagsRequestRequestTypeDef,
     CopyDistributionResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     GetDistributionResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     ListDistributionsByRealtimeLogConfigResultTypeDef,
     ListDistributionsByWebACLIdResultTypeDef,
     ListDistributionsResultTypeDef,
+    CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
-def get_structure() -> AliasICPRecordalTypeDef:
+def get_value() -> AliasICPRecordalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/README.md` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-cloudfront
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore cloudfront type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudfront"></a>
 
 # types-aiobotocore-cloudfront
 
 [![PyPI - types-aiobotocore-cloudfront](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudfront?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudfront)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [types-aiobotocore-cloudfront docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/).
 
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
@@ -362,46 +394,57 @@
 )
 
 
 def check_value(value: CachePolicyCookieBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudfront.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
+    AliasesOutputTypeDef,
     AliasesTypeDef,
+    CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    BlobTypeDef,
+    TrustedKeyGroupsOutputTypeDef,
+    TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
+    CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
     ContentTypeProfileTypeDef,
+    StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
     CustomErrorResponseTypeDef,
     OriginCustomHeaderTypeDef,
+    OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
     DeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     DeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
@@ -414,20 +457,22 @@
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
-    EmptyResponseMetadataTypeDef,
+    FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
     KinesisStreamConfigTypeDef,
+    QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
     FunctionAssociationTypeDef,
     FunctionMetadataTypeDef,
+    GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigRequestRequestTypeDef,
     GetContinuousDeploymentPolicyRequestRequestTypeDef,
@@ -435,271 +480,332 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
-    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
+    KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
+    PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
+    StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
     OriginGroupMemberTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
-    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
     QueryArgProfileTypeDef,
+    ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
+    ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
+    ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
+    ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
-    ResponseMetadataTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
-    TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    TestFunctionRequestRequestTypeDef,
+    CachePolicyCookiesConfigOutputTypeDef,
+    CookiePreferenceOutputTypeDef,
+    OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
+    CachePolicyHeadersConfigOutputTypeDef,
+    OriginRequestPolicyHeadersConfigOutputTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
+    CachePolicyQueryStringsConfigOutputTypeDef,
+    OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
+    ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
-    GetKeyGroupConfigResultTypeDef,
-    KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
     GetOriginAccessControlConfigResultTypeDef,
     OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
     GetPublicKeyConfigResultTypeDef,
     PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
+    CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
+    CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
+    CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
+    EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
     EndPointTypeDef,
+    FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
+    RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
+    GetKeyGroupConfigResultTypeDef,
+    KeyGroupConfigUnionTypeDef,
+    KeyGroupTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
+    LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
+    OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
+    OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
+    QueryArgProfilesOutputTypeDef,
     QueryArgProfilesTypeDef,
+    ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
+    ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
+    ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
+    ForwardedValuesOutputTypeDef,
     ForwardedValuesTypeDef,
+    ParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     ParametersInCacheKeyAndForwardedToOriginTypeDef,
     OriginRequestPolicyConfigTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
+    ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
     TrafficConfigTypeDef,
-    CreateKeyGroupResultTypeDef,
-    GetKeyGroupResultTypeDef,
-    KeyGroupSummaryTypeDef,
-    UpdateKeyGroupResultTypeDef,
     CreateOriginAccessControlResultTypeDef,
     GetOriginAccessControlResultTypeDef,
     UpdateOriginAccessControlResultTypeDef,
     CreatePublicKeyResultTypeDef,
     GetPublicKeyResultTypeDef,
     UpdatePublicKeyResultTypeDef,
+    OriginOutputTypeDef,
     OriginTypeDef,
+    EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
     CreateRealtimeLogConfigRequestRequestTypeDef,
     RealtimeLogConfigTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
-    CreateInvalidationRequestRequestTypeDef,
+    CreateKeyGroupResultTypeDef,
+    GetKeyGroupResultTypeDef,
+    KeyGroupSummaryTypeDef,
+    UpdateKeyGroupResultTypeDef,
     InvalidationTypeDef,
+    CreateInvalidationRequestRequestTypeDef,
+    InvalidationBatchUnionTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
     CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
     ListOriginAccessControlsResultTypeDef,
+    OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
+    QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
-    CreateStreamingDistributionRequestRequestTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
+    CreateStreamingDistributionRequestRequestTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsUnionTypeDef,
+    CacheBehaviorOutputTypeDef,
+    DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
-    CachePolicyConfigTypeDef,
-    CreateOriginRequestPolicyRequestRequestTypeDef,
+    CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
+    CachePolicyConfigTypeDef,
+    CreateOriginRequestPolicyRequestRequestTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
-    KeyGroupListTypeDef,
+    OriginsOutputTypeDef,
     OriginsTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     RealtimeLogConfigsTypeDef,
     UpdateRealtimeLogConfigResultTypeDef,
     ListFunctionsResultTypeDef,
     TestFunctionResultTypeDef,
+    KeyGroupListTypeDef,
     CreateInvalidationResultTypeDef,
     GetInvalidationResultTypeDef,
     StreamingDistributionTypeDef,
+    OriginGroupsOutputTypeDef,
     OriginGroupsTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
-    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
+    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
+    CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
-    CreateCachePolicyRequestRequestTypeDef,
     GetCachePolicyConfigResultTypeDef,
-    UpdateCachePolicyRequestRequestTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CachePolicyConfigUnionTypeDef,
+    CreateCachePolicyRequestRequestTypeDef,
+    UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
-    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
-    ListKeyGroupsResultTypeDef,
-    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
-    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
+    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
+    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
+    ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
-    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
-    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionListTypeDef,
+    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
+    DistributionConfigTypeDef,
     CachePolicySummaryTypeDef,
     CreateCachePolicyResultTypeDef,
     GetCachePolicyResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     OriginRequestPolicyListTypeDef,
     ContinuousDeploymentPolicySummaryTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
@@ -710,40 +816,41 @@
     UpdateFieldLevelEncryptionProfileResultTypeDef,
     ListFieldLevelEncryptionProfilesResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
     GetFieldLevelEncryptionResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
-    CreateDistributionRequestRequestTypeDef,
-    DistributionConfigWithTagsTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
-    UpdateDistributionRequestRequestTypeDef,
     DistributionListTypeDef,
+    CreateDistributionRequestRequestTypeDef,
+    DistributionConfigUnionTypeDef,
+    DistributionConfigWithTagsTypeDef,
+    UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
-    CreateDistributionWithTagsRequestRequestTypeDef,
     CopyDistributionResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     GetDistributionResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     ListDistributionsByRealtimeLogConfigResultTypeDef,
     ListDistributionsByWebACLIdResultTypeDef,
     ListDistributionsResultTypeDef,
+    CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
-def get_structure() -> AliasICPRecordalTypeDef:
+def get_value() -> AliasICPRecordalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/setup.py` & `types-aiobotocore-cloudfront-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudfront",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudFront 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudfront type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudfront type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudfront": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/"
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__init__.pyi` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/__main__.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFront 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudFront 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("cloudfront") as client:
         client: CloudFrontClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     CachePolicyTypeType,
     FunctionStageType,
     OriginRequestPolicyTypeType,
     ResponseHeadersPolicyTypeType,
@@ -30,17 +29,18 @@
 from .paginator import (
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
-    CachePolicyConfigTypeDef,
+    BlobTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -53,20 +53,20 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
@@ -88,16 +88,16 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
-    InvalidationBatchTypeDef,
-    KeyGroupConfigTypeDef,
+    InvalidationBatchUnionTypeDef,
+    KeyGroupConfigUnionTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -115,22 +115,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigTypeDef,
-    StreamingDistributionConfigTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsTypeDef,
+    TagsUnionTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -372,15 +372,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
         """
 
     async def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cache_policy)
         """
@@ -392,26 +392,26 @@
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
 
     async def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_continuous_deployment_policy)
         """
 
     async def create_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution)
         """
@@ -423,59 +423,55 @@
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution_with_tags)
         """
 
     async def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_config)
         """
 
     async def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_profile)
         """
 
     async def create_function(
-        self,
-        *,
-        Name: str,
-        FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, Name: str, FunctionConfig: FunctionConfigTypeDef, FunctionCode: BlobTypeDef
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_function)
         """
 
     async def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_invalidation)
         """
 
     async def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_key_group)
@@ -498,15 +494,15 @@
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_access_control)
         """
 
     async def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_request_policy)
         """
@@ -537,25 +533,25 @@
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_realtime_log_config)
         """
 
     async def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_response_headers_policy)
         """
 
     async def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_streaming_distribution)
         """
@@ -1255,30 +1251,25 @@
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#publish_function)
         """
 
     async def tag_resource(
-        self, *, Resource: str, Tags: TagsTypeDef
+        self, *, Resource: str, Tags: TagsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#tag_resource)
         """
 
     async def test_function(
-        self,
-        *,
-        Name: str,
-        IfMatch: str,
-        EventObject: Union[str, bytes, IO[Any], StreamingBody],
-        Stage: FunctionStageType = ...
+        self, *, Name: str, IfMatch: str, EventObject: BlobTypeDef, Stage: FunctionStageType = ...
     ) -> TestFunctionResultTypeDef:
         """
         Tests a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#test_function)
         """
@@ -1290,15 +1281,15 @@
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#untag_resource)
         """
 
     async def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cache_policy)
         """
@@ -1316,27 +1307,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     async def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_continuous_deployment_policy)
         """
 
     async def update_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution)
         """
@@ -1351,29 +1342,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution_with_staging_config)
         """
 
     async def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_config)
         """
 
     async def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1382,25 +1373,25 @@
 
     async def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        FunctionCode: BlobTypeDef
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_function)
         """
 
     async def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_key_group)
         """
@@ -1418,15 +1409,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_access_control)
         """
 
     async def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1458,29 +1449,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_realtime_log_config)
         """
 
     async def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_response_headers_policy)
         """
 
     async def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
+        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/client.pyi` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("cloudfront") as client:
         client: CloudFrontClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     CachePolicyTypeType,
     FunctionStageType,
     OriginRequestPolicyTypeType,
     ResponseHeadersPolicyTypeType,
@@ -30,17 +29,18 @@
 from .paginator import (
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
-    CachePolicyConfigTypeDef,
+    BlobTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -53,20 +53,20 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
@@ -88,16 +88,16 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
-    InvalidationBatchTypeDef,
-    KeyGroupConfigTypeDef,
+    InvalidationBatchUnionTypeDef,
+    KeyGroupConfigUnionTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -115,22 +115,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigTypeDef,
-    StreamingDistributionConfigTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsTypeDef,
+    TagsUnionTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -363,15 +363,15 @@
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#copy_distribution)
         """
     async def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cache_policy)
         """
@@ -381,25 +381,25 @@
         """
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
     async def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_continuous_deployment_policy)
         """
     async def create_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution)
         """
@@ -409,55 +409,51 @@
         """
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_distribution_with_tags)
         """
     async def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_config)
         """
     async def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_field_level_encryption_profile)
         """
     async def create_function(
-        self,
-        *,
-        Name: str,
-        FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, Name: str, FunctionConfig: FunctionConfigTypeDef, FunctionCode: BlobTypeDef
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_function)
         """
     async def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_invalidation)
         """
     async def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_key_group)
@@ -477,15 +473,15 @@
         """
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_access_control)
         """
     async def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_origin_request_policy)
         """
@@ -513,24 +509,24 @@
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_realtime_log_config)
         """
     async def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_response_headers_policy)
         """
     async def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#create_streaming_distribution)
         """
@@ -1159,29 +1155,24 @@
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#publish_function)
         """
     async def tag_resource(
-        self, *, Resource: str, Tags: TagsTypeDef
+        self, *, Resource: str, Tags: TagsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#tag_resource)
         """
     async def test_function(
-        self,
-        *,
-        Name: str,
-        IfMatch: str,
-        EventObject: Union[str, bytes, IO[Any], StreamingBody],
-        Stage: FunctionStageType = ...
+        self, *, Name: str, IfMatch: str, EventObject: BlobTypeDef, Stage: FunctionStageType = ...
     ) -> TestFunctionResultTypeDef:
         """
         Tests a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#test_function)
         """
@@ -1191,15 +1182,15 @@
         """
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#untag_resource)
         """
     async def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cache_policy)
         """
@@ -1215,26 +1206,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
     async def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_continuous_deployment_policy)
         """
     async def update_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution)
         """
@@ -1247,28 +1238,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_distribution_with_staging_config)
         """
     async def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_field_level_encryption_config)
         """
     async def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1276,24 +1267,24 @@
         """
     async def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        FunctionCode: BlobTypeDef
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_function)
         """
     async def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_key_group)
         """
@@ -1309,15 +1300,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_origin_access_control)
         """
     async def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1346,28 +1337,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_realtime_log_config)
         """
     async def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/client/#update_response_headers_policy)
         """
     async def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
+        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/literals.pyi` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,76 +42,70 @@
 __all__ = (
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
     "ListInvalidationsPaginator",
     "ListStreamingDistributionsPaginator",
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
 class ListCloudFrontOriginAccessIdentitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
-
 class ListDistributionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listdistributionspaginator)
         """
 
-
 class ListInvalidationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
-        self, *, DistributionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listinvalidationspaginator)
         """
 
-
 class ListStreamingDistributionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#liststreamingdistributionspaginator)
         """
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/paginator.pyi` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,70 +42,76 @@
 __all__ = (
     "ListCloudFrontOriginAccessIdentitiesPaginator",
     "ListDistributionsPaginator",
     "ListInvalidationsPaginator",
     "ListStreamingDistributionsPaginator",
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
 class ListCloudFrontOriginAccessIdentitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCloudFrontOriginAccessIdentitiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListCloudFrontOriginAccessIdentities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listcloudfrontoriginaccessidentitiespaginator)
         """
 
+
 class ListDistributionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListDistributions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listdistributionspaginator)
         """
 
+
 class ListInvalidationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listinvalidationspaginator)
     """
 
     def paginate(
-        self, *, DistributionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DistributionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvalidationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListInvalidations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#listinvalidationspaginator)
         """
 
+
 class ListStreamingDistributionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#liststreamingdistributionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamingDistributionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Paginator.ListStreamingDistributions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/paginators/#liststreamingdistributionspaginator)
         """
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudfront.type_defs import AliasICPRecordalTypeDef
 
-    data: AliasICPRecordalTypeDef = {...}
+    data: AliasICPRecordalTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -55,39 +55,49 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasICPRecordalTypeDef",
+    "AliasesOutputTypeDef",
     "AliasesTypeDef",
+    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
+    "BlobTypeDef",
+    "TrustedKeyGroupsOutputTypeDef",
+    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
+    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
+    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
+    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
+    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -100,20 +110,22 @@
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
+    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
+    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -121,271 +133,332 @@
     "WaiterConfigTypeDef",
     "GetDistributionRequestRequestTypeDef",
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
-    "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
+    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
+    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
     "ListDistributionsByKeyGroupRequestRequestTypeDef",
     "ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef",
     "ListDistributionsByWebACLIdRequestRequestTypeDef",
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListDistributionsRequestRequestTypeDef",
     "ListFieldLevelEncryptionConfigsRequestRequestTypeDef",
     "ListFieldLevelEncryptionProfilesRequestRequestTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListInvalidationsRequestRequestTypeDef",
     "ListKeyGroupsRequestRequestTypeDef",
     "ListOriginAccessControlsRequestRequestTypeDef",
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
+    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
+    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
-    "ResponseMetadataTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
-    "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
+    "TestFunctionRequestRequestTypeDef",
+    "CachePolicyCookiesConfigOutputTypeDef",
+    "CookiePreferenceOutputTypeDef",
+    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
+    "CachePolicyHeadersConfigOutputTypeDef",
+    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
+    "CachePolicyQueryStringsConfigOutputTypeDef",
+    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
+    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
     "GetOriginAccessControlConfigResultTypeDef",
     "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
     "GetPublicKeyConfigResultTypeDef",
     "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
+    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
+    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
+    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
+    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
     "EndPointTypeDef",
+    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
+    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupConfigUnionTypeDef",
+    "KeyGroupTypeDef",
+    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
+    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
+    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
+    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
+    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
+    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
+    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
+    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
+    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "TagsOutputTypeDef",
     "TagsTypeDef",
+    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
+    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
+    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
     "TrafficConfigTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
     "CreateOriginAccessControlResultTypeDef",
     "GetOriginAccessControlResultTypeDef",
     "UpdateOriginAccessControlResultTypeDef",
     "CreatePublicKeyResultTypeDef",
     "GetPublicKeyResultTypeDef",
     "UpdatePublicKeyResultTypeDef",
+    "OriginOutputTypeDef",
     "OriginTypeDef",
+    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
-    "CreateInvalidationRequestRequestTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
     "InvalidationTypeDef",
+    "CreateInvalidationRequestRequestTypeDef",
+    "InvalidationBatchUnionTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
+    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
+    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
+    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "CreateStreamingDistributionRequestRequestTypeDef",
     "GetStreamingDistributionConfigResultTypeDef",
+    "CreateStreamingDistributionRequestRequestTypeDef",
+    "StreamingDistributionConfigUnionTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagsUnionTypeDef",
+    "CacheBehaviorOutputTypeDef",
+    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigTypeDef",
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "CachePolicyConfigOutputTypeDef",
     "GetOriginRequestPolicyConfigResultTypeDef",
     "OriginRequestPolicyTypeDef",
+    "CachePolicyConfigTypeDef",
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "OriginRequestPolicyConfigUnionTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
+    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "KeyGroupListTypeDef",
+    "OriginsOutputTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileConfigOutputTypeDef",
     "FieldLevelEncryptionProfileSummaryTypeDef",
+    "FieldLevelEncryptionProfileConfigTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
+    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
+    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionConfigOutputTypeDef",
     "FieldLevelEncryptionSummaryTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
+    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
+    "CachePolicyConfigUnionTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
+    "ContinuousDeploymentPolicyConfigUnionTypeDef",
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
-    "ListKeyGroupsResultTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileListTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileConfigUnionTypeDef",
+    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
+    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionListTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigUnionTypeDef",
+    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigTypeDef",
+    "DistributionConfigOutputTypeDef",
     "DistributionSummaryTypeDef",
+    "DistributionConfigTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -396,159 +469,271 @@
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigWithTagsTypeDef",
     "DistributionTypeDef",
     "GetDistributionConfigResultTypeDef",
-    "UpdateDistributionRequestRequestTypeDef",
     "DistributionListTypeDef",
+    "CreateDistributionRequestRequestTypeDef",
+    "DistributionConfigUnionTypeDef",
+    "DistributionConfigWithTagsTypeDef",
+    "UpdateDistributionRequestRequestTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": str,
         "ICPRecordalStatus": ICPRecordalStatusType,
     },
     total=False,
 )
 
+_RequiredAliasesOutputTypeDef = TypedDict(
+    "_RequiredAliasesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalAliasesOutputTypeDef = TypedDict(
+    "_OptionalAliasesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class AliasesOutputTypeDef(_RequiredAliasesOutputTypeDef, _OptionalAliasesOutputTypeDef):
+    pass
+
 _RequiredAliasesTypeDef = TypedDict(
     "_RequiredAliasesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalAliasesTypeDef = TypedDict(
     "_OptionalAliasesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class AliasesTypeDef(_RequiredAliasesTypeDef, _OptionalAliasesTypeDef):
     pass
 
+CachedMethodsOutputTypeDef = TypedDict(
+    "CachedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
 
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": List[MethodType],
+        "Items": Sequence[MethodType],
     },
 )
 
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_RequiredTrustedKeyGroupsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_OptionalTrustedKeyGroupsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class TrustedKeyGroupsOutputTypeDef(
+    _RequiredTrustedKeyGroupsOutputTypeDef, _OptionalTrustedKeyGroupsOutputTypeDef
+):
+    pass
+
+_RequiredTrustedSignersOutputTypeDef = TypedDict(
+    "_RequiredTrustedSignersOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedSignersOutputTypeDef = TypedDict(
+    "_OptionalTrustedSignersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class TrustedSignersOutputTypeDef(
+    _RequiredTrustedSignersOutputTypeDef, _OptionalTrustedSignersOutputTypeDef
+):
+    pass
+
 _RequiredTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedKeyGroupsTypeDef = TypedDict(
     "_OptionalTrustedKeyGroupsTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class TrustedKeyGroupsTypeDef(_RequiredTrustedKeyGroupsTypeDef, _OptionalTrustedKeyGroupsTypeDef):
     pass
 
-
 _RequiredTrustedSignersTypeDef = TypedDict(
     "_RequiredTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedSignersTypeDef = TypedDict(
     "_OptionalTrustedSignersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
     pass
 
+_RequiredCookieNamesOutputTypeDef = TypedDict(
+    "_RequiredCookieNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCookieNamesOutputTypeDef = TypedDict(
+    "_OptionalCookieNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class CookieNamesOutputTypeDef(
+    _RequiredCookieNamesOutputTypeDef, _OptionalCookieNamesOutputTypeDef
+):
+    pass
 
 _RequiredCookieNamesTypeDef = TypedDict(
     "_RequiredCookieNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCookieNamesTypeDef = TypedDict(
     "_OptionalCookieNamesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
     pass
 
+_RequiredHeadersOutputTypeDef = TypedDict(
+    "_RequiredHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalHeadersOutputTypeDef = TypedDict(
+    "_OptionalHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class HeadersOutputTypeDef(_RequiredHeadersOutputTypeDef, _OptionalHeadersOutputTypeDef):
+    pass
 
 _RequiredHeadersTypeDef = TypedDict(
     "_RequiredHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalHeadersTypeDef = TypedDict(
     "_OptionalHeadersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
     pass
 
+_RequiredQueryStringNamesOutputTypeDef = TypedDict(
+    "_RequiredQueryStringNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringNamesOutputTypeDef = TypedDict(
+    "_OptionalQueryStringNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class QueryStringNamesOutputTypeDef(
+    _RequiredQueryStringNamesOutputTypeDef, _OptionalQueryStringNamesOutputTypeDef
+):
+    pass
 
 _RequiredQueryStringNamesTypeDef = TypedDict(
     "_RequiredQueryStringNamesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -556,19 +741,17 @@
     "_OptionalQueryStringNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
-
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -603,20 +786,38 @@
     "_OptionalContentTypeProfileTypeDef",
     {
         "ProfileId": str,
     },
     total=False,
 )
 
-
 class ContentTypeProfileTypeDef(
     _RequiredContentTypeProfileTypeDef, _OptionalContentTypeProfileTypeDef
 ):
     pass
 
+_RequiredStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_RequiredStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_OptionalStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class StagingDistributionDnsNamesOutputTypeDef(
+    _RequiredStagingDistributionDnsNamesOutputTypeDef,
+    _OptionalStagingDistributionDnsNamesOutputTypeDef,
+):
+    pass
 
 _RequiredStagingDistributionDnsNamesTypeDef = TypedDict(
     "_RequiredStagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -624,21 +825,19 @@
     "_OptionalStagingDistributionDnsNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
-
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
@@ -663,20 +862,29 @@
     {
         "Staging": bool,
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
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
 
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
         "Runtime": Literal["cloudfront-js-1.0"],
     },
@@ -693,19 +901,17 @@
     "_OptionalKeyGroupConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class KeyGroupConfigTypeDef(_RequiredKeyGroupConfigTypeDef, _OptionalKeyGroupConfigTypeDef):
     pass
 
-
 _RequiredOriginAccessControlConfigTypeDef = TypedDict(
     "_RequiredOriginAccessControlConfigTypeDef",
     {
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
@@ -715,21 +921,19 @@
     "_OptionalOriginAccessControlConfigTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class OriginAccessControlConfigTypeDef(
     _RequiredOriginAccessControlConfigTypeDef, _OptionalOriginAccessControlConfigTypeDef
 ):
     pass
 
-
 _RequiredPublicKeyConfigTypeDef = TypedDict(
     "_RequiredPublicKeyConfigTypeDef",
     {
         "CallerReference": str,
         "Name": str,
         "EncodedKey": str,
     },
@@ -738,19 +942,17 @@
     "_OptionalPublicKeyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
-
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -759,34 +961,40 @@
         "ResponsePagePath": str,
         "ResponseCode": str,
         "ErrorCachingMinTTL": int,
     },
     total=False,
 )
 
-
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
-
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+OriginSslProtocolsOutputTypeDef = TypedDict(
+    "OriginSslProtocolsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[SslProtocolType],
+    },
+)
+
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": List[SslProtocolType],
+        "Items": Sequence[SslProtocolType],
     },
 )
 
 _RequiredDeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
@@ -796,131 +1004,119 @@
     "_OptionalDeleteCachePolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteCachePolicyRequestRequestTypeDef(
     _RequiredDeleteCachePolicyRequestRequestTypeDef, _OptionalDeleteCachePolicyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteDistributionRequestRequestTypeDef(
     _RequiredDeleteDistributionRequestRequestTypeDef,
     _OptionalDeleteDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteFieldLevelEncryptionConfigRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteFunctionRequestRequestTypeDef = TypedDict(
     "DeleteFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -935,21 +1131,19 @@
     "_OptionalDeleteKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteKeyGroupRequestRequestTypeDef(
     _RequiredDeleteKeyGroupRequestRequestTypeDef, _OptionalDeleteKeyGroupRequestRequestTypeDef
 ):
     pass
 
-
 DeleteMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 
@@ -963,65 +1157,59 @@
     "_OptionalDeleteOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteOriginAccessControlRequestRequestTypeDef(
     _RequiredDeleteOriginAccessControlRequestRequestTypeDef,
     _OptionalDeleteOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteOriginRequestPolicyRequestRequestTypeDef(
     _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef,
     _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeletePublicKeyRequestRequestTypeDef(
     _RequiredDeletePublicKeyRequestRequestTypeDef, _OptionalDeletePublicKeyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "ARN": str,
     },
     total=False,
@@ -1037,65 +1225,59 @@
     "_OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredDeleteResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class DeleteStreamingDistributionRequestRequestTypeDef(
     _RequiredDeleteStreamingDistributionRequestRequestTypeDef,
     _OptionalDeleteStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFunctionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1130,27 +1312,37 @@
     {
         "NextMarker": str,
         "Items": List[str],
     },
     total=False,
 )
 
-
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_RequiredFieldPatternsOutputTypeDef = TypedDict(
+    "_RequiredFieldPatternsOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Quantity": int,
     },
 )
+_OptionalFieldPatternsOutputTypeDef = TypedDict(
+    "_OptionalFieldPatternsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class FieldPatternsOutputTypeDef(
+    _RequiredFieldPatternsOutputTypeDef, _OptionalFieldPatternsOutputTypeDef
+):
+    pass
 
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -1158,48 +1350,63 @@
     "_OptionalFieldPatternsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
-
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
 
+_RequiredQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_RequiredQueryStringCacheKeysOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_OptionalQueryStringCacheKeysOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class QueryStringCacheKeysOutputTypeDef(
+    _RequiredQueryStringCacheKeysOutputTypeDef, _OptionalQueryStringCacheKeysOutputTypeDef
+):
+    pass
+
 _RequiredQueryStringCacheKeysTypeDef = TypedDict(
     "_RequiredQueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringCacheKeysTypeDef = TypedDict(
     "_OptionalQueryStringCacheKeysTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
-
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1216,39 +1423,55 @@
     {
         "Stage": FunctionStageType,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-
 class FunctionMetadataTypeDef(_RequiredFunctionMetadataTypeDef, _OptionalFunctionMetadataTypeDef):
     pass
 
+_RequiredGeoRestrictionOutputTypeDef = TypedDict(
+    "_RequiredGeoRestrictionOutputTypeDef",
+    {
+        "RestrictionType": GeoRestrictionTypeType,
+        "Quantity": int,
+    },
+)
+_OptionalGeoRestrictionOutputTypeDef = TypedDict(
+    "_OptionalGeoRestrictionOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class GeoRestrictionOutputTypeDef(
+    _RequiredGeoRestrictionOutputTypeDef, _OptionalGeoRestrictionOutputTypeDef
+):
+    pass
 
 _RequiredGeoRestrictionTypeDef = TypedDict(
     "_RequiredGeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
     },
 )
 _OptionalGeoRestrictionTypeDef = TypedDict(
     "_OptionalGeoRestrictionTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class GeoRestrictionTypeDef(_RequiredGeoRestrictionTypeDef, _OptionalGeoRestrictionTypeDef):
     pass
 
-
 GetCachePolicyConfigRequestRequestTypeDef = TypedDict(
     "GetCachePolicyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1348,31 +1571,19 @@
     "_OptionalGetFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
-
-GetFunctionResultTypeDef = TypedDict(
-    "GetFunctionResultTypeDef",
-    {
-        "FunctionCode": StreamingBody,
-        "ETag": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -1380,14 +1591,34 @@
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredKeyGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredKeyGroupConfigOutputTypeDef",
+    {
+        "Name": str,
+        "Items": List[str],
+    },
+)
+_OptionalKeyGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalKeyGroupConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class KeyGroupConfigOutputTypeDef(
+    _RequiredKeyGroupConfigOutputTypeDef, _OptionalKeyGroupConfigOutputTypeDef
+):
+    pass
+
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1473,33 +1704,48 @@
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredPathsOutputTypeDef = TypedDict(
+    "_RequiredPathsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalPathsOutputTypeDef = TypedDict(
+    "_OptionalPathsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class PathsOutputTypeDef(_RequiredPathsOutputTypeDef, _OptionalPathsOutputTypeDef):
+    pass
+
 _RequiredPathsTypeDef = TypedDict(
     "_RequiredPathsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalPathsTypeDef = TypedDict(
     "_OptionalPathsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class PathsTypeDef(_RequiredPathsTypeDef, _OptionalPathsTypeDef):
     pass
 
-
 InvalidationSummaryTypeDef = TypedDict(
     "InvalidationSummaryTypeDef",
     {
         "Id": str,
         "CreateTime": datetime,
         "Status": str,
     },
@@ -1515,19 +1761,17 @@
     "_OptionalKeyPairIdsTypeDef",
     {
         "Items": List[str],
     },
     total=False,
 )
 
-
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
-
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1535,35 +1779,35 @@
     "_OptionalLambdaFunctionAssociationTypeDef",
     {
         "IncludeBody": bool,
     },
     total=False,
 )
 
-
 class LambdaFunctionAssociationTypeDef(
     _RequiredLambdaFunctionAssociationTypeDef, _OptionalLambdaFunctionAssociationTypeDef
 ):
     pass
 
-
 ListCachePoliciesRequestRequestTypeDef = TypedDict(
     "ListCachePoliciesRequestRequestTypeDef",
     {
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
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
 
 ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     {
@@ -1585,22 +1829,20 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-
 class ListConflictingAliasesRequestRequestTypeDef(
     _RequiredListConflictingAliasesRequestRequestTypeDef,
     _OptionalListConflictingAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 ListContinuousDeploymentPoliciesRequestRequestTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1617,22 +1859,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByCachePolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByCachePolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByCachePolicyIdRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupId": str,
     },
 )
 _OptionalListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
@@ -1640,22 +1880,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByKeyGroupRequestRequestTypeDef(
     _RequiredListDistributionsByKeyGroupRequestRequestTypeDef,
     _OptionalListDistributionsByKeyGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     {
         "OriginRequestPolicyId": str,
     },
 )
 _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
@@ -1663,22 +1901,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
 ):
     pass
 
-
 ListDistributionsByRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "RealtimeLogConfigName": str,
         "RealtimeLogConfigArn": str,
@@ -1697,22 +1933,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByWebACLIdRequestRequestTypeDef",
     {
         "WebACLId": str,
     },
 )
 _OptionalListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
@@ -1720,30 +1954,20 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
-
-ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1773,36 +1997,14 @@
         "Marker": str,
         "MaxItems": str,
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "DistributionId": str,
-    },
-)
-_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
-    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInvalidationsRequestRequestTypeDef = TypedDict(
     "_RequiredListInvalidationsRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 _OptionalListInvalidationsRequestRequestTypeDef = TypedDict(
@@ -1810,21 +2012,19 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-
 class ListInvalidationsRequestRequestTypeDef(
     _RequiredListInvalidationsRequestRequestTypeDef, _OptionalListInvalidationsRequestRequestTypeDef
 ):
     pass
 
-
 ListKeyGroupsRequestRequestTypeDef = TypedDict(
     "ListKeyGroupsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1873,22 +2073,14 @@
         "Type": ResponseHeadersPolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamingDistributionsRequestRequestTypeDef = TypedDict(
     "ListStreamingDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1916,19 +2108,27 @@
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
 
+StatusCodesOutputTypeDef = TypedDict(
+    "StatusCodesOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[int],
+    },
+)
+
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": List[int],
+        "Items": Sequence[int],
     },
 )
 
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
@@ -1945,36 +2145,24 @@
     "_OptionalOriginShieldTypeDef",
     {
         "OriginShieldRegion": str,
     },
     total=False,
 )
 
-
 class OriginShieldTypeDef(_RequiredOriginShieldTypeDef, _OptionalOriginShieldTypeDef):
     pass
 
-
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
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
 _RequiredPublicKeySummaryTypeDef = TypedDict(
     "_RequiredPublicKeySummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatedTime": datetime,
         "EncodedKey": str,
@@ -1984,19 +2172,17 @@
     "_OptionalPublicKeySummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class PublicKeySummaryTypeDef(_RequiredPublicKeySummaryTypeDef, _OptionalPublicKeySummaryTypeDef):
     pass
 
-
 PublishFunctionRequestRequestTypeDef = TypedDict(
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -2005,82 +2191,122 @@
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef(
+    _RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+    _OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
-
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "SamplingRate": float,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
-
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
@@ -2136,22 +2362,20 @@
     {
         "IncludeSubdomains": bool,
         "Preload": bool,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyStrictTransportSecurityTypeDef(
     _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef,
     _OptionalResponseHeadersPolicyStrictTransportSecurityTypeDef,
 ):
     pass
 
-
 _RequiredResponseHeadersPolicyXSSProtectionTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyXSSProtectionTypeDef",
     {
         "Override": bool,
         "Protection": bool,
     },
 )
@@ -2160,33 +2384,20 @@
     {
         "ModeBlock": bool,
         "ReportUri": str,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
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
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
@@ -2218,84 +2429,154 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    {
+        "StagingDistributionId": str,
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
+    _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
+):
+    pass
+
+_RequiredAllowedMethodsOutputTypeDef = TypedDict(
+    "_RequiredAllowedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+_OptionalAllowedMethodsOutputTypeDef = TypedDict(
+    "_OptionalAllowedMethodsOutputTypeDef",
+    {
+        "CachedMethods": CachedMethodsOutputTypeDef,
+    },
+    total=False,
+)
+
+class AllowedMethodsOutputTypeDef(
+    _RequiredAllowedMethodsOutputTypeDef, _OptionalAllowedMethodsOutputTypeDef
+):
+    pass
+
+_RequiredAllowedMethodsTypeDef = TypedDict(
+    "_RequiredAllowedMethodsTypeDef",
+    {
+        "Quantity": int,
+        "Items": Sequence[MethodType],
+    },
+)
+_OptionalAllowedMethodsTypeDef = TypedDict(
+    "_OptionalAllowedMethodsTypeDef",
+    {
+        "CachedMethods": CachedMethodsTypeDef,
+    },
+    total=False,
+)
+
+class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
+    pass
 
 _RequiredTestFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredTestFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
-        "EventObject": Union[str, bytes, IO[Any], StreamingBody],
+        "EventObject": BlobTypeDef,
     },
 )
 _OptionalTestFunctionRequestRequestTypeDef = TypedDict(
     "_OptionalTestFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-
 class TestFunctionRequestRequestTypeDef(
     _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+_RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyCookiesConfigOutputTypeDef",
     {
-        "Id": str,
+        "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
-_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+_OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyCookiesConfigOutputTypeDef",
     {
-        "StagingDistributionId": str,
-        "IfMatch": str,
+        "Cookies": CookieNamesOutputTypeDef,
     },
     total=False,
 )
 
-
-class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
-    _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
-    _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
+class CachePolicyCookiesConfigOutputTypeDef(
+    _RequiredCachePolicyCookiesConfigOutputTypeDef, _OptionalCachePolicyCookiesConfigOutputTypeDef
 ):
     pass
 
-
-_RequiredAllowedMethodsTypeDef = TypedDict(
-    "_RequiredAllowedMethodsTypeDef",
+_RequiredCookiePreferenceOutputTypeDef = TypedDict(
+    "_RequiredCookiePreferenceOutputTypeDef",
     {
-        "Quantity": int,
-        "Items": List[MethodType],
+        "Forward": ItemSelectionType,
     },
 )
-_OptionalAllowedMethodsTypeDef = TypedDict(
-    "_OptionalAllowedMethodsTypeDef",
+_OptionalCookiePreferenceOutputTypeDef = TypedDict(
+    "_OptionalCookiePreferenceOutputTypeDef",
     {
-        "CachedMethods": CachedMethodsTypeDef,
+        "WhitelistedNames": CookieNamesOutputTypeDef,
     },
     total=False,
 )
 
-
-class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
+class CookiePreferenceOutputTypeDef(
+    _RequiredCookiePreferenceOutputTypeDef, _OptionalCookiePreferenceOutputTypeDef
+):
     pass
 
+_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "Cookies": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyCookiesConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyCookiesConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyCookiesConfigOutputTypeDef,
+):
+    pass
 
 _RequiredCachePolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
@@ -2303,61 +2584,94 @@
     "_OptionalCachePolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
-
 class CachePolicyCookiesConfigTypeDef(
     _RequiredCachePolicyCookiesConfigTypeDef, _OptionalCachePolicyCookiesConfigTypeDef
 ):
     pass
 
-
 _RequiredCookiePreferenceTypeDef = TypedDict(
     "_RequiredCookiePreferenceTypeDef",
     {
         "Forward": ItemSelectionType,
     },
 )
 _OptionalCookiePreferenceTypeDef = TypedDict(
     "_OptionalCookiePreferenceTypeDef",
     {
         "WhitelistedNames": CookieNamesTypeDef,
     },
     total=False,
 )
 
-
 class CookiePreferenceTypeDef(_RequiredCookiePreferenceTypeDef, _OptionalCookiePreferenceTypeDef):
     pass
 
-
 _RequiredOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyCookiesConfigTypeDef(
     _RequiredOriginRequestPolicyCookiesConfigTypeDef,
     _OptionalOriginRequestPolicyCookiesConfigTypeDef,
 ):
     pass
 
+_RequiredCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": CachePolicyHeaderBehaviorType,
+    },
+)
+_OptionalCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyHeadersConfigOutputTypeDef(
+    _RequiredCachePolicyHeadersConfigOutputTypeDef, _OptionalCachePolicyHeadersConfigOutputTypeDef
+):
+    pass
+
+_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyHeadersConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyHeadersConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyHeadersConfigOutputTypeDef,
+):
+    pass
 
 _RequiredCachePolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredCachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
     },
 )
@@ -2365,42 +2679,78 @@
     "_OptionalCachePolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
-
 class CachePolicyHeadersConfigTypeDef(
     _RequiredCachePolicyHeadersConfigTypeDef, _OptionalCachePolicyHeadersConfigTypeDef
 ):
     pass
 
-
 _RequiredOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyHeadersConfigTypeDef(
     _RequiredOriginRequestPolicyHeadersConfigTypeDef,
     _OptionalOriginRequestPolicyHeadersConfigTypeDef,
 ):
     pass
 
+_RequiredCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
+    },
+)
+_OptionalCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyQueryStringsConfigOutputTypeDef(
+    _RequiredCachePolicyQueryStringsConfigOutputTypeDef,
+    _OptionalCachePolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
+_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyQueryStringsConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
 
 _RequiredCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
     },
 )
@@ -2408,43 +2758,39 @@
     "_OptionalCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
-
 class CachePolicyQueryStringsConfigTypeDef(
     _RequiredCachePolicyQueryStringsConfigTypeDef, _OptionalCachePolicyQueryStringsConfigTypeDef
 ):
     pass
 
-
 _RequiredOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyQueryStringsConfigTypeDef(
     _RequiredOriginRequestPolicyQueryStringsConfigTypeDef,
     _OptionalOriginRequestPolicyQueryStringsConfigTypeDef,
 ):
     pass
 
-
 _RequiredCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityTypeDef",
     {
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
@@ -2452,37 +2798,26 @@
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
     total=False,
 )
 
-
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
-
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
         "Id": str,
     },
 )
@@ -2490,22 +2825,20 @@
     "_OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCloudFrontOriginAccessIdentityListTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -2516,120 +2849,141 @@
     {
         "NextMarker": str,
         "Items": List[CloudFrontOriginAccessIdentitySummaryTypeDef],
     },
     total=False,
 )
 
-
 class CloudFrontOriginAccessIdentityListTypeDef(
     _RequiredCloudFrontOriginAccessIdentityListTypeDef,
     _OptionalCloudFrontOriginAccessIdentityListTypeDef,
 ):
     pass
 
-
 ConflictingAliasesListTypeDef = TypedDict(
     "ConflictingAliasesListTypeDef",
     {
         "NextMarker": str,
         "MaxItems": int,
         "Quantity": int,
         "Items": List[ConflictingAliasTypeDef],
     },
     total=False,
 )
 
+_RequiredContentTypeProfilesOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalContentTypeProfilesOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfilesOutputTypeDef",
+    {
+        "Items": List[ContentTypeProfileTypeDef],
+    },
+    total=False,
+)
+
+class ContentTypeProfilesOutputTypeDef(
+    _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
+):
+    pass
+
 _RequiredContentTypeProfilesTypeDef = TypedDict(
     "_RequiredContentTypeProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesTypeDef = TypedDict(
     "_OptionalContentTypeProfilesTypeDef",
     {
         "Items": Sequence[ContentTypeProfileTypeDef],
     },
     total=False,
 )
 
-
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
-
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_OptionalContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "SessionStickinessConfig": SessionStickinessConfigTypeDef,
     },
     total=False,
 )
 
-
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    {
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionResultTypeDef = TypedDict(
+    "GetFunctionResultTypeDef",
+    {
+        "FunctionCode": StreamingBody,
+        "ETag": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 UpdateFunctionRequestRequestTypeDef = TypedDict(
     "UpdateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
 
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-    },
-)
-
 _RequiredUpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
     },
 )
@@ -2637,34 +2991,32 @@
     "_OptionalUpdateKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateKeyGroupRequestRequestTypeDef(
     _RequiredUpdateKeyGroupRequestRequestTypeDef, _OptionalUpdateKeyGroupRequestRequestTypeDef
 ):
     pass
 
-
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
 GetOriginAccessControlConfigResultTypeDef = TypedDict(
     "GetOriginAccessControlConfigResultTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOriginAccessControlTypeDef = TypedDict(
     "_RequiredOriginAccessControlTypeDef",
     {
         "Id": str,
@@ -2674,21 +3026,19 @@
     "_OptionalOriginAccessControlTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
     total=False,
 )
 
-
 class OriginAccessControlTypeDef(
     _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
 ):
     pass
 
-
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -2696,35 +3046,33 @@
     "_OptionalUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateOriginAccessControlRequestRequestTypeDef(
     _RequiredUpdateOriginAccessControlRequestRequestTypeDef,
     _OptionalUpdateOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
 GetPublicKeyConfigResultTypeDef = TypedDict(
     "GetPublicKeyConfigResultTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Id": str,
@@ -2744,60 +3092,115 @@
     "_OptionalUpdatePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdatePublicKeyRequestRequestTypeDef(
     _RequiredUpdatePublicKeyRequestRequestTypeDef, _OptionalUpdatePublicKeyRequestRequestTypeDef
 ):
     pass
 
+_RequiredCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_RequiredCustomErrorResponsesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_OptionalCustomErrorResponsesOutputTypeDef",
+    {
+        "Items": List[CustomErrorResponseTypeDef],
+    },
+    total=False,
+)
+
+class CustomErrorResponsesOutputTypeDef(
+    _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
+):
+    pass
 
 _RequiredCustomErrorResponsesTypeDef = TypedDict(
     "_RequiredCustomErrorResponsesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesTypeDef",
     {
-        "Items": List[CustomErrorResponseTypeDef],
+        "Items": Sequence[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
-
 class CustomErrorResponsesTypeDef(
     _RequiredCustomErrorResponsesTypeDef, _OptionalCustomErrorResponsesTypeDef
 ):
     pass
 
+_RequiredCustomHeadersOutputTypeDef = TypedDict(
+    "_RequiredCustomHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomHeadersOutputTypeDef = TypedDict(
+    "_OptionalCustomHeadersOutputTypeDef",
+    {
+        "Items": List[OriginCustomHeaderTypeDef],
+    },
+    total=False,
+)
+
+class CustomHeadersOutputTypeDef(
+    _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
+):
+    pass
 
 _RequiredCustomHeadersTypeDef = TypedDict(
     "_RequiredCustomHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersTypeDef = TypedDict(
     "_OptionalCustomHeadersTypeDef",
     {
-        "Items": List[OriginCustomHeaderTypeDef],
+        "Items": Sequence[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
-
 class CustomHeadersTypeDef(_RequiredCustomHeadersTypeDef, _OptionalCustomHeadersTypeDef):
     pass
 
+_RequiredCustomOriginConfigOutputTypeDef = TypedDict(
+    "_RequiredCustomOriginConfigOutputTypeDef",
+    {
+        "HTTPPort": int,
+        "HTTPSPort": int,
+        "OriginProtocolPolicy": OriginProtocolPolicyType,
+    },
+)
+_OptionalCustomOriginConfigOutputTypeDef = TypedDict(
+    "_OptionalCustomOriginConfigOutputTypeDef",
+    {
+        "OriginSslProtocols": OriginSslProtocolsOutputTypeDef,
+        "OriginReadTimeout": int,
+        "OriginKeepaliveTimeout": int,
+    },
+    total=False,
+)
+
+class CustomOriginConfigOutputTypeDef(
+    _RequiredCustomOriginConfigOutputTypeDef, _OptionalCustomOriginConfigOutputTypeDef
+):
+    pass
 
 _RequiredCustomOriginConfigTypeDef = TypedDict(
     "_RequiredCustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
         "OriginProtocolPolicy": OriginProtocolPolicyType,
@@ -2809,50 +3212,57 @@
         "OriginSslProtocols": OriginSslProtocolsTypeDef,
         "OriginReadTimeout": int,
         "OriginKeepaliveTimeout": int,
     },
     total=False,
 )
 
-
 class CustomOriginConfigTypeDef(
     _RequiredCustomOriginConfigTypeDef, _OptionalCustomOriginConfigTypeDef
 ):
     pass
 
-
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByKeyGroupResultTypeDef = TypedDict(
     "ListDistributionsByKeyGroupResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByOriginRequestPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EncryptionEntityOutputTypeDef = TypedDict(
+    "EncryptionEntityOutputTypeDef",
+    {
+        "PublicKeyId": str,
+        "ProviderId": str,
+        "FieldPatterns": FieldPatternsOutputTypeDef,
     },
 )
 
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
@@ -2871,40 +3281,55 @@
     "_OptionalEndPointTypeDef",
     {
         "KinesisStreamConfig": KinesisStreamConfigTypeDef,
     },
     total=False,
 )
 
-
 class EndPointTypeDef(_RequiredEndPointTypeDef, _OptionalEndPointTypeDef):
     pass
 
+_RequiredFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[FunctionAssociationTypeDef],
+    },
+    total=False,
+)
+
+class FunctionAssociationsOutputTypeDef(
+    _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
+):
+    pass
 
 _RequiredFunctionAssociationsTypeDef = TypedDict(
     "_RequiredFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsTypeDef = TypedDict(
     "_OptionalFunctionAssociationsTypeDef",
     {
-        "Items": List[FunctionAssociationTypeDef],
+        "Items": Sequence[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
-
 class FunctionAssociationsTypeDef(
     _RequiredFunctionAssociationsTypeDef, _OptionalFunctionAssociationsTypeDef
 ):
     pass
 
-
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
@@ -2913,18 +3338,23 @@
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-
 class FunctionSummaryTypeDef(_RequiredFunctionSummaryTypeDef, _OptionalFunctionSummaryTypeDef):
     pass
 
+RestrictionsOutputTypeDef = TypedDict(
+    "RestrictionsOutputTypeDef",
+    {
+        "GeoRestriction": GeoRestrictionOutputTypeDef,
+    },
+)
 
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
 )
@@ -2939,22 +3369,20 @@
     "_OptionalGetDistributionRequestDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetDistributionRequestDistributionDeployedWaitTypeDef(
     _RequiredGetDistributionRequestDistributionDeployedWaitTypeDef,
     _OptionalGetDistributionRequestDistributionDeployedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef = TypedDict(
     "_RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -2962,43 +3390,66 @@
     "_OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetInvalidationRequestInvalidationCompletedWaitTypeDef(
     _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef,
     _OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(
     _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
 ):
     pass
 
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+    },
+)
+
+InvalidationBatchOutputTypeDef = TypedDict(
+    "InvalidationBatchOutputTypeDef",
+    {
+        "Paths": PathsOutputTypeDef,
+        "CallerReference": str,
+    },
+)
 
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
@@ -3018,19 +3469,17 @@
     {
         "NextMarker": str,
         "Items": List[InvalidationSummaryTypeDef],
     },
     total=False,
 )
 
-
 class InvalidationListTypeDef(_RequiredInvalidationListTypeDef, _OptionalInvalidationListTypeDef):
     pass
 
-
 KGKeyPairIdsTypeDef = TypedDict(
     "KGKeyPairIdsTypeDef",
     {
         "KeyGroupId": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
@@ -3041,34 +3490,96 @@
     {
         "AwsAccountNumber": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
 )
 
+_RequiredLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[LambdaFunctionAssociationTypeDef],
+    },
+    total=False,
+)
+
+class LambdaFunctionAssociationsOutputTypeDef(
+    _RequiredLambdaFunctionAssociationsOutputTypeDef,
+    _OptionalLambdaFunctionAssociationsOutputTypeDef,
+):
+    pass
+
 _RequiredLambdaFunctionAssociationsTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsTypeDef",
     {
-        "Items": List[LambdaFunctionAssociationTypeDef],
+        "Items": Sequence[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
-
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
+ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "DistributionId": str,
+    },
+)
+_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
+    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
+):
+    pass
+
+ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
         "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigTypeDef,
     },
     total=False,
@@ -3088,33 +3599,46 @@
     {
         "NextMarker": str,
         "Items": List[OriginAccessControlSummaryTypeDef],
     },
     total=False,
 )
 
-
 class OriginAccessControlListTypeDef(
     _RequiredOriginAccessControlListTypeDef, _OptionalOriginAccessControlListTypeDef
 ):
     pass
 
+OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
+    "OriginGroupFailoverCriteriaOutputTypeDef",
+    {
+        "StatusCodes": StatusCodesOutputTypeDef,
+    },
+)
 
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
 
+OriginGroupMembersOutputTypeDef = TypedDict(
+    "OriginGroupMembersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[OriginGroupMemberTypeDef],
+    },
+)
+
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
+        "Items": Sequence[OriginGroupMemberTypeDef],
     },
 )
 
 _RequiredPublicKeyListTypeDef = TypedDict(
     "_RequiredPublicKeyListTypeDef",
     {
         "MaxItems": int,
@@ -3126,18 +3650,35 @@
     {
         "NextMarker": str,
         "Items": List[PublicKeySummaryTypeDef],
     },
     total=False,
 )
 
-
 class PublicKeyListTypeDef(_RequiredPublicKeyListTypeDef, _OptionalPublicKeyListTypeDef):
     pass
 
+_RequiredQueryArgProfilesOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryArgProfilesOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfilesOutputTypeDef",
+    {
+        "Items": List[QueryArgProfileTypeDef],
+    },
+    total=False,
+)
+
+class QueryArgProfilesOutputTypeDef(
+    _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
+):
+    pass
 
 _RequiredQueryArgProfilesTypeDef = TypedDict(
     "_RequiredQueryArgProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3145,18 +3686,41 @@
     "_OptionalQueryArgProfilesTypeDef",
     {
         "Items": Sequence[QueryArgProfileTypeDef],
     },
     total=False,
 )
 
-
 class QueryArgProfilesTypeDef(_RequiredQueryArgProfilesTypeDef, _OptionalQueryArgProfilesTypeDef):
     pass
 
+_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
+        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
+        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
+        "AccessControlAllowCredentials": bool,
+        "OriginOverride": bool,
+    },
+)
+_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+        "AccessControlMaxAgeSec": int,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyCorsConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCorsConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCorsConfigOutputTypeDef,
+):
+    pass
 
 _RequiredResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
@@ -3169,20 +3733,38 @@
     {
         "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
         "AccessControlMaxAgeSec": int,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyCorsConfigTypeDef(
     _RequiredResponseHeadersPolicyCorsConfigTypeDef, _OptionalResponseHeadersPolicyCorsConfigTypeDef
 ):
     pass
 
+_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyCustomHeaderTypeDef],
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+):
+    pass
 
 _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3190,21 +3772,39 @@
     "_OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyCustomHeaderTypeDef],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyCustomHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef,
 ):
     pass
 
+_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyRemoveHeaderTypeDef],
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+):
+    pass
 
 _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3212,22 +3812,20 @@
     "_OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
-
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -3242,22 +3840,48 @@
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
         "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesTypeDef,
-        "TrustedSigners": TrustedSignersTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
+_RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredStreamingDistributionConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "S3Origin": S3OriginTypeDef,
+        "Comment": str,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalStreamingDistributionConfigOutputTypeDef",
+    {
+        "Aliases": AliasesOutputTypeDef,
+        "Logging": StreamingLoggingConfigTypeDef,
+        "PriceClass": PriceClassType,
+    },
+    total=False,
+)
+
+class StreamingDistributionConfigOutputTypeDef(
+    _RequiredStreamingDistributionConfigOutputTypeDef,
+    _OptionalStreamingDistributionConfigOutputTypeDef,
+):
+    pass
+
 _RequiredStreamingDistributionConfigTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -3270,37 +3894,64 @@
         "Aliases": AliasesTypeDef,
         "Logging": StreamingLoggingConfigTypeDef,
         "PriceClass": PriceClassType,
     },
     total=False,
 )
 
-
 class StreamingDistributionConfigTypeDef(
     _RequiredStreamingDistributionConfigTypeDef, _OptionalStreamingDistributionConfigTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
 
+TagsOutputTypeDef = TypedDict(
+    "TagsOutputTypeDef",
+    {
+        "Items": List[TagTypeDef],
+    },
+    total=False,
+)
+
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredForwardedValuesOutputTypeDef = TypedDict(
+    "_RequiredForwardedValuesOutputTypeDef",
+    {
+        "QueryString": bool,
+        "Cookies": CookiePreferenceOutputTypeDef,
+    },
+)
+_OptionalForwardedValuesOutputTypeDef = TypedDict(
+    "_OptionalForwardedValuesOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+        "QueryStringCacheKeys": QueryStringCacheKeysOutputTypeDef,
+    },
+    total=False,
+)
+
+class ForwardedValuesOutputTypeDef(
+    _RequiredForwardedValuesOutputTypeDef, _OptionalForwardedValuesOutputTypeDef
+):
+    pass
+
 _RequiredForwardedValuesTypeDef = TypedDict(
     "_RequiredForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
     },
 )
@@ -3309,18 +3960,61 @@
     {
         "Headers": HeadersTypeDef,
         "QueryStringCacheKeys": QueryStringCacheKeysTypeDef,
     },
     total=False,
 )
 
-
 class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
     pass
 
+_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingGzip": bool,
+        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingBrotli": bool,
+    },
+    total=False,
+)
+
+class ParametersInCacheKeyAndForwardedToOriginOutputTypeDef(
+    _RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    _OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+):
+    pass
+
+_RequiredOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyConfigOutputTypeDef, _OptionalOriginRequestPolicyConfigOutputTypeDef
+):
+    pass
 
 _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "_RequiredParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
@@ -3331,22 +4025,20 @@
     "_OptionalParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingBrotli": bool,
     },
     total=False,
 )
 
-
 class ParametersInCacheKeyAndForwardedToOriginTypeDef(
     _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef,
     _OptionalParametersInCacheKeyAndForwardedToOriginTypeDef,
 ):
     pass
 
-
 _RequiredOriginRequestPolicyConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyConfigTypeDef",
     {
         "Name": str,
         "HeadersConfig": OriginRequestPolicyHeadersConfigTypeDef,
         "CookiesConfig": OriginRequestPolicyCookiesConfigTypeDef,
         "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigTypeDef,
@@ -3356,64 +4048,81 @@
     "_OptionalOriginRequestPolicyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class OriginRequestPolicyConfigTypeDef(
     _RequiredOriginRequestPolicyConfigTypeDef, _OptionalOriginRequestPolicyConfigTypeDef
 ):
     pass
 
-
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCloudFrontOriginAccessIdentitiesResultTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     {
         "CloudFrontOriginAccessIdentityList": CloudFrontOriginAccessIdentityListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
+_OptionalContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfileConfigOutputTypeDef",
+    {
+        "ContentTypeProfiles": ContentTypeProfilesOutputTypeDef,
+    },
+    total=False,
+)
+
+class ContentTypeProfileConfigOutputTypeDef(
+    _RequiredContentTypeProfileConfigOutputTypeDef, _OptionalContentTypeProfileConfigOutputTypeDef
+):
+    pass
 
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
@@ -3421,21 +4130,19 @@
     "_OptionalContentTypeProfileConfigTypeDef",
     {
         "ContentTypeProfiles": ContentTypeProfilesTypeDef,
     },
     total=False,
 )
 
-
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
-
 _RequiredTrafficConfigTypeDef = TypedDict(
     "_RequiredTrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
 _OptionalTrafficConfigTypeDef = TypedDict(
@@ -3443,110 +4150,98 @@
     {
         "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
         "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
     total=False,
 )
 
-
 class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
     pass
 
-
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
-
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateOriginAccessControlResultTypeDef = TypedDict(
     "CreateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginAccessControlResultTypeDef = TypedDict(
     "GetOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOriginAccessControlResultTypeDef = TypedDict(
     "UpdateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePublicKeyResultTypeDef = TypedDict(
     "CreatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPublicKeyResultTypeDef = TypedDict(
     "GetPublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePublicKeyResultTypeDef = TypedDict(
     "UpdatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredOriginOutputTypeDef = TypedDict(
+    "_RequiredOriginOutputTypeDef",
+    {
+        "Id": str,
+        "DomainName": str,
+    },
+)
+_OptionalOriginOutputTypeDef = TypedDict(
+    "_OptionalOriginOutputTypeDef",
+    {
+        "OriginPath": str,
+        "CustomHeaders": CustomHeadersOutputTypeDef,
+        "S3OriginConfig": S3OriginConfigTypeDef,
+        "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
+        "ConnectionAttempts": int,
+        "ConnectionTimeout": int,
+        "OriginShield": OriginShieldTypeDef,
+        "OriginAccessControlId": str,
+    },
+    total=False,
+)
+
+class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
+    pass
+
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
 )
@@ -3561,18 +4256,35 @@
         "ConnectionTimeout": int,
         "OriginShield": OriginShieldTypeDef,
         "OriginAccessControlId": str,
     },
     total=False,
 )
 
-
 class OriginTypeDef(_RequiredOriginTypeDef, _OptionalOriginTypeDef):
     pass
 
+_RequiredEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_RequiredEncryptionEntitiesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_OptionalEncryptionEntitiesOutputTypeDef",
+    {
+        "Items": List[EncryptionEntityOutputTypeDef],
+    },
+    total=False,
+)
+
+class EncryptionEntitiesOutputTypeDef(
+    _RequiredEncryptionEntitiesOutputTypeDef, _OptionalEncryptionEntitiesOutputTypeDef
+):
+    pass
 
 _RequiredEncryptionEntitiesTypeDef = TypedDict(
     "_RequiredEncryptionEntitiesTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -3580,21 +4292,19 @@
     "_OptionalEncryptionEntitiesTypeDef",
     {
         "Items": Sequence[EncryptionEntityTypeDef],
     },
     total=False,
 )
 
-
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
-
 CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
         "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
@@ -3626,24 +4336,24 @@
 
 CreateFunctionResultTypeDef = TypedDict(
     "CreateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFunctionResultTypeDef = TypedDict(
     "DescribeFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionListTypeDef = TypedDict(
     "_RequiredFunctionListTypeDef",
     {
         "MaxItems": int,
@@ -3655,24 +4365,22 @@
     {
         "NextMarker": str,
         "Items": List[FunctionSummaryTypeDef],
     },
     total=False,
 )
 
-
 class FunctionListTypeDef(_RequiredFunctionListTypeDef, _OptionalFunctionListTypeDef):
     pass
 
-
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestResultTypeDef = TypedDict(
     "TestResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
@@ -3685,41 +4393,77 @@
 )
 
 UpdateFunctionResultTypeDef = TypedDict(
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
     {
-        "DistributionId": str,
-        "InvalidationBatch": InvalidationBatchTypeDef,
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
+        "InvalidationBatch": InvalidationBatchOutputTypeDef,
+    },
+)
+
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
+    {
+        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
+InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActiveTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredActiveTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
@@ -3730,21 +4474,19 @@
     "_OptionalActiveTrustedKeyGroupsTypeDef",
     {
         "Items": List[KGKeyPairIdsTypeDef],
     },
     total=False,
 )
 
-
 class ActiveTrustedKeyGroupsTypeDef(
     _RequiredActiveTrustedKeyGroupsTypeDef, _OptionalActiveTrustedKeyGroupsTypeDef
 ):
     pass
 
-
 _RequiredActiveTrustedSignersTypeDef = TypedDict(
     "_RequiredActiveTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
@@ -3752,50 +4494,57 @@
     "_OptionalActiveTrustedSignersTypeDef",
     {
         "Items": List[SignerTypeDef],
     },
     total=False,
 )
 
-
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
-
 CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
     },
 )
 
 CreateMonitoringSubscriptionResultTypeDef = TypedDict(
     "CreateMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMonitoringSubscriptionResultTypeDef = TypedDict(
     "GetMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OriginGroupOutputTypeDef = TypedDict(
+    "OriginGroupOutputTypeDef",
+    {
+        "Id": str,
+        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
+        "Members": OriginGroupMembersOutputTypeDef,
     },
 )
 
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
@@ -3804,38 +4553,80 @@
     },
 )
 
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenQueryArgProfileIsUnknown": bool,
+    },
+)
+_OptionalQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfileConfigOutputTypeDef",
+    {
+        "QueryArgProfiles": QueryArgProfilesOutputTypeDef,
     },
+    total=False,
 )
 
+class QueryArgProfileConfigOutputTypeDef(
+    _RequiredQueryArgProfileConfigOutputTypeDef, _OptionalQueryArgProfileConfigOutputTypeDef
+):
+    pass
+
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
 _OptionalQueryArgProfileConfigTypeDef = TypedDict(
     "_OptionalQueryArgProfileConfigTypeDef",
     {
         "QueryArgProfiles": QueryArgProfilesTypeDef,
     },
     total=False,
 )
 
-
 class QueryArgProfileConfigTypeDef(
     _RequiredQueryArgProfileConfigTypeDef, _OptionalQueryArgProfileConfigTypeDef
 ):
     pass
 
+_RequiredResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
+        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigTypeDef,
+        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
+        "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+        "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyConfigOutputTypeDef,
+):
+    pass
 
 _RequiredResponseHeadersPolicyConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
     },
 )
@@ -3848,21 +4639,19 @@
         "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
         "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigTypeDef,
         "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyConfigTypeDef(
     _RequiredResponseHeadersPolicyConfigTypeDef, _OptionalResponseHeadersPolicyConfigTypeDef
 ):
     pass
 
-
 _RequiredStreamingDistributionListTypeDef = TypedDict(
     "_RequiredStreamingDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -3873,37 +4662,38 @@
     {
         "NextMarker": str,
         "Items": List[StreamingDistributionSummaryTypeDef],
     },
     total=False,
 )
 
-
 class StreamingDistributionListTypeDef(
     _RequiredStreamingDistributionListTypeDef, _OptionalStreamingDistributionListTypeDef
 ):
     pass
 
-
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StreamingDistributionConfigUnionTypeDef = Union[
+    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+]
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -3911,27 +4701,25 @@
     "_OptionalUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateStreamingDistributionRequestRequestTypeDef(
     _RequiredUpdateStreamingDistributionRequestRequestTypeDef,
     _OptionalUpdateStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": TagsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3943,14 +4731,86 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
+TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
+_RequiredCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorOutputTypeDef",
+    {
+        "PathPattern": str,
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+class CacheBehaviorOutputTypeDef(
+    _RequiredCacheBehaviorOutputTypeDef, _OptionalCacheBehaviorOutputTypeDef
+):
+    pass
+
+_RequiredDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+class DefaultCacheBehaviorOutputTypeDef(
+    _RequiredDefaultCacheBehaviorOutputTypeDef, _OptionalDefaultCacheBehaviorOutputTypeDef
+):
+    pass
+
 _RequiredCacheBehaviorTypeDef = TypedDict(
     "_RequiredCacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -3974,19 +4834,17 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
-
 class CacheBehaviorTypeDef(_RequiredCacheBehaviorTypeDef, _OptionalCacheBehaviorTypeDef):
     pass
 
-
 _RequiredDefaultCacheBehaviorTypeDef = TypedDict(
     "_RequiredDefaultCacheBehaviorTypeDef",
     {
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
 )
@@ -4009,71 +4867,95 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
-
 class DefaultCacheBehaviorTypeDef(
     _RequiredDefaultCacheBehaviorTypeDef, _OptionalDefaultCacheBehaviorTypeDef
 ):
     pass
 
-
-_RequiredCachePolicyConfigTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigTypeDef",
+_RequiredCachePolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigOutputTypeDef",
     {
         "Name": str,
         "MinTTL": int,
     },
 )
-_OptionalCachePolicyConfigTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigTypeDef",
+_OptionalCachePolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigOutputTypeDef",
     {
         "Comment": str,
         "DefaultTTL": int,
         "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+        "ParametersInCacheKeyAndForwardedToOrigin": (
+            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
+        ),
     },
     total=False,
 )
 
-
-class CachePolicyConfigTypeDef(
-    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+class CachePolicyConfigOutputTypeDef(
+    _RequiredCachePolicyConfigOutputTypeDef, _OptionalCachePolicyConfigOutputTypeDef
 ):
     pass
 
-
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
-    },
-)
-
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+    },
+)
+
+_RequiredCachePolicyConfigTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigTypeDef",
+    {
+        "Name": str,
+        "MinTTL": int,
+    },
+)
+_OptionalCachePolicyConfigTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigTypeDef",
+    {
+        "Comment": str,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyConfigTypeDef(
+    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+):
+    pass
+
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
+OriginRequestPolicyConfigUnionTypeDef = Union[
+    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+]
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -4081,21 +4963,40 @@
     "_OptionalUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateOriginRequestPolicyRequestRequestTypeDef(
     _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef,
     _OptionalUpdateOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
+_RequiredContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "TrafficConfig": TrafficConfigTypeDef,
+    },
+    total=False,
+)
+
+class ContinuousDeploymentPolicyConfigOutputTypeDef(
+    _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
+    _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
+):
+    pass
 
 _RequiredContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
     },
@@ -4104,113 +5005,116 @@
     "_OptionalContinuousDeploymentPolicyConfigTypeDef",
     {
         "TrafficConfig": TrafficConfigTypeDef,
     },
     total=False,
 )
 
-
 class ContinuousDeploymentPolicyConfigTypeDef(
     _RequiredContinuousDeploymentPolicyConfigTypeDef,
     _OptionalContinuousDeploymentPolicyConfigTypeDef,
 ):
     pass
 
-
-_RequiredKeyGroupListTypeDef = TypedDict(
-    "_RequiredKeyGroupListTypeDef",
+OriginsOutputTypeDef = TypedDict(
+    "OriginsOutputTypeDef",
     {
-        "MaxItems": int,
         "Quantity": int,
+        "Items": List[OriginOutputTypeDef],
     },
 )
-_OptionalKeyGroupListTypeDef = TypedDict(
-    "_OptionalKeyGroupListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[KeyGroupSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
-    pass
-
 
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginTypeDef],
+        "Items": Sequence[OriginTypeDef],
     },
 )
 
-_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
-class FieldLevelEncryptionProfileConfigTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+class FieldLevelEncryptionProfileConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigOutputTypeDef,
 ):
     pass
 
-
 _RequiredFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
 _OptionalFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-
 class FieldLevelEncryptionProfileSummaryTypeDef(
     _RequiredFieldLevelEncryptionProfileSummaryTypeDef,
     _OptionalFieldLevelEncryptionProfileSummaryTypeDef,
 ):
     pass
 
+_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Name": str,
+        "CallerReference": str,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
+    },
+)
+_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class FieldLevelEncryptionProfileConfigTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+):
+    pass
 
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRealtimeLogConfigResultTypeDef = TypedDict(
     "GetRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRealtimeLogConfigsTypeDef = TypedDict(
     "_RequiredRealtimeLogConfigsTypeDef",
     {
         "MaxItems": int,
@@ -4223,179 +5127,232 @@
     {
         "Items": List[RealtimeLogConfigTypeDef],
         "NextMarker": str,
     },
     total=False,
 )
 
-
 class RealtimeLogConfigsTypeDef(
     _RequiredRealtimeLogConfigsTypeDef, _OptionalRealtimeLogConfigsTypeDef
 ):
     pass
 
-
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResultTypeDef = TypedDict(
     "ListFunctionsResultTypeDef",
     {
         "FunctionList": FunctionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFunctionResultTypeDef = TypedDict(
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredKeyGroupListTypeDef = TypedDict(
+    "_RequiredKeyGroupListTypeDef",
+    {
+        "MaxItems": int,
+        "Quantity": int,
+    },
+)
+_OptionalKeyGroupListTypeDef = TypedDict(
+    "_OptionalKeyGroupListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[KeyGroupSummaryTypeDef],
+    },
+    total=False,
+)
+
+class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
+    pass
+
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvalidationResultTypeDef = TypedDict(
     "GetInvalidationResultTypeDef",
     {
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStreamingDistributionTypeDef = TypedDict(
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
     },
 )
 _OptionalStreamingDistributionTypeDef = TypedDict(
     "_OptionalStreamingDistributionTypeDef",
     {
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-
 class StreamingDistributionTypeDef(
     _RequiredStreamingDistributionTypeDef, _OptionalStreamingDistributionTypeDef
 ):
     pass
 
+_RequiredOriginGroupsOutputTypeDef = TypedDict(
+    "_RequiredOriginGroupsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalOriginGroupsOutputTypeDef = TypedDict(
+    "_OptionalOriginGroupsOutputTypeDef",
+    {
+        "Items": List[OriginGroupOutputTypeDef],
+    },
+    total=False,
+)
+
+class OriginGroupsOutputTypeDef(
+    _RequiredOriginGroupsOutputTypeDef, _OptionalOriginGroupsOutputTypeDef
+):
+    pass
 
 _RequiredOriginGroupsTypeDef = TypedDict(
     "_RequiredOriginGroupsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalOriginGroupsTypeDef = TypedDict(
     "_OptionalOriginGroupsTypeDef",
     {
-        "Items": List[OriginGroupTypeDef],
+        "Items": Sequence[OriginGroupTypeDef],
     },
     total=False,
 )
 
-
 class OriginGroupsTypeDef(_RequiredOriginGroupsTypeDef, _OptionalOriginGroupsTypeDef):
     pass
 
-
-_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigTypeDef",
+_RequiredFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigOutputTypeDef",
     {
         "CallerReference": str,
     },
 )
-_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigTypeDef",
+_OptionalFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigOutputTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
-
-class FieldLevelEncryptionConfigTypeDef(
-    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+class FieldLevelEncryptionConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionConfigOutputTypeDef,
 ):
     pass
 
-
 _RequiredFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
     },
 )
 _OptionalFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionSummaryTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
-
 class FieldLevelEncryptionSummaryTypeDef(
     _RequiredFieldLevelEncryptionSummaryTypeDef, _OptionalFieldLevelEncryptionSummaryTypeDef
 ):
     pass
 
-
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "CallerReference": str,
     },
 )
+_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigTypeDef",
+    {
+        "Comment": str,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+    },
+    total=False,
+)
+
+class FieldLevelEncryptionConfigTypeDef(
+    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+):
+    pass
 
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+    },
+)
+
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
+ResponseHeadersPolicyConfigUnionTypeDef = Union[
+    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+]
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -4403,119 +5360,105 @@
     "_OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
 
+_RequiredCacheBehaviorsOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCacheBehaviorsOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorsOutputTypeDef",
+    {
+        "Items": List[CacheBehaviorOutputTypeDef],
+    },
+    total=False,
+)
+
+class CacheBehaviorsOutputTypeDef(
+    _RequiredCacheBehaviorsOutputTypeDef, _OptionalCacheBehaviorsOutputTypeDef
+):
+    pass
+
 _RequiredCacheBehaviorsTypeDef = TypedDict(
     "_RequiredCacheBehaviorsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCacheBehaviorsTypeDef = TypedDict(
     "_OptionalCacheBehaviorsTypeDef",
     {
-        "Items": List[CacheBehaviorTypeDef],
+        "Items": Sequence[CacheBehaviorTypeDef],
     },
     total=False,
 )
 
-
 class CacheBehaviorsTypeDef(_RequiredCacheBehaviorsTypeDef, _OptionalCacheBehaviorsTypeDef):
     pass
 
-
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
     },
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-
-class UpdateCachePolicyRequestRequestTypeDef(
-    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
-):
-    pass
-
 
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginRequestPolicyResultTypeDef = TypedDict(
     "GetOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicySummaryTypeDef = TypedDict(
     "OriginRequestPolicySummaryTypeDef",
     {
         "Type": OriginRequestPolicyTypeType,
@@ -4524,40 +5467,71 @@
 )
 
 UpdateOriginRequestPolicyResultTypeDef = TypedDict(
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+
+_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+class UpdateCachePolicyRequestRequestTypeDef(
+    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
+):
+    pass
+
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
     },
 )
 
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
+ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
+    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+]
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -4568,55 +5542,69 @@
     "_OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
+FieldLevelEncryptionProfileTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileTypeDef",
     {
-        "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
     },
 )
 
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
+    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FieldLevelEncryptionProfileTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileTypeDef",
+_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
+_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+    },
+    total=False,
+)
 
-GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
-    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
+class FieldLevelEncryptionProfileListTypeDef(
+    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
+):
+    pass
+
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
+    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+]
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "Id": str,
     },
 )
@@ -4624,178 +5612,160 @@
     "_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
-
 class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-    },
-)
-_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+ListRealtimeLogConfigsResultTypeDef = TypedDict(
+    "ListRealtimeLogConfigsResultTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class FieldLevelEncryptionProfileListTypeDef(
-    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
-):
-    pass
-
-
-ListRealtimeLogConfigsResultTypeDef = TypedDict(
-    "ListRealtimeLogConfigsResultTypeDef",
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
     {
-        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "KeyGroupList": KeyGroupListTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsResultTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingDistributionResultTypeDef = TypedDict(
     "GetStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStreamingDistributionResultTypeDef = TypedDict(
     "UpdateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
     },
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionListTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
-_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionSummaryTypeDef],
     },
     total=False,
 )
 
-
-class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
-    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
-    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+class FieldLevelEncryptionListTypeDef(
+    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
 ):
     pass
 
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+    },
+)
 
-_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionListTypeDef",
+FieldLevelEncryptionConfigUnionTypeDef = Union[
+    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+]
+_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
     },
 )
-_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionListTypeDef",
+_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionSummaryTypeDef],
+        "IfMatch": str,
     },
     total=False,
 )
 
-
-class FieldLevelEncryptionListTypeDef(
-    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
+class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
+    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResponseHeadersPolicyResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicySummaryTypeDef = TypedDict(
     "ResponseHeadersPolicySummaryTypeDef",
     {
         "Type": ResponseHeadersPolicyTypeType,
@@ -4804,95 +5774,127 @@
 )
 
 UpdateResponseHeadersPolicyResultTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDistributionConfigTypeDef = TypedDict(
-    "_RequiredDistributionConfigTypeDef",
+_RequiredDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
         "Comment": str,
         "Enabled": bool,
     },
 )
-_OptionalDistributionConfigTypeDef = TypedDict(
-    "_OptionalDistributionConfigTypeDef",
+_OptionalDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalDistributionConfigOutputTypeDef",
     {
-        "Aliases": AliasesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
         "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Logging": LoggingConfigTypeDef,
         "PriceClass": PriceClassType,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
     total=False,
 )
 
-
-class DistributionConfigTypeDef(
-    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+class DistributionConfigOutputTypeDef(
+    _RequiredDistributionConfigOutputTypeDef, _OptionalDistributionConfigOutputTypeDef
 ):
     pass
 
-
 _RequiredDistributionSummaryTypeDef = TypedDict(
     "_RequiredDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesTypeDef,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
 _OptionalDistributionSummaryTypeDef = TypedDict(
     "_OptionalDistributionSummaryTypeDef",
     {
-        "OriginGroups": OriginGroupsTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
-
 class DistributionSummaryTypeDef(
     _RequiredDistributionSummaryTypeDef, _OptionalDistributionSummaryTypeDef
 ):
     pass
 
+_RequiredDistributionConfigTypeDef = TypedDict(
+    "_RequiredDistributionConfigTypeDef",
+    {
+        "CallerReference": str,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Comment": str,
+        "Enabled": bool,
+    },
+)
+_OptionalDistributionConfigTypeDef = TypedDict(
+    "_OptionalDistributionConfigTypeDef",
+    {
+        "Aliases": AliasesTypeDef,
+        "DefaultRootObject": str,
+        "OriginGroups": OriginGroupsTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Logging": LoggingConfigTypeDef,
+        "PriceClass": PriceClassType,
+        "ViewerCertificate": ViewerCertificateTypeDef,
+        "Restrictions": RestrictionsTypeDef,
+        "WebACLId": str,
+        "HttpVersion": HttpVersionType,
+        "IsIPV6Enabled": bool,
+        "ContinuousDeploymentPolicyId": str,
+        "Staging": bool,
+    },
+    total=False,
+)
+
+class DistributionConfigTypeDef(
+    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+):
+    pass
 
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
     },
@@ -4900,33 +5902,33 @@
 
 CreateCachePolicyResultTypeDef = TypedDict(
     "CreateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCachePolicyResultTypeDef = TypedDict(
     "GetCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCachePolicyResultTypeDef = TypedDict(
     "UpdateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOriginRequestPolicyListTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4938,125 +5940,123 @@
     {
         "NextMarker": str,
         "Items": List[OriginRequestPolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class OriginRequestPolicyListTypeDef(
     _RequiredOriginRequestPolicyListTypeDef, _OptionalOriginRequestPolicyListTypeDef
 ):
     pass
 
-
 ContinuousDeploymentPolicySummaryTypeDef = TypedDict(
     "ContinuousDeploymentPolicySummaryTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
     },
 )
 
 CreateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionProfilesResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     {
         "FieldLevelEncryptionProfileList": FieldLevelEncryptionProfileListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionConfigsResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     {
         "FieldLevelEncryptionList": FieldLevelEncryptionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResponseHeadersPolicyListTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -5068,94 +6068,52 @@
     {
         "NextMarker": str,
         "Items": List[ResponseHeadersPolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class ResponseHeadersPolicyListTypeDef(
     _RequiredResponseHeadersPolicyListTypeDef, _OptionalResponseHeadersPolicyListTypeDef
 ):
     pass
 
-
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
     "_OptionalDistributionTypeDef",
     {
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
         "ActiveTrustedKeyGroups": ActiveTrustedKeyGroupsTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
-
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
-
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-
-class UpdateDistributionRequestRequestTypeDef(
-    _RequiredUpdateDistributionRequestRequestTypeDef,
-    _OptionalUpdateDistributionRequestRequestTypeDef,
-):
-    pass
-
 
 _RequiredDistributionListTypeDef = TypedDict(
     "_RequiredDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
@@ -5167,18 +6125,53 @@
     {
         "NextMarker": str,
         "Items": List[DistributionSummaryTypeDef],
     },
     total=False,
 )
 
-
 class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
     pass
 
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+
+DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
+
+_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+class UpdateDistributionRequestRequestTypeDef(
+    _RequiredUpdateDistributionRequestRequestTypeDef,
+    _OptionalUpdateDistributionRequestRequestTypeDef,
+):
+    pass
 
 _RequiredCachePolicyListTypeDef = TypedDict(
     "_RequiredCachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
     },
@@ -5188,24 +6181,22 @@
     {
         "NextMarker": str,
         "Items": List[CachePolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class CachePolicyListTypeDef(_RequiredCachePolicyListTypeDef, _OptionalCachePolicyListTypeDef):
     pass
 
-
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContinuousDeploymentPolicyListTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -5217,125 +6208,123 @@
     {
         "NextMarker": str,
         "Items": List[ContinuousDeploymentPolicySummaryTypeDef],
     },
     total=False,
 )
 
-
 class ContinuousDeploymentPolicyListTypeDef(
     _RequiredContinuousDeploymentPolicyListTypeDef, _OptionalContinuousDeploymentPolicyListTypeDef
 ):
     pass
 
-
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionWithTagsResultTypeDef = TypedDict(
     "CreateDistributionWithTagsResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionResultTypeDef = TypedDict(
     "GetDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionWithStagingConfigResultTypeDef = TypedDict(
     "UpdateDistributionWithStagingConfigResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByRealtimeLogConfigResultTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByWebACLIdResultTypeDef = TypedDict(
     "ListDistributionsByWebACLIdResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
     },
 )
 
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListContinuousDeploymentPoliciesResultTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesResultTypeDef",
     {
         "ContinuousDeploymentPolicyList": ContinuousDeploymentPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/type_defs.pyi` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudfront.type_defs import AliasICPRecordalTypeDef
 
-    data: AliasICPRecordalTypeDef = {...}
+    data: AliasICPRecordalTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -55,38 +55,50 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasICPRecordalTypeDef",
+    "AliasesOutputTypeDef",
     "AliasesTypeDef",
+    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
+    "BlobTypeDef",
+    "TrustedKeyGroupsOutputTypeDef",
+    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
+    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
+    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
     "ContentTypeProfileTypeDef",
+    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
     "CustomErrorResponseTypeDef",
     "OriginCustomHeaderTypeDef",
+    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -99,20 +111,22 @@
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
     "KinesisStreamConfigTypeDef",
+    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
     "FunctionAssociationTypeDef",
     "FunctionMetadataTypeDef",
+    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -120,271 +134,332 @@
     "WaiterConfigTypeDef",
     "GetDistributionRequestRequestTypeDef",
     "GetFieldLevelEncryptionConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
-    "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
+    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
+    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
     "ListDistributionsByKeyGroupRequestRequestTypeDef",
     "ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef",
     "ListDistributionsByWebACLIdRequestRequestTypeDef",
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
     "ListDistributionsRequestRequestTypeDef",
     "ListFieldLevelEncryptionConfigsRequestRequestTypeDef",
     "ListFieldLevelEncryptionProfilesRequestRequestTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
     "ListInvalidationsRequestRequestTypeDef",
     "ListKeyGroupsRequestRequestTypeDef",
     "ListOriginAccessControlsRequestRequestTypeDef",
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
+    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
     "OriginGroupMemberTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
     "QueryArgProfileTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
+    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
-    "ResponseMetadataTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
-    "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
+    "TestFunctionRequestRequestTypeDef",
+    "CachePolicyCookiesConfigOutputTypeDef",
+    "CookiePreferenceOutputTypeDef",
+    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
+    "CachePolicyHeadersConfigOutputTypeDef",
+    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
+    "CachePolicyQueryStringsConfigOutputTypeDef",
+    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
+    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    "GetFunctionResultTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
     "GetOriginAccessControlConfigResultTypeDef",
     "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
     "GetPublicKeyConfigResultTypeDef",
     "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
+    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
+    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
+    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
+    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
     "EndPointTypeDef",
+    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
+    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupConfigUnionTypeDef",
+    "KeyGroupTypeDef",
+    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
+    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    "ListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
+    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
+    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
+    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
+    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
+    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
+    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
+    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "TagsOutputTypeDef",
     "TagsTypeDef",
+    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
+    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
+    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
     "TrafficConfigTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
     "CreateOriginAccessControlResultTypeDef",
     "GetOriginAccessControlResultTypeDef",
     "UpdateOriginAccessControlResultTypeDef",
     "CreatePublicKeyResultTypeDef",
     "GetPublicKeyResultTypeDef",
     "UpdatePublicKeyResultTypeDef",
+    "OriginOutputTypeDef",
     "OriginTypeDef",
+    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
-    "CreateInvalidationRequestRequestTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
     "InvalidationTypeDef",
+    "CreateInvalidationRequestRequestTypeDef",
+    "InvalidationBatchUnionTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
+    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
+    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
+    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "CreateStreamingDistributionRequestRequestTypeDef",
     "GetStreamingDistributionConfigResultTypeDef",
+    "CreateStreamingDistributionRequestRequestTypeDef",
+    "StreamingDistributionConfigUnionTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagsUnionTypeDef",
+    "CacheBehaviorOutputTypeDef",
+    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigTypeDef",
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "CachePolicyConfigOutputTypeDef",
     "GetOriginRequestPolicyConfigResultTypeDef",
     "OriginRequestPolicyTypeDef",
+    "CachePolicyConfigTypeDef",
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "OriginRequestPolicyConfigUnionTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
+    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "KeyGroupListTypeDef",
+    "OriginsOutputTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileConfigOutputTypeDef",
     "FieldLevelEncryptionProfileSummaryTypeDef",
+    "FieldLevelEncryptionProfileConfigTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
+    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
+    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionConfigOutputTypeDef",
     "FieldLevelEncryptionSummaryTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
+    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
+    "CachePolicyConfigUnionTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
+    "ContinuousDeploymentPolicyConfigUnionTypeDef",
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
-    "ListKeyGroupsResultTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileListTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileConfigUnionTypeDef",
+    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
+    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionListTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigUnionTypeDef",
+    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigTypeDef",
+    "DistributionConfigOutputTypeDef",
     "DistributionSummaryTypeDef",
+    "DistributionConfigTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -395,167 +470,313 @@
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigWithTagsTypeDef",
     "DistributionTypeDef",
     "GetDistributionConfigResultTypeDef",
-    "UpdateDistributionRequestRequestTypeDef",
     "DistributionListTypeDef",
+    "CreateDistributionRequestRequestTypeDef",
+    "DistributionConfigUnionTypeDef",
+    "DistributionConfigWithTagsTypeDef",
+    "UpdateDistributionRequestRequestTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": str,
         "ICPRecordalStatus": ICPRecordalStatusType,
     },
     total=False,
 )
 
+_RequiredAliasesOutputTypeDef = TypedDict(
+    "_RequiredAliasesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalAliasesOutputTypeDef = TypedDict(
+    "_OptionalAliasesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class AliasesOutputTypeDef(_RequiredAliasesOutputTypeDef, _OptionalAliasesOutputTypeDef):
+    pass
+
+
 _RequiredAliasesTypeDef = TypedDict(
     "_RequiredAliasesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalAliasesTypeDef = TypedDict(
     "_OptionalAliasesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class AliasesTypeDef(_RequiredAliasesTypeDef, _OptionalAliasesTypeDef):
     pass
 
+
+CachedMethodsOutputTypeDef = TypedDict(
+    "CachedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": List[MethodType],
+        "Items": Sequence[MethodType],
     },
 )
 
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_RequiredTrustedKeyGroupsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_OptionalTrustedKeyGroupsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class TrustedKeyGroupsOutputTypeDef(
+    _RequiredTrustedKeyGroupsOutputTypeDef, _OptionalTrustedKeyGroupsOutputTypeDef
+):
+    pass
+
+
+_RequiredTrustedSignersOutputTypeDef = TypedDict(
+    "_RequiredTrustedSignersOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedSignersOutputTypeDef = TypedDict(
+    "_OptionalTrustedSignersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class TrustedSignersOutputTypeDef(
+    _RequiredTrustedSignersOutputTypeDef, _OptionalTrustedSignersOutputTypeDef
+):
+    pass
+
+
 _RequiredTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedKeyGroupsTypeDef = TypedDict(
     "_OptionalTrustedKeyGroupsTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class TrustedKeyGroupsTypeDef(_RequiredTrustedKeyGroupsTypeDef, _OptionalTrustedKeyGroupsTypeDef):
     pass
 
+
 _RequiredTrustedSignersTypeDef = TypedDict(
     "_RequiredTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedSignersTypeDef = TypedDict(
     "_OptionalTrustedSignersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
     pass
 
+
+_RequiredCookieNamesOutputTypeDef = TypedDict(
+    "_RequiredCookieNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCookieNamesOutputTypeDef = TypedDict(
+    "_OptionalCookieNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class CookieNamesOutputTypeDef(
+    _RequiredCookieNamesOutputTypeDef, _OptionalCookieNamesOutputTypeDef
+):
+    pass
+
+
 _RequiredCookieNamesTypeDef = TypedDict(
     "_RequiredCookieNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCookieNamesTypeDef = TypedDict(
     "_OptionalCookieNamesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
     pass
 
+
+_RequiredHeadersOutputTypeDef = TypedDict(
+    "_RequiredHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalHeadersOutputTypeDef = TypedDict(
+    "_OptionalHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class HeadersOutputTypeDef(_RequiredHeadersOutputTypeDef, _OptionalHeadersOutputTypeDef):
+    pass
+
+
 _RequiredHeadersTypeDef = TypedDict(
     "_RequiredHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalHeadersTypeDef = TypedDict(
     "_OptionalHeadersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
     pass
 
+
+_RequiredQueryStringNamesOutputTypeDef = TypedDict(
+    "_RequiredQueryStringNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringNamesOutputTypeDef = TypedDict(
+    "_OptionalQueryStringNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class QueryStringNamesOutputTypeDef(
+    _RequiredQueryStringNamesOutputTypeDef, _OptionalQueryStringNamesOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryStringNamesTypeDef = TypedDict(
     "_RequiredQueryStringNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringNamesTypeDef = TypedDict(
     "_OptionalQueryStringNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
+
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -590,38 +811,64 @@
     "_OptionalContentTypeProfileTypeDef",
     {
         "ProfileId": str,
     },
     total=False,
 )
 
+
 class ContentTypeProfileTypeDef(
     _RequiredContentTypeProfileTypeDef, _OptionalContentTypeProfileTypeDef
 ):
     pass
 
+
+_RequiredStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_RequiredStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_OptionalStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class StagingDistributionDnsNamesOutputTypeDef(
+    _RequiredStagingDistributionDnsNamesOutputTypeDef,
+    _OptionalStagingDistributionDnsNamesOutputTypeDef,
+):
+    pass
+
+
 _RequiredStagingDistributionDnsNamesTypeDef = TypedDict(
     "_RequiredStagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalStagingDistributionDnsNamesTypeDef = TypedDict(
     "_OptionalStagingDistributionDnsNamesTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
+
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
@@ -646,19 +893,32 @@
     {
         "Staging": bool,
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class CopyDistributionRequestRequestTypeDef(
     _RequiredCopyDistributionRequestRequestTypeDef, _OptionalCopyDistributionRequestRequestTypeDef
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
 FunctionConfigTypeDef = TypedDict(
     "FunctionConfigTypeDef",
     {
         "Comment": str,
         "Runtime": Literal["cloudfront-js-1.0"],
     },
 )
@@ -674,17 +934,19 @@
     "_OptionalKeyGroupConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class KeyGroupConfigTypeDef(_RequiredKeyGroupConfigTypeDef, _OptionalKeyGroupConfigTypeDef):
     pass
 
+
 _RequiredOriginAccessControlConfigTypeDef = TypedDict(
     "_RequiredOriginAccessControlConfigTypeDef",
     {
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
@@ -694,19 +956,21 @@
     "_OptionalOriginAccessControlConfigTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class OriginAccessControlConfigTypeDef(
     _RequiredOriginAccessControlConfigTypeDef, _OptionalOriginAccessControlConfigTypeDef
 ):
     pass
 
+
 _RequiredPublicKeyConfigTypeDef = TypedDict(
     "_RequiredPublicKeyConfigTypeDef",
     {
         "CallerReference": str,
         "Name": str,
         "EncodedKey": str,
     },
@@ -715,17 +979,19 @@
     "_OptionalPublicKeyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
+
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -734,32 +1000,42 @@
         "ResponsePagePath": str,
         "ResponseCode": str,
         "ErrorCachingMinTTL": int,
     },
     total=False,
 )
 
+
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
+
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+OriginSslProtocolsOutputTypeDef = TypedDict(
+    "OriginSslProtocolsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[SslProtocolType],
+    },
+)
+
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": List[SslProtocolType],
+        "Items": Sequence[SslProtocolType],
     },
 )
 
 _RequiredDeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
@@ -769,119 +1045,131 @@
     "_OptionalDeleteCachePolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteCachePolicyRequestRequestTypeDef(
     _RequiredDeleteCachePolicyRequestRequestTypeDef, _OptionalDeleteCachePolicyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalDeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalDeleteContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteDistributionRequestRequestTypeDef(
     _RequiredDeleteDistributionRequestRequestTypeDef,
     _OptionalDeleteDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteFieldLevelEncryptionConfigRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalDeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteFunctionRequestRequestTypeDef = TypedDict(
     "DeleteFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -896,19 +1184,21 @@
     "_OptionalDeleteKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteKeyGroupRequestRequestTypeDef(
     _RequiredDeleteKeyGroupRequestRequestTypeDef, _OptionalDeleteKeyGroupRequestRequestTypeDef
 ):
     pass
 
+
 DeleteMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 
@@ -922,59 +1212,65 @@
     "_OptionalDeleteOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteOriginAccessControlRequestRequestTypeDef(
     _RequiredDeleteOriginAccessControlRequestRequestTypeDef,
     _OptionalDeleteOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteOriginRequestPolicyRequestRequestTypeDef(
     _RequiredDeleteOriginRequestPolicyRequestRequestTypeDef,
     _OptionalDeleteOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeletePublicKeyRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeletePublicKeyRequestRequestTypeDef(
     _RequiredDeletePublicKeyRequestRequestTypeDef, _OptionalDeletePublicKeyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "ARN": str,
     },
     total=False,
@@ -990,59 +1286,65 @@
     "_OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredDeleteResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalDeleteResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class DeleteStreamingDistributionRequestRequestTypeDef(
     _RequiredDeleteStreamingDistributionRequestRequestTypeDef,
     _OptionalDeleteStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFunctionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeFunctionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
+
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1077,25 +1379,41 @@
     {
         "NextMarker": str,
         "Items": List[str],
     },
     total=False,
 )
 
+
 class DistributionIdListTypeDef(
     _RequiredDistributionIdListTypeDef, _OptionalDistributionIdListTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+
+_RequiredFieldPatternsOutputTypeDef = TypedDict(
+    "_RequiredFieldPatternsOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Quantity": int,
     },
 )
+_OptionalFieldPatternsOutputTypeDef = TypedDict(
+    "_OptionalFieldPatternsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class FieldPatternsOutputTypeDef(
+    _RequiredFieldPatternsOutputTypeDef, _OptionalFieldPatternsOutputTypeDef
+):
+    pass
+
 
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
@@ -1103,44 +1421,69 @@
     "_OptionalFieldPatternsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
+
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
 
+_RequiredQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_RequiredQueryStringCacheKeysOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_OptionalQueryStringCacheKeysOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class QueryStringCacheKeysOutputTypeDef(
+    _RequiredQueryStringCacheKeysOutputTypeDef, _OptionalQueryStringCacheKeysOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryStringCacheKeysTypeDef = TypedDict(
     "_RequiredQueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringCacheKeysTypeDef = TypedDict(
     "_OptionalQueryStringCacheKeysTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
+
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1157,35 +1500,61 @@
     {
         "Stage": FunctionStageType,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
+
 class FunctionMetadataTypeDef(_RequiredFunctionMetadataTypeDef, _OptionalFunctionMetadataTypeDef):
     pass
 
+
+_RequiredGeoRestrictionOutputTypeDef = TypedDict(
+    "_RequiredGeoRestrictionOutputTypeDef",
+    {
+        "RestrictionType": GeoRestrictionTypeType,
+        "Quantity": int,
+    },
+)
+_OptionalGeoRestrictionOutputTypeDef = TypedDict(
+    "_OptionalGeoRestrictionOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class GeoRestrictionOutputTypeDef(
+    _RequiredGeoRestrictionOutputTypeDef, _OptionalGeoRestrictionOutputTypeDef
+):
+    pass
+
+
 _RequiredGeoRestrictionTypeDef = TypedDict(
     "_RequiredGeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
     },
 )
 _OptionalGeoRestrictionTypeDef = TypedDict(
     "_OptionalGeoRestrictionTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class GeoRestrictionTypeDef(_RequiredGeoRestrictionTypeDef, _OptionalGeoRestrictionTypeDef):
     pass
 
+
 GetCachePolicyConfigRequestRequestTypeDef = TypedDict(
     "GetCachePolicyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1285,28 +1654,20 @@
     "_OptionalGetFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+
 class GetFunctionRequestRequestTypeDef(
     _RequiredGetFunctionRequestRequestTypeDef, _OptionalGetFunctionRequestRequestTypeDef
 ):
     pass
 
-GetFunctionResultTypeDef = TypedDict(
-    "GetFunctionResultTypeDef",
-    {
-        "FunctionCode": StreamingBody,
-        "ETag": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetInvalidationRequestRequestTypeDef = TypedDict(
     "GetInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
@@ -1315,14 +1676,36 @@
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredKeyGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredKeyGroupConfigOutputTypeDef",
+    {
+        "Name": str,
+        "Items": List[str],
+    },
+)
+_OptionalKeyGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalKeyGroupConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class KeyGroupConfigOutputTypeDef(
+    _RequiredKeyGroupConfigOutputTypeDef, _OptionalKeyGroupConfigOutputTypeDef
+):
+    pass
+
+
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1408,31 +1791,52 @@
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredPathsOutputTypeDef = TypedDict(
+    "_RequiredPathsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalPathsOutputTypeDef = TypedDict(
+    "_OptionalPathsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class PathsOutputTypeDef(_RequiredPathsOutputTypeDef, _OptionalPathsOutputTypeDef):
+    pass
+
+
 _RequiredPathsTypeDef = TypedDict(
     "_RequiredPathsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalPathsTypeDef = TypedDict(
     "_OptionalPathsTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class PathsTypeDef(_RequiredPathsTypeDef, _OptionalPathsTypeDef):
     pass
 
+
 InvalidationSummaryTypeDef = TypedDict(
     "InvalidationSummaryTypeDef",
     {
         "Id": str,
         "CreateTime": datetime,
         "Status": str,
     },
@@ -1448,17 +1852,19 @@
     "_OptionalKeyPairIdsTypeDef",
     {
         "Items": List[str],
     },
     total=False,
 )
 
+
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
+
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1466,33 +1872,37 @@
     "_OptionalLambdaFunctionAssociationTypeDef",
     {
         "IncludeBody": bool,
     },
     total=False,
 )
 
+
 class LambdaFunctionAssociationTypeDef(
     _RequiredLambdaFunctionAssociationTypeDef, _OptionalLambdaFunctionAssociationTypeDef
 ):
     pass
 
+
 ListCachePoliciesRequestRequestTypeDef = TypedDict(
     "ListCachePoliciesRequestRequestTypeDef",
     {
         "Type": CachePolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
-    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
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
 
 ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     {
@@ -1514,20 +1924,22 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+
 class ListConflictingAliasesRequestRequestTypeDef(
     _RequiredListConflictingAliasesRequestRequestTypeDef,
     _OptionalListConflictingAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 ListContinuousDeploymentPoliciesRequestRequestTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1544,20 +1956,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByCachePolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByCachePolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByCachePolicyIdRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupId": str,
     },
 )
 _OptionalListDistributionsByKeyGroupRequestRequestTypeDef = TypedDict(
@@ -1565,20 +1979,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByKeyGroupRequestRequestTypeDef(
     _RequiredListDistributionsByKeyGroupRequestRequestTypeDef,
     _OptionalListDistributionsByKeyGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef",
     {
         "OriginRequestPolicyId": str,
     },
 )
 _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef = TypedDict(
@@ -1586,20 +2002,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
 ):
     pass
 
+
 ListDistributionsByRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "RealtimeLogConfigName": str,
         "RealtimeLogConfigArn": str,
@@ -1618,20 +2036,22 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef(
     _RequiredListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     _OptionalListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
     "_RequiredListDistributionsByWebACLIdRequestRequestTypeDef",
     {
         "WebACLId": str,
     },
 )
 _OptionalListDistributionsByWebACLIdRequestRequestTypeDef = TypedDict(
@@ -1639,27 +2059,21 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListDistributionsByWebACLIdRequestRequestTypeDef(
     _RequiredListDistributionsByWebACLIdRequestRequestTypeDef,
     _OptionalListDistributionsByWebACLIdRequestRequestTypeDef,
 ):
     pass
 
-ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
-    "ListDistributionsRequestListDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDistributionsRequestRequestTypeDef = TypedDict(
     "ListDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
@@ -1690,34 +2104,14 @@
         "Marker": str,
         "MaxItems": str,
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
-_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "DistributionId": str,
-    },
-)
-_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
-    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
-    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
-    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListInvalidationsRequestRequestTypeDef = TypedDict(
     "_RequiredListInvalidationsRequestRequestTypeDef",
     {
         "DistributionId": str,
     },
 )
 _OptionalListInvalidationsRequestRequestTypeDef = TypedDict(
@@ -1725,19 +2119,21 @@
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
+
 class ListInvalidationsRequestRequestTypeDef(
     _RequiredListInvalidationsRequestRequestTypeDef, _OptionalListInvalidationsRequestRequestTypeDef
 ):
     pass
 
+
 ListKeyGroupsRequestRequestTypeDef = TypedDict(
     "ListKeyGroupsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1786,22 +2182,14 @@
         "Type": ResponseHeadersPolicyTypeType,
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
-    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamingDistributionsRequestRequestTypeDef = TypedDict(
     "ListStreamingDistributionsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1829,19 +2217,27 @@
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
 
+StatusCodesOutputTypeDef = TypedDict(
+    "StatusCodesOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[int],
+    },
+)
+
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": List[int],
+        "Items": Sequence[int],
     },
 )
 
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
@@ -1858,34 +2254,26 @@
     "_OptionalOriginShieldTypeDef",
     {
         "OriginShieldRegion": str,
     },
     total=False,
 )
 
+
 class OriginShieldTypeDef(_RequiredOriginShieldTypeDef, _OptionalOriginShieldTypeDef):
     pass
 
+
 S3OriginConfigTypeDef = TypedDict(
     "S3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
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
 _RequiredPublicKeySummaryTypeDef = TypedDict(
     "_RequiredPublicKeySummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatedTime": datetime,
         "EncodedKey": str,
@@ -1895,17 +2283,19 @@
     "_OptionalPublicKeySummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class PublicKeySummaryTypeDef(_RequiredPublicKeySummaryTypeDef, _OptionalPublicKeySummaryTypeDef):
     pass
 
+
 PublishFunctionRequestRequestTypeDef = TypedDict(
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
@@ -1914,78 +2304,128 @@
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef(
+    _RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+    _OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
+
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "SamplingRate": float,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
+
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
@@ -2041,20 +2481,22 @@
     {
         "IncludeSubdomains": bool,
         "Preload": bool,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyStrictTransportSecurityTypeDef(
     _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef,
     _OptionalResponseHeadersPolicyStrictTransportSecurityTypeDef,
 ):
     pass
 
+
 _RequiredResponseHeadersPolicyXSSProtectionTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyXSSProtectionTypeDef",
     {
         "Override": bool,
         "Protection": bool,
     },
 )
@@ -2063,30 +2505,21 @@
     {
         "ModeBlock": bool,
         "ReportUri": str,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyXSSProtectionTypeDef(
     _RequiredResponseHeadersPolicyXSSProtectionTypeDef,
     _OptionalResponseHeadersPolicyXSSProtectionTypeDef,
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
 
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
@@ -2119,211 +2552,406 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
+_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    {
+        "StagingDistributionId": str,
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+
+class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
+    _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredAllowedMethodsOutputTypeDef = TypedDict(
+    "_RequiredAllowedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+_OptionalAllowedMethodsOutputTypeDef = TypedDict(
+    "_OptionalAllowedMethodsOutputTypeDef",
+    {
+        "CachedMethods": CachedMethodsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AllowedMethodsOutputTypeDef(
+    _RequiredAllowedMethodsOutputTypeDef, _OptionalAllowedMethodsOutputTypeDef
+):
+    pass
+
+
+_RequiredAllowedMethodsTypeDef = TypedDict(
+    "_RequiredAllowedMethodsTypeDef",
+    {
+        "Quantity": int,
+        "Items": Sequence[MethodType],
+    },
+)
+_OptionalAllowedMethodsTypeDef = TypedDict(
+    "_OptionalAllowedMethodsTypeDef",
+    {
+        "CachedMethods": CachedMethodsTypeDef,
+    },
+    total=False,
+)
+
+
+class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
+    pass
+
+
 _RequiredTestFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredTestFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
-        "EventObject": Union[str, bytes, IO[Any], StreamingBody],
+        "EventObject": BlobTypeDef,
     },
 )
 _OptionalTestFunctionRequestRequestTypeDef = TypedDict(
     "_OptionalTestFunctionRequestRequestTypeDef",
     {
         "Stage": FunctionStageType,
     },
     total=False,
 )
 
+
 class TestFunctionRequestRequestTypeDef(
     _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+
+_RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyCookiesConfigOutputTypeDef",
     {
-        "Id": str,
+        "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
-_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef",
+_OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyCookiesConfigOutputTypeDef",
     {
-        "StagingDistributionId": str,
-        "IfMatch": str,
+        "Cookies": CookieNamesOutputTypeDef,
     },
     total=False,
 )
 
-class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
-    _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
-    _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
+
+class CachePolicyCookiesConfigOutputTypeDef(
+    _RequiredCachePolicyCookiesConfigOutputTypeDef, _OptionalCachePolicyCookiesConfigOutputTypeDef
 ):
     pass
 
-_RequiredAllowedMethodsTypeDef = TypedDict(
-    "_RequiredAllowedMethodsTypeDef",
+
+_RequiredCookiePreferenceOutputTypeDef = TypedDict(
+    "_RequiredCookiePreferenceOutputTypeDef",
     {
-        "Quantity": int,
-        "Items": List[MethodType],
+        "Forward": ItemSelectionType,
     },
 )
-_OptionalAllowedMethodsTypeDef = TypedDict(
-    "_OptionalAllowedMethodsTypeDef",
+_OptionalCookiePreferenceOutputTypeDef = TypedDict(
+    "_OptionalCookiePreferenceOutputTypeDef",
     {
-        "CachedMethods": CachedMethodsTypeDef,
+        "WhitelistedNames": CookieNamesOutputTypeDef,
     },
     total=False,
 )
 
-class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
+
+class CookiePreferenceOutputTypeDef(
+    _RequiredCookiePreferenceOutputTypeDef, _OptionalCookiePreferenceOutputTypeDef
+):
     pass
 
+
+_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "Cookies": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyCookiesConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyCookiesConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyCookiesConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCachePolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
 _OptionalCachePolicyCookiesConfigTypeDef = TypedDict(
     "_OptionalCachePolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
+
 class CachePolicyCookiesConfigTypeDef(
     _RequiredCachePolicyCookiesConfigTypeDef, _OptionalCachePolicyCookiesConfigTypeDef
 ):
     pass
 
+
 _RequiredCookiePreferenceTypeDef = TypedDict(
     "_RequiredCookiePreferenceTypeDef",
     {
         "Forward": ItemSelectionType,
     },
 )
 _OptionalCookiePreferenceTypeDef = TypedDict(
     "_OptionalCookiePreferenceTypeDef",
     {
         "WhitelistedNames": CookieNamesTypeDef,
     },
     total=False,
 )
 
+
 class CookiePreferenceTypeDef(_RequiredCookiePreferenceTypeDef, _OptionalCookiePreferenceTypeDef):
     pass
 
+
 _RequiredOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyCookiesConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyCookiesConfigTypeDef",
     {
         "Cookies": CookieNamesTypeDef,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyCookiesConfigTypeDef(
     _RequiredOriginRequestPolicyCookiesConfigTypeDef,
     _OptionalOriginRequestPolicyCookiesConfigTypeDef,
 ):
     pass
 
+
+_RequiredCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": CachePolicyHeaderBehaviorType,
+    },
+)
+_OptionalCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyHeadersConfigOutputTypeDef(
+    _RequiredCachePolicyHeadersConfigOutputTypeDef, _OptionalCachePolicyHeadersConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyHeadersConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyHeadersConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCachePolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredCachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
     },
 )
 _OptionalCachePolicyHeadersConfigTypeDef = TypedDict(
     "_OptionalCachePolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
+
 class CachePolicyHeadersConfigTypeDef(
     _RequiredCachePolicyHeadersConfigTypeDef, _OptionalCachePolicyHeadersConfigTypeDef
 ):
     pass
 
+
 _RequiredOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyHeadersConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyHeadersConfigTypeDef",
     {
         "Headers": HeadersTypeDef,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyHeadersConfigTypeDef(
     _RequiredOriginRequestPolicyHeadersConfigTypeDef,
     _OptionalOriginRequestPolicyHeadersConfigTypeDef,
 ):
     pass
 
+
+_RequiredCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
+    },
+)
+_OptionalCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyQueryStringsConfigOutputTypeDef(
+    _RequiredCachePolicyQueryStringsConfigOutputTypeDef,
+    _OptionalCachePolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
+
+_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyQueryStringsConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
     },
 )
 _OptionalCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_OptionalCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
+
 class CachePolicyQueryStringsConfigTypeDef(
     _RequiredCachePolicyQueryStringsConfigTypeDef, _OptionalCachePolicyQueryStringsConfigTypeDef
 ):
     pass
 
+
 _RequiredOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
     },
 )
 _OptionalOriginRequestPolicyQueryStringsConfigTypeDef = TypedDict(
     "_OptionalOriginRequestPolicyQueryStringsConfigTypeDef",
     {
         "QueryStrings": QueryStringNamesTypeDef,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyQueryStringsConfigTypeDef(
     _RequiredOriginRequestPolicyQueryStringsConfigTypeDef,
     _OptionalOriginRequestPolicyQueryStringsConfigTypeDef,
 ):
     pass
 
+
 _RequiredCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityTypeDef",
     {
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
@@ -2331,35 +2959,28 @@
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
     total=False,
 )
 
+
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
+
 CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
     },
 )
 
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
-    {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
         "Id": str,
     },
 )
@@ -2367,20 +2988,22 @@
     "_OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef(
     _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     _OptionalUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCloudFrontOriginAccessIdentityListTypeDef = TypedDict(
     "_RequiredCloudFrontOriginAccessIdentityListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -2391,114 +3014,149 @@
     {
         "NextMarker": str,
         "Items": List[CloudFrontOriginAccessIdentitySummaryTypeDef],
     },
     total=False,
 )
 
+
 class CloudFrontOriginAccessIdentityListTypeDef(
     _RequiredCloudFrontOriginAccessIdentityListTypeDef,
     _OptionalCloudFrontOriginAccessIdentityListTypeDef,
 ):
     pass
 
+
 ConflictingAliasesListTypeDef = TypedDict(
     "ConflictingAliasesListTypeDef",
     {
         "NextMarker": str,
         "MaxItems": int,
         "Quantity": int,
         "Items": List[ConflictingAliasTypeDef],
     },
     total=False,
 )
 
+_RequiredContentTypeProfilesOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalContentTypeProfilesOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfilesOutputTypeDef",
+    {
+        "Items": List[ContentTypeProfileTypeDef],
+    },
+    total=False,
+)
+
+
+class ContentTypeProfilesOutputTypeDef(
+    _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
+):
+    pass
+
+
 _RequiredContentTypeProfilesTypeDef = TypedDict(
     "_RequiredContentTypeProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesTypeDef = TypedDict(
     "_OptionalContentTypeProfilesTypeDef",
     {
         "Items": Sequence[ContentTypeProfileTypeDef],
     },
     total=False,
 )
 
+
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
+
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_OptionalContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "SessionStickinessConfig": SessionStickinessConfigTypeDef,
     },
     total=False,
 )
 
+
 class ContinuousDeploymentSingleWeightConfigTypeDef(
     _RequiredContinuousDeploymentSingleWeightConfigTypeDef,
     _OptionalContinuousDeploymentSingleWeightConfigTypeDef,
 ):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    {
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionResultTypeDef = TypedDict(
+    "GetFunctionResultTypeDef",
+    {
+        "FunctionCode": StreamingBody,
+        "ETag": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 UpdateFunctionRequestRequestTypeDef = TypedDict(
     "UpdateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
 
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-    },
-)
-
 _RequiredUpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
     },
 )
@@ -2506,32 +3164,34 @@
     "_OptionalUpdateKeyGroupRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateKeyGroupRequestRequestTypeDef(
     _RequiredUpdateKeyGroupRequestRequestTypeDef, _OptionalUpdateKeyGroupRequestRequestTypeDef
 ):
     pass
 
+
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
 GetOriginAccessControlConfigResultTypeDef = TypedDict(
     "GetOriginAccessControlConfigResultTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOriginAccessControlTypeDef = TypedDict(
     "_RequiredOriginAccessControlTypeDef",
     {
         "Id": str,
@@ -2541,19 +3201,21 @@
     "_OptionalOriginAccessControlTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
     total=False,
 )
 
+
 class OriginAccessControlTypeDef(
     _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
 ):
     pass
 
+
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -2561,33 +3223,35 @@
     "_OptionalUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateOriginAccessControlRequestRequestTypeDef(
     _RequiredUpdateOriginAccessControlRequestRequestTypeDef,
     _OptionalUpdateOriginAccessControlRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
 GetPublicKeyConfigResultTypeDef = TypedDict(
     "GetPublicKeyConfigResultTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Id": str,
@@ -2607,55 +3271,128 @@
     "_OptionalUpdatePublicKeyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdatePublicKeyRequestRequestTypeDef(
     _RequiredUpdatePublicKeyRequestRequestTypeDef, _OptionalUpdatePublicKeyRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_RequiredCustomErrorResponsesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_OptionalCustomErrorResponsesOutputTypeDef",
+    {
+        "Items": List[CustomErrorResponseTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomErrorResponsesOutputTypeDef(
+    _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomErrorResponsesTypeDef = TypedDict(
     "_RequiredCustomErrorResponsesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesTypeDef",
     {
-        "Items": List[CustomErrorResponseTypeDef],
+        "Items": Sequence[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
+
 class CustomErrorResponsesTypeDef(
     _RequiredCustomErrorResponsesTypeDef, _OptionalCustomErrorResponsesTypeDef
 ):
     pass
 
+
+_RequiredCustomHeadersOutputTypeDef = TypedDict(
+    "_RequiredCustomHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomHeadersOutputTypeDef = TypedDict(
+    "_OptionalCustomHeadersOutputTypeDef",
+    {
+        "Items": List[OriginCustomHeaderTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomHeadersOutputTypeDef(
+    _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomHeadersTypeDef = TypedDict(
     "_RequiredCustomHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersTypeDef = TypedDict(
     "_OptionalCustomHeadersTypeDef",
     {
-        "Items": List[OriginCustomHeaderTypeDef],
+        "Items": Sequence[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
+
 class CustomHeadersTypeDef(_RequiredCustomHeadersTypeDef, _OptionalCustomHeadersTypeDef):
     pass
 
+
+_RequiredCustomOriginConfigOutputTypeDef = TypedDict(
+    "_RequiredCustomOriginConfigOutputTypeDef",
+    {
+        "HTTPPort": int,
+        "HTTPSPort": int,
+        "OriginProtocolPolicy": OriginProtocolPolicyType,
+    },
+)
+_OptionalCustomOriginConfigOutputTypeDef = TypedDict(
+    "_OptionalCustomOriginConfigOutputTypeDef",
+    {
+        "OriginSslProtocols": OriginSslProtocolsOutputTypeDef,
+        "OriginReadTimeout": int,
+        "OriginKeepaliveTimeout": int,
+    },
+    total=False,
+)
+
+
+class CustomOriginConfigOutputTypeDef(
+    _RequiredCustomOriginConfigOutputTypeDef, _OptionalCustomOriginConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomOriginConfigTypeDef = TypedDict(
     "_RequiredCustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
         "OriginProtocolPolicy": OriginProtocolPolicyType,
     },
@@ -2666,48 +3403,59 @@
         "OriginSslProtocols": OriginSslProtocolsTypeDef,
         "OriginReadTimeout": int,
         "OriginKeepaliveTimeout": int,
     },
     total=False,
 )
 
+
 class CustomOriginConfigTypeDef(
     _RequiredCustomOriginConfigTypeDef, _OptionalCustomOriginConfigTypeDef
 ):
     pass
 
+
 ListDistributionsByCachePolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByCachePolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByKeyGroupResultTypeDef = TypedDict(
     "ListDistributionsByKeyGroupResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByOriginRequestPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByResponseHeadersPolicyIdResultTypeDef = TypedDict(
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EncryptionEntityOutputTypeDef = TypedDict(
+    "EncryptionEntityOutputTypeDef",
+    {
+        "PublicKeyId": str,
+        "ProviderId": str,
+        "FieldPatterns": FieldPatternsOutputTypeDef,
     },
 )
 
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
@@ -2726,36 +3474,61 @@
     "_OptionalEndPointTypeDef",
     {
         "KinesisStreamConfig": KinesisStreamConfigTypeDef,
     },
     total=False,
 )
 
+
 class EndPointTypeDef(_RequiredEndPointTypeDef, _OptionalEndPointTypeDef):
     pass
 
+
+_RequiredFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[FunctionAssociationTypeDef],
+    },
+    total=False,
+)
+
+
+class FunctionAssociationsOutputTypeDef(
+    _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
+):
+    pass
+
+
 _RequiredFunctionAssociationsTypeDef = TypedDict(
     "_RequiredFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsTypeDef = TypedDict(
     "_OptionalFunctionAssociationsTypeDef",
     {
-        "Items": List[FunctionAssociationTypeDef],
+        "Items": Sequence[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
+
 class FunctionAssociationsTypeDef(
     _RequiredFunctionAssociationsTypeDef, _OptionalFunctionAssociationsTypeDef
 ):
     pass
 
+
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
@@ -2764,17 +3537,26 @@
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
+
 class FunctionSummaryTypeDef(_RequiredFunctionSummaryTypeDef, _OptionalFunctionSummaryTypeDef):
     pass
 
+
+RestrictionsOutputTypeDef = TypedDict(
+    "RestrictionsOutputTypeDef",
+    {
+        "GeoRestriction": GeoRestrictionOutputTypeDef,
+    },
+)
+
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
 )
 
@@ -2788,20 +3570,22 @@
     "_OptionalGetDistributionRequestDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetDistributionRequestDistributionDeployedWaitTypeDef(
     _RequiredGetDistributionRequestDistributionDeployedWaitTypeDef,
     _OptionalGetDistributionRequestDistributionDeployedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef = TypedDict(
     "_RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "DistributionId": str,
         "Id": str,
     },
 )
@@ -2809,40 +3593,71 @@
     "_OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetInvalidationRequestInvalidationCompletedWaitTypeDef(
     _RequiredGetInvalidationRequestInvalidationCompletedWaitTypeDef,
     _OptionalGetInvalidationRequestInvalidationCompletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef = TypedDict(
     "_OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(
     _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
 ):
     pass
 
+
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+    },
+)
+
+InvalidationBatchOutputTypeDef = TypedDict(
+    "InvalidationBatchOutputTypeDef",
+    {
+        "Paths": PathsOutputTypeDef,
+        "CallerReference": str,
+    },
+)
+
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
 )
@@ -2861,17 +3676,19 @@
     {
         "NextMarker": str,
         "Items": List[InvalidationSummaryTypeDef],
     },
     total=False,
 )
 
+
 class InvalidationListTypeDef(_RequiredInvalidationListTypeDef, _OptionalInvalidationListTypeDef):
     pass
 
+
 KGKeyPairIdsTypeDef = TypedDict(
     "KGKeyPairIdsTypeDef",
     {
         "KeyGroupId": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
@@ -2882,33 +3699,103 @@
     {
         "AwsAccountNumber": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
 )
 
+_RequiredLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[LambdaFunctionAssociationTypeDef],
+    },
+    total=False,
+)
+
+
+class LambdaFunctionAssociationsOutputTypeDef(
+    _RequiredLambdaFunctionAssociationsOutputTypeDef,
+    _OptionalLambdaFunctionAssociationsOutputTypeDef,
+):
+    pass
+
+
 _RequiredLambdaFunctionAssociationsTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsTypeDef",
     {
-        "Items": List[LambdaFunctionAssociationTypeDef],
+        "Items": Sequence[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
+
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
+
+ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef = TypedDict(
+    "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDistributionsRequestListDistributionsPaginateTypeDef = TypedDict(
+    "ListDistributionsRequestListDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "DistributionId": str,
+    },
+)
+_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef = TypedDict(
+    "_OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInvalidationsRequestListInvalidationsPaginateTypeDef(
+    _RequiredListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    _OptionalListInvalidationsRequestListInvalidationsPaginateTypeDef,
+):
+    pass
+
+
+ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef = TypedDict(
+    "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
         "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigTypeDef,
     },
     total=False,
 )
@@ -2927,31 +3814,48 @@
     {
         "NextMarker": str,
         "Items": List[OriginAccessControlSummaryTypeDef],
     },
     total=False,
 )
 
+
 class OriginAccessControlListTypeDef(
     _RequiredOriginAccessControlListTypeDef, _OptionalOriginAccessControlListTypeDef
 ):
     pass
 
+
+OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
+    "OriginGroupFailoverCriteriaOutputTypeDef",
+    {
+        "StatusCodes": StatusCodesOutputTypeDef,
+    },
+)
+
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
 
+OriginGroupMembersOutputTypeDef = TypedDict(
+    "OriginGroupMembersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[OriginGroupMemberTypeDef],
+    },
+)
+
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
+        "Items": Sequence[OriginGroupMemberTypeDef],
     },
 )
 
 _RequiredPublicKeyListTypeDef = TypedDict(
     "_RequiredPublicKeyListTypeDef",
     {
         "MaxItems": int,
@@ -2963,34 +3867,86 @@
     {
         "NextMarker": str,
         "Items": List[PublicKeySummaryTypeDef],
     },
     total=False,
 )
 
+
 class PublicKeyListTypeDef(_RequiredPublicKeyListTypeDef, _OptionalPublicKeyListTypeDef):
     pass
 
+
+_RequiredQueryArgProfilesOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryArgProfilesOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfilesOutputTypeDef",
+    {
+        "Items": List[QueryArgProfileTypeDef],
+    },
+    total=False,
+)
+
+
+class QueryArgProfilesOutputTypeDef(
+    _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryArgProfilesTypeDef = TypedDict(
     "_RequiredQueryArgProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryArgProfilesTypeDef = TypedDict(
     "_OptionalQueryArgProfilesTypeDef",
     {
         "Items": Sequence[QueryArgProfileTypeDef],
     },
     total=False,
 )
 
+
 class QueryArgProfilesTypeDef(_RequiredQueryArgProfilesTypeDef, _OptionalQueryArgProfilesTypeDef):
     pass
 
+
+_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
+        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
+        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
+        "AccessControlAllowCredentials": bool,
+        "OriginOverride": bool,
+    },
+)
+_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+        "AccessControlMaxAgeSec": int,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyCorsConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCorsConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCorsConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
         "AccessControlAllowCredentials": bool,
@@ -3002,59 +3958,109 @@
     {
         "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
         "AccessControlMaxAgeSec": int,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyCorsConfigTypeDef(
     _RequiredResponseHeadersPolicyCorsConfigTypeDef, _OptionalResponseHeadersPolicyCorsConfigTypeDef
 ):
     pass
 
+
+_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyCustomHeaderTypeDef],
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyCustomHeaderTypeDef],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyCustomHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef,
 ):
     pass
 
+
+_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyRemoveHeaderTypeDef],
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Items": Sequence[ResponseHeadersPolicyRemoveHeaderTypeDef],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
+
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -3069,22 +4075,50 @@
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
         "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesTypeDef,
-        "TrustedSigners": TrustedSignersTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
+_RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredStreamingDistributionConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "S3Origin": S3OriginTypeDef,
+        "Comment": str,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalStreamingDistributionConfigOutputTypeDef",
+    {
+        "Aliases": AliasesOutputTypeDef,
+        "Logging": StreamingLoggingConfigTypeDef,
+        "PriceClass": PriceClassType,
+    },
+    total=False,
+)
+
+
+class StreamingDistributionConfigOutputTypeDef(
+    _RequiredStreamingDistributionConfigOutputTypeDef,
+    _OptionalStreamingDistributionConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredStreamingDistributionConfigTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -3097,35 +4131,68 @@
         "Aliases": AliasesTypeDef,
         "Logging": StreamingLoggingConfigTypeDef,
         "PriceClass": PriceClassType,
     },
     total=False,
 )
 
+
 class StreamingDistributionConfigTypeDef(
     _RequiredStreamingDistributionConfigTypeDef, _OptionalStreamingDistributionConfigTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
 
+TagsOutputTypeDef = TypedDict(
+    "TagsOutputTypeDef",
+    {
+        "Items": List[TagTypeDef],
+    },
+    total=False,
+)
+
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredForwardedValuesOutputTypeDef = TypedDict(
+    "_RequiredForwardedValuesOutputTypeDef",
+    {
+        "QueryString": bool,
+        "Cookies": CookiePreferenceOutputTypeDef,
+    },
+)
+_OptionalForwardedValuesOutputTypeDef = TypedDict(
+    "_OptionalForwardedValuesOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+        "QueryStringCacheKeys": QueryStringCacheKeysOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ForwardedValuesOutputTypeDef(
+    _RequiredForwardedValuesOutputTypeDef, _OptionalForwardedValuesOutputTypeDef
+):
+    pass
+
+
 _RequiredForwardedValuesTypeDef = TypedDict(
     "_RequiredForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
     },
 )
@@ -3134,17 +4201,68 @@
     {
         "Headers": HeadersTypeDef,
         "QueryStringCacheKeys": QueryStringCacheKeysTypeDef,
     },
     total=False,
 )
 
+
 class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
     pass
 
+
+_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingGzip": bool,
+        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingBrotli": bool,
+    },
+    total=False,
+)
+
+
+class ParametersInCacheKeyAndForwardedToOriginOutputTypeDef(
+    _RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    _OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+):
+    pass
+
+
+_RequiredOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyConfigOutputTypeDef, _OptionalOriginRequestPolicyConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "_RequiredParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
         "QueryStringsConfig": CachePolicyQueryStringsConfigTypeDef,
@@ -3154,20 +4272,22 @@
     "_OptionalParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingBrotli": bool,
     },
     total=False,
 )
 
+
 class ParametersInCacheKeyAndForwardedToOriginTypeDef(
     _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef,
     _OptionalParametersInCacheKeyAndForwardedToOriginTypeDef,
 ):
     pass
 
+
 _RequiredOriginRequestPolicyConfigTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyConfigTypeDef",
     {
         "Name": str,
         "HeadersConfig": OriginRequestPolicyHeadersConfigTypeDef,
         "CookiesConfig": OriginRequestPolicyCookiesConfigTypeDef,
         "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigTypeDef,
@@ -3177,82 +4297,107 @@
     "_OptionalOriginRequestPolicyConfigTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class OriginRequestPolicyConfigTypeDef(
     _RequiredOriginRequestPolicyConfigTypeDef, _OptionalOriginRequestPolicyConfigTypeDef
 ):
     pass
 
+
 CreateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCloudFrontOriginAccessIdentityResultTypeDef = TypedDict(
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     {
         "CloudFrontOriginAccessIdentity": CloudFrontOriginAccessIdentityTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCloudFrontOriginAccessIdentitiesResultTypeDef = TypedDict(
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     {
         "CloudFrontOriginAccessIdentityList": CloudFrontOriginAccessIdentityListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConflictingAliasesResultTypeDef = TypedDict(
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenContentTypeIsUnknown": bool,
+    },
+)
+_OptionalContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfileConfigOutputTypeDef",
+    {
+        "ContentTypeProfiles": ContentTypeProfilesOutputTypeDef,
     },
+    total=False,
 )
 
+
+class ContentTypeProfileConfigOutputTypeDef(
+    _RequiredContentTypeProfileConfigOutputTypeDef, _OptionalContentTypeProfileConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
 _OptionalContentTypeProfileConfigTypeDef = TypedDict(
     "_OptionalContentTypeProfileConfigTypeDef",
     {
         "ContentTypeProfiles": ContentTypeProfilesTypeDef,
     },
     total=False,
 )
 
+
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
+
 _RequiredTrafficConfigTypeDef = TypedDict(
     "_RequiredTrafficConfigTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
 _OptionalTrafficConfigTypeDef = TypedDict(
@@ -3260,108 +4405,102 @@
     {
         "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
         "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
     total=False,
 )
 
+
 class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
     pass
 
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
-
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateOriginAccessControlResultTypeDef = TypedDict(
     "CreateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginAccessControlResultTypeDef = TypedDict(
     "GetOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOriginAccessControlResultTypeDef = TypedDict(
     "UpdateOriginAccessControlResultTypeDef",
     {
         "OriginAccessControl": OriginAccessControlTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePublicKeyResultTypeDef = TypedDict(
     "CreatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPublicKeyResultTypeDef = TypedDict(
     "GetPublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePublicKeyResultTypeDef = TypedDict(
     "UpdatePublicKeyResultTypeDef",
     {
         "PublicKey": PublicKeyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredOriginOutputTypeDef = TypedDict(
+    "_RequiredOriginOutputTypeDef",
+    {
+        "Id": str,
+        "DomainName": str,
+    },
+)
+_OptionalOriginOutputTypeDef = TypedDict(
+    "_OptionalOriginOutputTypeDef",
+    {
+        "OriginPath": str,
+        "CustomHeaders": CustomHeadersOutputTypeDef,
+        "S3OriginConfig": S3OriginConfigTypeDef,
+        "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
+        "ConnectionAttempts": int,
+        "ConnectionTimeout": int,
+        "OriginShield": OriginShieldTypeDef,
+        "OriginAccessControlId": str,
+    },
+    total=False,
+)
+
+
+class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
+    pass
+
+
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
 )
@@ -3376,36 +4515,61 @@
         "ConnectionTimeout": int,
         "OriginShield": OriginShieldTypeDef,
         "OriginAccessControlId": str,
     },
     total=False,
 )
 
+
 class OriginTypeDef(_RequiredOriginTypeDef, _OptionalOriginTypeDef):
     pass
 
+
+_RequiredEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_RequiredEncryptionEntitiesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_OptionalEncryptionEntitiesOutputTypeDef",
+    {
+        "Items": List[EncryptionEntityOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class EncryptionEntitiesOutputTypeDef(
+    _RequiredEncryptionEntitiesOutputTypeDef, _OptionalEncryptionEntitiesOutputTypeDef
+):
+    pass
+
+
 _RequiredEncryptionEntitiesTypeDef = TypedDict(
     "_RequiredEncryptionEntitiesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalEncryptionEntitiesTypeDef = TypedDict(
     "_OptionalEncryptionEntitiesTypeDef",
     {
         "Items": Sequence[EncryptionEntityTypeDef],
     },
     total=False,
 )
 
+
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
+
 CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
         "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
@@ -3437,24 +4601,24 @@
 
 CreateFunctionResultTypeDef = TypedDict(
     "CreateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFunctionResultTypeDef = TypedDict(
     "DescribeFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionListTypeDef = TypedDict(
     "_RequiredFunctionListTypeDef",
     {
         "MaxItems": int,
@@ -3466,22 +4630,24 @@
     {
         "NextMarker": str,
         "Items": List[FunctionSummaryTypeDef],
     },
     total=False,
 )
 
+
 class FunctionListTypeDef(_RequiredFunctionListTypeDef, _OptionalFunctionListTypeDef):
     pass
 
+
 PublishFunctionResultTypeDef = TypedDict(
     "PublishFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestResultTypeDef = TypedDict(
     "TestResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
@@ -3494,41 +4660,77 @@
 )
 
 UpdateFunctionResultTypeDef = TypedDict(
     "UpdateFunctionResultTypeDef",
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
     {
-        "DistributionId": str,
-        "InvalidationBatch": InvalidationBatchTypeDef,
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
+        "InvalidationBatch": InvalidationBatchOutputTypeDef,
+    },
+)
+
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
+    {
+        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
+InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredActiveTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredActiveTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
@@ -3539,19 +4741,21 @@
     "_OptionalActiveTrustedKeyGroupsTypeDef",
     {
         "Items": List[KGKeyPairIdsTypeDef],
     },
     total=False,
 )
 
+
 class ActiveTrustedKeyGroupsTypeDef(
     _RequiredActiveTrustedKeyGroupsTypeDef, _OptionalActiveTrustedKeyGroupsTypeDef
 ):
     pass
 
+
 _RequiredActiveTrustedSignersTypeDef = TypedDict(
     "_RequiredActiveTrustedSignersTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
@@ -3559,48 +4763,59 @@
     "_OptionalActiveTrustedSignersTypeDef",
     {
         "Items": List[SignerTypeDef],
     },
     total=False,
 )
 
+
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
+
 CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     {
         "DistributionId": str,
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
     },
 )
 
 CreateMonitoringSubscriptionResultTypeDef = TypedDict(
     "CreateMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMonitoringSubscriptionResultTypeDef = TypedDict(
     "GetMonitoringSubscriptionResultTypeDef",
     {
         "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OriginGroupOutputTypeDef = TypedDict(
+    "OriginGroupOutputTypeDef",
+    {
+        "Id": str,
+        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
+        "Members": OriginGroupMembersOutputTypeDef,
     },
 )
 
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
@@ -3609,17 +4824,38 @@
     },
 )
 
 ListPublicKeysResultTypeDef = TypedDict(
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
+_OptionalQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfileConfigOutputTypeDef",
+    {
+        "QueryArgProfiles": QueryArgProfilesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryArgProfileConfigOutputTypeDef(
+    _RequiredQueryArgProfileConfigOutputTypeDef, _OptionalQueryArgProfileConfigOutputTypeDef
+):
+    pass
+
 
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
@@ -3627,19 +4863,48 @@
     "_OptionalQueryArgProfileConfigTypeDef",
     {
         "QueryArgProfiles": QueryArgProfilesTypeDef,
     },
     total=False,
 )
 
+
 class QueryArgProfileConfigTypeDef(
     _RequiredQueryArgProfileConfigTypeDef, _OptionalQueryArgProfileConfigTypeDef
 ):
     pass
 
+
+_RequiredResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
+        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigTypeDef,
+        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
+        "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+        "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalResponseHeadersPolicyConfigTypeDef = TypedDict(
@@ -3651,19 +4916,21 @@
         "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
         "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigTypeDef,
         "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyConfigTypeDef(
     _RequiredResponseHeadersPolicyConfigTypeDef, _OptionalResponseHeadersPolicyConfigTypeDef
 ):
     pass
 
+
 _RequiredStreamingDistributionListTypeDef = TypedDict(
     "_RequiredStreamingDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -3674,35 +4941,40 @@
     {
         "NextMarker": str,
         "Items": List[StreamingDistributionSummaryTypeDef],
     },
     total=False,
 )
 
+
 class StreamingDistributionListTypeDef(
     _RequiredStreamingDistributionListTypeDef, _OptionalStreamingDistributionListTypeDef
 ):
     pass
 
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StreamingDistributionConfigUnionTypeDef = Union[
+    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+]
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -3710,25 +4982,27 @@
     "_OptionalUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateStreamingDistributionRequestRequestTypeDef(
     _RequiredUpdateStreamingDistributionRequestRequestTypeDef,
     _OptionalUpdateStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": TagsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3740,14 +5014,90 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
+TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
+_RequiredCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorOutputTypeDef",
+    {
+        "PathPattern": str,
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+
+class CacheBehaviorOutputTypeDef(
+    _RequiredCacheBehaviorOutputTypeDef, _OptionalCacheBehaviorOutputTypeDef
+):
+    pass
+
+
+_RequiredDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+
+class DefaultCacheBehaviorOutputTypeDef(
+    _RequiredDefaultCacheBehaviorOutputTypeDef, _OptionalDefaultCacheBehaviorOutputTypeDef
+):
+    pass
+
+
 _RequiredCacheBehaviorTypeDef = TypedDict(
     "_RequiredCacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -3771,17 +5121,19 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
+
 class CacheBehaviorTypeDef(_RequiredCacheBehaviorTypeDef, _OptionalCacheBehaviorTypeDef):
     pass
 
+
 _RequiredDefaultCacheBehaviorTypeDef = TypedDict(
     "_RequiredDefaultCacheBehaviorTypeDef",
     {
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
 )
@@ -3804,67 +5156,101 @@
         "MinTTL": int,
         "DefaultTTL": int,
         "MaxTTL": int,
     },
     total=False,
 )
 
+
 class DefaultCacheBehaviorTypeDef(
     _RequiredDefaultCacheBehaviorTypeDef, _OptionalDefaultCacheBehaviorTypeDef
 ):
     pass
 
-_RequiredCachePolicyConfigTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigTypeDef",
+
+_RequiredCachePolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigOutputTypeDef",
     {
         "Name": str,
         "MinTTL": int,
     },
 )
-_OptionalCachePolicyConfigTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigTypeDef",
+_OptionalCachePolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigOutputTypeDef",
     {
         "Comment": str,
         "DefaultTTL": int,
         "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+        "ParametersInCacheKeyAndForwardedToOrigin": (
+            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
+        ),
     },
     total=False,
 )
 
-class CachePolicyConfigTypeDef(
-    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+
+class CachePolicyConfigOutputTypeDef(
+    _RequiredCachePolicyConfigOutputTypeDef, _OptionalCachePolicyConfigOutputTypeDef
 ):
     pass
 
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
-    },
-)
 
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+    },
+)
+
+_RequiredCachePolicyConfigTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigTypeDef",
+    {
+        "Name": str,
+        "MinTTL": int,
+    },
+)
+_OptionalCachePolicyConfigTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigTypeDef",
+    {
+        "Comment": str,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyConfigTypeDef(
+    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+):
+    pass
+
+
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
+OriginRequestPolicyConfigUnionTypeDef = Union[
+    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+]
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -3872,20 +5258,45 @@
     "_OptionalUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateOriginRequestPolicyRequestRequestTypeDef(
     _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef,
     _OptionalUpdateOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "TrafficConfig": TrafficConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ContinuousDeploymentPolicyConfigOutputTypeDef(
+    _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
+    _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
     },
 )
@@ -3893,105 +5304,124 @@
     "_OptionalContinuousDeploymentPolicyConfigTypeDef",
     {
         "TrafficConfig": TrafficConfigTypeDef,
     },
     total=False,
 )
 
+
 class ContinuousDeploymentPolicyConfigTypeDef(
     _RequiredContinuousDeploymentPolicyConfigTypeDef,
     _OptionalContinuousDeploymentPolicyConfigTypeDef,
 ):
     pass
 
-_RequiredKeyGroupListTypeDef = TypedDict(
-    "_RequiredKeyGroupListTypeDef",
+
+OriginsOutputTypeDef = TypedDict(
+    "OriginsOutputTypeDef",
     {
-        "MaxItems": int,
         "Quantity": int,
+        "Items": List[OriginOutputTypeDef],
     },
 )
-_OptionalKeyGroupListTypeDef = TypedDict(
-    "_OptionalKeyGroupListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[KeyGroupSummaryTypeDef],
-    },
-    total=False,
-)
-
-class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
-    pass
 
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginTypeDef],
+        "Items": Sequence[OriginTypeDef],
     },
 )
 
-_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-class FieldLevelEncryptionProfileConfigTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+
+class FieldLevelEncryptionProfileConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigOutputTypeDef,
 ):
     pass
 
+
 _RequiredFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
 _OptionalFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
+
 class FieldLevelEncryptionProfileSummaryTypeDef(
     _RequiredFieldLevelEncryptionProfileSummaryTypeDef,
     _OptionalFieldLevelEncryptionProfileSummaryTypeDef,
 ):
     pass
 
+
+_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Name": str,
+        "CallerReference": str,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
+    },
+)
+_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class FieldLevelEncryptionProfileConfigTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+):
+    pass
+
+
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRealtimeLogConfigResultTypeDef = TypedDict(
     "GetRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRealtimeLogConfigsTypeDef = TypedDict(
     "_RequiredRealtimeLogConfigsTypeDef",
     {
         "MaxItems": int,
@@ -4004,169 +5434,248 @@
     {
         "Items": List[RealtimeLogConfigTypeDef],
         "NextMarker": str,
     },
     total=False,
 )
 
+
 class RealtimeLogConfigsTypeDef(
     _RequiredRealtimeLogConfigsTypeDef, _OptionalRealtimeLogConfigsTypeDef
 ):
     pass
 
+
 UpdateRealtimeLogConfigResultTypeDef = TypedDict(
     "UpdateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResultTypeDef = TypedDict(
     "ListFunctionsResultTypeDef",
     {
         "FunctionList": FunctionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFunctionResultTypeDef = TypedDict(
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredKeyGroupListTypeDef = TypedDict(
+    "_RequiredKeyGroupListTypeDef",
+    {
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
+_OptionalKeyGroupListTypeDef = TypedDict(
+    "_OptionalKeyGroupListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[KeyGroupSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
+    pass
+
 
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvalidationResultTypeDef = TypedDict(
     "GetInvalidationResultTypeDef",
     {
         "Invalidation": InvalidationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStreamingDistributionTypeDef = TypedDict(
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
     },
 )
 _OptionalStreamingDistributionTypeDef = TypedDict(
     "_OptionalStreamingDistributionTypeDef",
     {
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
+
 class StreamingDistributionTypeDef(
     _RequiredStreamingDistributionTypeDef, _OptionalStreamingDistributionTypeDef
 ):
     pass
 
+
+_RequiredOriginGroupsOutputTypeDef = TypedDict(
+    "_RequiredOriginGroupsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalOriginGroupsOutputTypeDef = TypedDict(
+    "_OptionalOriginGroupsOutputTypeDef",
+    {
+        "Items": List[OriginGroupOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class OriginGroupsOutputTypeDef(
+    _RequiredOriginGroupsOutputTypeDef, _OptionalOriginGroupsOutputTypeDef
+):
+    pass
+
+
 _RequiredOriginGroupsTypeDef = TypedDict(
     "_RequiredOriginGroupsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalOriginGroupsTypeDef = TypedDict(
     "_OptionalOriginGroupsTypeDef",
     {
-        "Items": List[OriginGroupTypeDef],
+        "Items": Sequence[OriginGroupTypeDef],
     },
     total=False,
 )
 
+
 class OriginGroupsTypeDef(_RequiredOriginGroupsTypeDef, _OptionalOriginGroupsTypeDef):
     pass
 
-_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigTypeDef",
+
+_RequiredFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigOutputTypeDef",
     {
         "CallerReference": str,
     },
 )
-_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigTypeDef",
+_OptionalFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigOutputTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
-class FieldLevelEncryptionConfigTypeDef(
-    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+
+class FieldLevelEncryptionConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionConfigOutputTypeDef,
 ):
     pass
 
+
 _RequiredFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
     },
 )
 _OptionalFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionSummaryTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
+
 class FieldLevelEncryptionSummaryTypeDef(
     _RequiredFieldLevelEncryptionSummaryTypeDef, _OptionalFieldLevelEncryptionSummaryTypeDef
 ):
     pass
 
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+
+_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "CallerReference": str,
+    },
+)
+_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigTypeDef",
+    {
+        "Comment": str,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
     },
+    total=False,
 )
 
+
+class FieldLevelEncryptionConfigTypeDef(
+    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+):
+    pass
+
+
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+    },
+)
+
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
+ResponseHeadersPolicyConfigUnionTypeDef = Union[
+    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+]
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -4174,113 +5683,111 @@
     "_OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateResponseHeadersPolicyRequestRequestTypeDef(
     _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef,
     _OptionalUpdateResponseHeadersPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 ListStreamingDistributionsResultTypeDef = TypedDict(
     "ListStreamingDistributionsResultTypeDef",
     {
         "StreamingDistributionList": StreamingDistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
 
+_RequiredCacheBehaviorsOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCacheBehaviorsOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorsOutputTypeDef",
+    {
+        "Items": List[CacheBehaviorOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CacheBehaviorsOutputTypeDef(
+    _RequiredCacheBehaviorsOutputTypeDef, _OptionalCacheBehaviorsOutputTypeDef
+):
+    pass
+
+
 _RequiredCacheBehaviorsTypeDef = TypedDict(
     "_RequiredCacheBehaviorsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCacheBehaviorsTypeDef = TypedDict(
     "_OptionalCacheBehaviorsTypeDef",
     {
-        "Items": List[CacheBehaviorTypeDef],
+        "Items": Sequence[CacheBehaviorTypeDef],
     },
     total=False,
 )
 
+
 class CacheBehaviorsTypeDef(_RequiredCacheBehaviorsTypeDef, _OptionalCacheBehaviorsTypeDef):
     pass
 
+
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
     },
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "IfMatch": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateCachePolicyRequestRequestTypeDef(
-    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
-):
-    pass
-
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOriginRequestPolicyResultTypeDef = TypedDict(
     "GetOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OriginRequestPolicySummaryTypeDef = TypedDict(
     "OriginRequestPolicySummaryTypeDef",
     {
         "Type": OriginRequestPolicyTypeType,
@@ -4289,40 +5796,73 @@
 )
 
 UpdateOriginRequestPolicyResultTypeDef = TypedDict(
     "UpdateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 
+_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+
+class UpdateCachePolicyRequestRequestTypeDef(
+    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
+):
+    pass
+
+
 ContinuousDeploymentPolicyTypeDef = TypedDict(
     "ContinuousDeploymentPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
     },
 )
 
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
+    "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
-    "GetContinuousDeploymentPolicyConfigResultTypeDef",
+ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
+    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+]
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
@@ -4333,53 +5873,73 @@
     "_OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
+
+FieldLevelEncryptionProfileTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileTypeDef",
     {
-        "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
     },
 )
 
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
+    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FieldLevelEncryptionProfileTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileTypeDef",
+_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
+_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+    },
+    total=False,
+)
 
-GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
-    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
+
+class FieldLevelEncryptionProfileListTypeDef(
+    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
+):
+    pass
+
+
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
+    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+]
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "Id": str,
     },
 )
@@ -4387,170 +5947,166 @@
     "_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-    },
-)
-_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
-    },
-    total=False,
-)
-
-class FieldLevelEncryptionProfileListTypeDef(
-    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
-):
-    pass
 
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
+    {
+        "KeyGroupList": KeyGroupListTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStreamingDistributionWithTagsResultTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStreamingDistributionResultTypeDef = TypedDict(
     "GetStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStreamingDistributionResultTypeDef = TypedDict(
     "UpdateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
     },
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionListTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
-_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionSummaryTypeDef],
     },
     total=False,
 )
 
-class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
-    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
-    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+
+class FieldLevelEncryptionListTypeDef(
+    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
 ):
     pass
 
-_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionListTypeDef",
+
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionListTypeDef",
+
+FieldLevelEncryptionConfigUnionTypeDef = Union[
+    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+]
+_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionSummaryTypeDef],
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "IfMatch": str,
     },
     total=False,
 )
 
-class FieldLevelEncryptionListTypeDef(
-    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
+
+class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
+    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResponseHeadersPolicyResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseHeadersPolicySummaryTypeDef = TypedDict(
     "ResponseHeadersPolicySummaryTypeDef",
     {
         "Type": ResponseHeadersPolicyTypeType,
@@ -4559,125 +6115,167 @@
 )
 
 UpdateResponseHeadersPolicyResultTypeDef = TypedDict(
     "UpdateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDistributionConfigTypeDef = TypedDict(
-    "_RequiredDistributionConfigTypeDef",
+_RequiredDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
         "Comment": str,
         "Enabled": bool,
     },
 )
-_OptionalDistributionConfigTypeDef = TypedDict(
-    "_OptionalDistributionConfigTypeDef",
+_OptionalDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalDistributionConfigOutputTypeDef",
     {
-        "Aliases": AliasesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
         "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Logging": LoggingConfigTypeDef,
         "PriceClass": PriceClassType,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
     total=False,
 )
 
-class DistributionConfigTypeDef(
-    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+
+class DistributionConfigOutputTypeDef(
+    _RequiredDistributionConfigOutputTypeDef, _OptionalDistributionConfigOutputTypeDef
 ):
     pass
 
+
 _RequiredDistributionSummaryTypeDef = TypedDict(
     "_RequiredDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesTypeDef,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
         "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
 _OptionalDistributionSummaryTypeDef = TypedDict(
     "_OptionalDistributionSummaryTypeDef",
     {
-        "OriginGroups": OriginGroupsTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
+
 class DistributionSummaryTypeDef(
     _RequiredDistributionSummaryTypeDef, _OptionalDistributionSummaryTypeDef
 ):
     pass
 
+
+_RequiredDistributionConfigTypeDef = TypedDict(
+    "_RequiredDistributionConfigTypeDef",
+    {
+        "CallerReference": str,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Comment": str,
+        "Enabled": bool,
+    },
+)
+_OptionalDistributionConfigTypeDef = TypedDict(
+    "_OptionalDistributionConfigTypeDef",
+    {
+        "Aliases": AliasesTypeDef,
+        "DefaultRootObject": str,
+        "OriginGroups": OriginGroupsTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Logging": LoggingConfigTypeDef,
+        "PriceClass": PriceClassType,
+        "ViewerCertificate": ViewerCertificateTypeDef,
+        "Restrictions": RestrictionsTypeDef,
+        "WebACLId": str,
+        "HttpVersion": HttpVersionType,
+        "IsIPV6Enabled": bool,
+        "ContinuousDeploymentPolicyId": str,
+        "Staging": bool,
+    },
+    total=False,
+)
+
+
+class DistributionConfigTypeDef(
+    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+):
+    pass
+
+
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
     },
 )
 
 CreateCachePolicyResultTypeDef = TypedDict(
     "CreateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCachePolicyResultTypeDef = TypedDict(
     "GetCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCachePolicyResultTypeDef = TypedDict(
     "UpdateCachePolicyResultTypeDef",
     {
         "CachePolicy": CachePolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOriginRequestPolicyListTypeDef = TypedDict(
     "_RequiredOriginRequestPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4689,123 +6287,125 @@
     {
         "NextMarker": str,
         "Items": List[OriginRequestPolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class OriginRequestPolicyListTypeDef(
     _RequiredOriginRequestPolicyListTypeDef, _OptionalOriginRequestPolicyListTypeDef
 ):
     pass
 
+
 ContinuousDeploymentPolicySummaryTypeDef = TypedDict(
     "ContinuousDeploymentPolicySummaryTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
     },
 )
 
 CreateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContinuousDeploymentPolicyResultTypeDef = TypedDict(
     "UpdateContinuousDeploymentPolicyResultTypeDef",
     {
         "ContinuousDeploymentPolicy": ContinuousDeploymentPolicyTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionProfileResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     {
         "FieldLevelEncryptionProfile": FieldLevelEncryptionProfileTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionProfilesResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     {
         "FieldLevelEncryptionProfileList": FieldLevelEncryptionProfileListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFieldLevelEncryptionResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     {
         "FieldLevelEncryption": FieldLevelEncryptionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFieldLevelEncryptionConfigsResultTypeDef = TypedDict(
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     {
         "FieldLevelEncryptionList": FieldLevelEncryptionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResponseHeadersPolicyListTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4817,65 +6417,93 @@
     {
         "NextMarker": str,
         "Items": List[ResponseHeadersPolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class ResponseHeadersPolicyListTypeDef(
     _RequiredResponseHeadersPolicyListTypeDef, _OptionalResponseHeadersPolicyListTypeDef
 ):
     pass
 
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
 
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
     "_OptionalDistributionTypeDef",
     {
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
         "ActiveTrustedKeyGroups": ActiveTrustedKeyGroupsTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
+
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
+
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDistributionListTypeDef = TypedDict(
+    "_RequiredDistributionListTypeDef",
+    {
+        "Marker": str,
+        "MaxItems": int,
+        "IsTruncated": bool,
+        "Quantity": int,
+    },
+)
+_OptionalDistributionListTypeDef = TypedDict(
+    "_OptionalDistributionListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[DistributionSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
+    pass
+
+
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+
+DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
     },
 )
 
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
@@ -4886,40 +6514,21 @@
     "_OptionalUpdateDistributionRequestRequestTypeDef",
     {
         "IfMatch": str,
     },
     total=False,
 )
 
+
 class UpdateDistributionRequestRequestTypeDef(
     _RequiredUpdateDistributionRequestRequestTypeDef,
     _OptionalUpdateDistributionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDistributionListTypeDef = TypedDict(
-    "_RequiredDistributionListTypeDef",
-    {
-        "Marker": str,
-        "MaxItems": int,
-        "IsTruncated": bool,
-        "Quantity": int,
-    },
-)
-_OptionalDistributionListTypeDef = TypedDict(
-    "_OptionalDistributionListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[DistributionSummaryTypeDef],
-    },
-    total=False,
-)
-
-class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
-    pass
 
 _RequiredCachePolicyListTypeDef = TypedDict(
     "_RequiredCachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
     },
@@ -4929,22 +6538,24 @@
     {
         "NextMarker": str,
         "Items": List[CachePolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class CachePolicyListTypeDef(_RequiredCachePolicyListTypeDef, _OptionalCachePolicyListTypeDef):
     pass
 
+
 ListOriginRequestPoliciesResultTypeDef = TypedDict(
     "ListOriginRequestPoliciesResultTypeDef",
     {
         "OriginRequestPolicyList": OriginRequestPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredContinuousDeploymentPolicyListTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyListTypeDef",
     {
         "MaxItems": int,
@@ -4956,123 +6567,125 @@
     {
         "NextMarker": str,
         "Items": List[ContinuousDeploymentPolicySummaryTypeDef],
     },
     total=False,
 )
 
+
 class ContinuousDeploymentPolicyListTypeDef(
     _RequiredContinuousDeploymentPolicyListTypeDef, _OptionalContinuousDeploymentPolicyListTypeDef
 ):
     pass
 
+
 ListResponseHeadersPoliciesResultTypeDef = TypedDict(
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionWithTagsResultTypeDef = TypedDict(
     "CreateDistributionWithTagsResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionResultTypeDef = TypedDict(
     "GetDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionWithStagingConfigResultTypeDef = TypedDict(
     "UpdateDistributionWithStagingConfigResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByRealtimeLogConfigResultTypeDef = TypedDict(
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsByWebACLIdResultTypeDef = TypedDict(
     "ListDistributionsByWebACLIdResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributionsResultTypeDef = TypedDict(
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
     },
 )
 
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListContinuousDeploymentPoliciesResultTypeDef = TypedDict(
     "ListContinuousDeploymentPoliciesResultTypeDef",
     {
         "ContinuousDeploymentPolicyList": ContinuousDeploymentPolicyListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.py` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront/waiter.pyi` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/PKG-INFO` & `types-aiobotocore-cloudfront-2.5.2.post1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-cloudfront
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudFront 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudfront"></a>
 
 # types-aiobotocore-cloudfront
 
 [![PyPI - types-aiobotocore-cloudfront](https://img.shields.io/pypi/v/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudfront.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudfront?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudfront)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudfront)](https://pepy.tech/project/types-aiobotocore-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudFront 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [types-aiobotocore-cloudfront docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudfront/).
 
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
@@ -395,46 +362,57 @@
 )
 
 
 def check_value(value: CachePolicyCookieBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudfront.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
+    AliasesOutputTypeDef,
     AliasesTypeDef,
+    CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    BlobTypeDef,
+    TrustedKeyGroupsOutputTypeDef,
+    TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
+    CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
     ContentTypeProfileTypeDef,
+    StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
     CustomErrorResponseTypeDef,
     OriginCustomHeaderTypeDef,
+    OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
     DeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     DeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
@@ -447,20 +425,22 @@
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
-    EmptyResponseMetadataTypeDef,
+    FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
     KinesisStreamConfigTypeDef,
+    QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
     FunctionAssociationTypeDef,
     FunctionMetadataTypeDef,
+    GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigRequestRequestTypeDef,
     GetContinuousDeploymentPolicyRequestRequestTypeDef,
@@ -468,271 +448,332 @@
     WaiterConfigTypeDef,
     GetDistributionRequestRequestTypeDef,
     GetFieldLevelEncryptionConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
-    GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
+    KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
+    PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
-    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
     ListDistributionsByKeyGroupRequestRequestTypeDef,
     ListDistributionsByOriginRequestPolicyIdRequestRequestTypeDef,
     ListDistributionsByRealtimeLogConfigRequestRequestTypeDef,
     ListDistributionsByResponseHeadersPolicyIdRequestRequestTypeDef,
     ListDistributionsByWebACLIdRequestRequestTypeDef,
-    ListDistributionsRequestListDistributionsPaginateTypeDef,
     ListDistributionsRequestRequestTypeDef,
     ListFieldLevelEncryptionConfigsRequestRequestTypeDef,
     ListFieldLevelEncryptionProfilesRequestRequestTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
     ListInvalidationsRequestRequestTypeDef,
     ListKeyGroupsRequestRequestTypeDef,
     ListOriginAccessControlsRequestRequestTypeDef,
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
-    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
+    StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
     OriginGroupMemberTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
-    PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
     QueryArgProfileTypeDef,
+    ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
+    ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
+    ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
+    ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
-    ResponseMetadataTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
-    TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    TestFunctionRequestRequestTypeDef,
+    CachePolicyCookiesConfigOutputTypeDef,
+    CookiePreferenceOutputTypeDef,
+    OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
+    CachePolicyHeadersConfigOutputTypeDef,
+    OriginRequestPolicyHeadersConfigOutputTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
+    CachePolicyQueryStringsConfigOutputTypeDef,
+    OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
     CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
-    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
+    ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    GetFunctionResultTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
-    GetKeyGroupConfigResultTypeDef,
-    KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
     GetOriginAccessControlConfigResultTypeDef,
     OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
     GetPublicKeyConfigResultTypeDef,
     PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
+    CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
+    CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
+    CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
+    EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
     EndPointTypeDef,
+    FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
+    RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
+    GetKeyGroupConfigResultTypeDef,
+    KeyGroupConfigUnionTypeDef,
+    KeyGroupTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
+    LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
+    ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
+    ListDistributionsRequestListDistributionsPaginateTypeDef,
+    ListInvalidationsRequestListInvalidationsPaginateTypeDef,
+    ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
+    OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
+    OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
+    QueryArgProfilesOutputTypeDef,
     QueryArgProfilesTypeDef,
+    ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
+    ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
+    ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
+    ForwardedValuesOutputTypeDef,
     ForwardedValuesTypeDef,
+    ParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     ParametersInCacheKeyAndForwardedToOriginTypeDef,
     OriginRequestPolicyConfigTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
+    ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
     TrafficConfigTypeDef,
-    CreateKeyGroupResultTypeDef,
-    GetKeyGroupResultTypeDef,
-    KeyGroupSummaryTypeDef,
-    UpdateKeyGroupResultTypeDef,
     CreateOriginAccessControlResultTypeDef,
     GetOriginAccessControlResultTypeDef,
     UpdateOriginAccessControlResultTypeDef,
     CreatePublicKeyResultTypeDef,
     GetPublicKeyResultTypeDef,
     UpdatePublicKeyResultTypeDef,
+    OriginOutputTypeDef,
     OriginTypeDef,
+    EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
     CreateRealtimeLogConfigRequestRequestTypeDef,
     RealtimeLogConfigTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
-    CreateInvalidationRequestRequestTypeDef,
+    CreateKeyGroupResultTypeDef,
+    GetKeyGroupResultTypeDef,
+    KeyGroupSummaryTypeDef,
+    UpdateKeyGroupResultTypeDef,
     InvalidationTypeDef,
+    CreateInvalidationRequestRequestTypeDef,
+    InvalidationBatchUnionTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
     CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
     ListOriginAccessControlsResultTypeDef,
+    OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
+    QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
-    CreateStreamingDistributionRequestRequestTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
+    CreateStreamingDistributionRequestRequestTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsUnionTypeDef,
+    CacheBehaviorOutputTypeDef,
+    DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
-    CachePolicyConfigTypeDef,
-    CreateOriginRequestPolicyRequestRequestTypeDef,
+    CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
+    CachePolicyConfigTypeDef,
+    CreateOriginRequestPolicyRequestRequestTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
-    KeyGroupListTypeDef,
+    OriginsOutputTypeDef,
     OriginsTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     RealtimeLogConfigsTypeDef,
     UpdateRealtimeLogConfigResultTypeDef,
     ListFunctionsResultTypeDef,
     TestFunctionResultTypeDef,
+    KeyGroupListTypeDef,
     CreateInvalidationResultTypeDef,
     GetInvalidationResultTypeDef,
     StreamingDistributionTypeDef,
+    OriginGroupsOutputTypeDef,
     OriginGroupsTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
-    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
+    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
+    CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
-    CreateCachePolicyRequestRequestTypeDef,
     GetCachePolicyConfigResultTypeDef,
-    UpdateCachePolicyRequestRequestTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CachePolicyConfigUnionTypeDef,
+    CreateCachePolicyRequestRequestTypeDef,
+    UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
-    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
+    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
-    ListKeyGroupsResultTypeDef,
-    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
-    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
+    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
+    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
+    ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
-    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
-    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionListTypeDef,
+    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
+    DistributionConfigTypeDef,
     CachePolicySummaryTypeDef,
     CreateCachePolicyResultTypeDef,
     GetCachePolicyResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     OriginRequestPolicyListTypeDef,
     ContinuousDeploymentPolicySummaryTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
@@ -743,40 +784,41 @@
     UpdateFieldLevelEncryptionProfileResultTypeDef,
     ListFieldLevelEncryptionProfilesResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
     GetFieldLevelEncryptionResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
-    CreateDistributionRequestRequestTypeDef,
-    DistributionConfigWithTagsTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
-    UpdateDistributionRequestRequestTypeDef,
     DistributionListTypeDef,
+    CreateDistributionRequestRequestTypeDef,
+    DistributionConfigUnionTypeDef,
+    DistributionConfigWithTagsTypeDef,
+    UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
-    CreateDistributionWithTagsRequestRequestTypeDef,
     CopyDistributionResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     GetDistributionResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     ListDistributionsByRealtimeLogConfigResultTypeDef,
     ListDistributionsByWebACLIdResultTypeDef,
     ListDistributionsResultTypeDef,
+    CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
-def get_structure() -> AliasICPRecordalTypeDef:
+def get_value() -> AliasICPRecordalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudfront-2.5.2/types_aiobotocore_cloudfront.egg-info/SOURCES.txt` & `types-aiobotocore-cloudfront-2.5.2.post1/types_aiobotocore_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*


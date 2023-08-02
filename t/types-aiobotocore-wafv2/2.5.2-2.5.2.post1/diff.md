# Comparing `tmp/types-aiobotocore-wafv2-2.5.2.tar.gz` & `tmp/types-aiobotocore-wafv2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wafv2-2.5.2.tar", last modified: Sat Jul  8 01:44:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-wafv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
```

## Comparing `types-aiobotocore-wafv2-2.5.2.tar` & `types-aiobotocore-wafv2-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.655037 types-aiobotocore-wafv2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-07-08 01:44:27.655037 types-aiobotocore-wafv2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18496 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:27.655037 types-aiobotocore-wafv2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.655037 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39179 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39118 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-07-08 01:42:30.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68396 2023-07-08 01:42:31.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68315 2023-07-08 01:42:30.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:29.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.655037 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-07-08 01:44:27.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-08 01:44:27.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:27.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:44:27.000000 types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.421429 types-aiobotocore-wafv2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-08-02 14:53:09.417430 types-aiobotocore-wafv2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.421429 types-aiobotocore-wafv2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.413430 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-08-02 14:51:07.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39179 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-08-02 14:51:07.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-02 14:51:07.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    88004 2023-08-02 14:51:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87901 2023-08-02 14:51:08.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:06.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.417430 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:53:09.000000 types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wafv2-2.5.2/LICENSE` & `types-aiobotocore-wafv2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2/PKG-INFO` & `types-aiobotocore-wafv2-2.5.2.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wafv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore wafv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-wafv2"></a>
 
 # types-aiobotocore-wafv2
 
 [![PyPI - types-aiobotocore-wafv2](https://img.shields.io/pypi/v/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wafv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-wafv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAFV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [types-aiobotocore-wafv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -304,51 +303,52 @@
 )
 
 
 def check_value(value: ActionValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wafv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wafv2.type_defs import (
     APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
     AddressFieldTypeDef,
+    AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BlobTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    CheckCapacityResponseTypeDef,
+    ResponseMetadataTypeDef,
     LabelNameConditionTypeDef,
+    CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
-    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
     CustomHTTPHeaderTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
@@ -360,34 +360,33 @@
     EmailFieldTypeDef,
     ExcludedRuleTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
-    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
+    JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
     LabelMatchStatementTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
@@ -396,50 +395,66 @@
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
     NotStatementTypeDef,
+    OrStatementOutputTypeDef,
     OrStatementTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RateLimitLabelNamespaceTypeDef,
+    ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
+    ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
+    ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
+    ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateIPSetResponseTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
-    UpdateRegexPatternSetResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    UpdateWebACLResponseTypeDef,
-    ListAPIKeysResponseTypeDef,
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
+    RateLimitCookieOutputTypeDef,
     RateLimitCookieTypeDef,
+    RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
     RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringOutputTypeDef,
     RateLimitQueryStringTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
+    CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
+    UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
+    UpdateRegexPatternSetResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    UpdateWebACLResponseTypeDef,
     ConditionTypeDef,
+    CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
     MobileSdkReleaseTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
@@ -448,91 +463,133 @@
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    CustomRequestHandlingOutputTypeDef,
     CustomRequestHandlingTypeDef,
+    CustomResponseOutputTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
+    GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
+    JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
+    ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    TimeWindowTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
+    AssociationConfigUnionTypeDef,
+    RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
+    AllowActionOutputTypeDef,
+    CaptchaActionOutputTypeDef,
+    ChallengeActionOutputTypeDef,
+    CountActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
+    BlockActionOutputTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetOutputTypeDef,
+    AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
+    RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
+    LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
+    OverrideActionOutputTypeDef,
     OverrideActionTypeDef,
+    DefaultActionOutputTypeDef,
+    RuleActionOutputTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
+    ByteMatchStatementOutputTypeDef,
+    RegexMatchStatementOutputTypeDef,
+    RegexPatternSetReferenceStatementOutputTypeDef,
+    SizeConstraintStatementOutputTypeDef,
+    SqliMatchStatementOutputTypeDef,
+    XssMatchStatementOutputTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
     RegexPatternSetReferenceStatementTypeDef,
     SizeConstraintStatementTypeDef,
     SqliMatchStatementTypeDef,
     XssMatchStatementTypeDef,
+    ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
-    RuleActionOverrideTypeDef,
+    RuleActionOverrideOutputTypeDef,
+    RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    DefaultActionUnionTypeDef,
+    RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    ManagedRuleGroupStatementOutputTypeDef,
+    RuleGroupReferenceStatementOutputTypeDef,
+    RuleGroupTypeDef,
+    DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
-    DescribeManagedRuleGroupResponseTypeDef,
+    RuleUnionTypeDef,
+    FirewallManagerStatementTypeDef,
+    StatementOutputTypeDef,
+    GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    RuleGroupTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
-    FirewallManagerStatementTypeDef,
-    StatementTypeDef,
-    GetRuleGroupResponseTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> APIKeySummaryTypeDef:
+def get_value() -> APIKeySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wafv2-2.5.2/README.md` & `types-aiobotocore-wafv2-2.5.2.post1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-wafv2"></a>
 
 # types-aiobotocore-wafv2
 
 [![PyPI - types-aiobotocore-wafv2](https://img.shields.io/pypi/v/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wafv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-wafv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAFV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [types-aiobotocore-wafv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -271,51 +271,52 @@
 )
 
 
 def check_value(value: ActionValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wafv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wafv2.type_defs import (
     APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
     AddressFieldTypeDef,
+    AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BlobTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    CheckCapacityResponseTypeDef,
+    ResponseMetadataTypeDef,
     LabelNameConditionTypeDef,
+    CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
-    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
     CustomHTTPHeaderTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
@@ -327,34 +328,33 @@
     EmailFieldTypeDef,
     ExcludedRuleTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
-    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
+    JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
     LabelMatchStatementTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
@@ -363,50 +363,66 @@
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
     NotStatementTypeDef,
+    OrStatementOutputTypeDef,
     OrStatementTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RateLimitLabelNamespaceTypeDef,
+    ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
+    ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
+    ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
+    ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateIPSetResponseTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
-    UpdateRegexPatternSetResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    UpdateWebACLResponseTypeDef,
-    ListAPIKeysResponseTypeDef,
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
+    RateLimitCookieOutputTypeDef,
     RateLimitCookieTypeDef,
+    RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
     RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringOutputTypeDef,
     RateLimitQueryStringTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
+    CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
+    UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
+    UpdateRegexPatternSetResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    UpdateWebACLResponseTypeDef,
     ConditionTypeDef,
+    CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
     MobileSdkReleaseTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
@@ -415,91 +431,133 @@
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    CustomRequestHandlingOutputTypeDef,
     CustomRequestHandlingTypeDef,
+    CustomResponseOutputTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
+    GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
+    JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
+    ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    TimeWindowTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
+    AssociationConfigUnionTypeDef,
+    RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
+    AllowActionOutputTypeDef,
+    CaptchaActionOutputTypeDef,
+    ChallengeActionOutputTypeDef,
+    CountActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
+    BlockActionOutputTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetOutputTypeDef,
+    AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
+    RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
+    LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
+    OverrideActionOutputTypeDef,
     OverrideActionTypeDef,
+    DefaultActionOutputTypeDef,
+    RuleActionOutputTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
+    ByteMatchStatementOutputTypeDef,
+    RegexMatchStatementOutputTypeDef,
+    RegexPatternSetReferenceStatementOutputTypeDef,
+    SizeConstraintStatementOutputTypeDef,
+    SqliMatchStatementOutputTypeDef,
+    XssMatchStatementOutputTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
     RegexPatternSetReferenceStatementTypeDef,
     SizeConstraintStatementTypeDef,
     SqliMatchStatementTypeDef,
     XssMatchStatementTypeDef,
+    ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
-    RuleActionOverrideTypeDef,
+    RuleActionOverrideOutputTypeDef,
+    RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    DefaultActionUnionTypeDef,
+    RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    ManagedRuleGroupStatementOutputTypeDef,
+    RuleGroupReferenceStatementOutputTypeDef,
+    RuleGroupTypeDef,
+    DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
-    DescribeManagedRuleGroupResponseTypeDef,
+    RuleUnionTypeDef,
+    FirewallManagerStatementTypeDef,
+    StatementOutputTypeDef,
+    GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    RuleGroupTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
-    FirewallManagerStatementTypeDef,
-    StatementTypeDef,
-    GetRuleGroupResponseTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> APIKeySummaryTypeDef:
+def get_value() -> APIKeySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wafv2-2.5.2/setup.py` & `types-aiobotocore-wafv2-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wafv2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore wafv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore wafv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_wafv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/"
```

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/__main__.py` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAFV2 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WAFV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/client.py` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,33 +10,32 @@
     from types_aiobotocore_wafv2.client import WAFV2Client
 
     session = get_session()
     async with session.create_client("wafv2") as client:
         client: WAFV2Client
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
-    AssociationConfigTypeDef,
+    AssociationConfigUnionTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
-    DefaultActionTypeDef,
+    DefaultActionUnionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
@@ -58,21 +57,22 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     TagTypeDef,
-    TimeWindowTypeDef,
+    TimestampTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
     VisibilityConfigTypeDef,
@@ -143,15 +143,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#can_paginate)
         """
 
     async def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[RuleTypeDef]
+        self, *, Scope: ScopeType, Rules: Sequence[RuleUnionTypeDef]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#check_capacity)
@@ -215,15 +215,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
@@ -231,24 +231,24 @@
         """
 
     async def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_web_acl)
         """
@@ -484,15 +484,15 @@
 
     async def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: TimeWindowTypeDef,
+        TimeWindow: TimeWindowUnionTypeDef,
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -647,15 +647,15 @@
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#list_web_acls)
         """
 
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#put_logging_configuration)
@@ -724,15 +724,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         VersionToExpire: str,
-        ExpiryTimestamp: Union[datetime, str]
+        ExpiryTimestamp: TimestampTypeDef
     ) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:
         """
         Updates the expiration information for your managed rule set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_managed_rule_set_version_expiry_date)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_managed_rule_set_version_expiry_date)
         """
@@ -759,15 +759,15 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_rule_group)
@@ -775,24 +775,24 @@
 
     async def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/client.pyi` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,33 +10,32 @@
     from types_aiobotocore_wafv2.client import WAFV2Client
 
     session = get_session()
     async with session.create_client("wafv2") as client:
         client: WAFV2Client
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
-    AssociationConfigTypeDef,
+    AssociationConfigUnionTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
-    DefaultActionTypeDef,
+    DefaultActionUnionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
@@ -58,21 +57,22 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     TagTypeDef,
-    TimeWindowTypeDef,
+    TimestampTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
     VisibilityConfigTypeDef,
@@ -137,15 +137,15 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#can_paginate)
         """
     async def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[RuleTypeDef]
+        self, *, Scope: ScopeType, Rules: Sequence[RuleUnionTypeDef]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#check_capacity)
@@ -204,39 +204,39 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_rule_group)
         """
     async def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#create_web_acl)
         """
@@ -449,15 +449,15 @@
         """
     async def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: TimeWindowTypeDef,
+        TimeWindow: TimeWindowUnionTypeDef,
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -597,15 +597,15 @@
         """
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#list_web_acls)
         """
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#put_logging_configuration)
@@ -668,15 +668,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         VersionToExpire: str,
-        ExpiryTimestamp: Union[datetime, str]
+        ExpiryTimestamp: TimestampTypeDef
     ) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:
         """
         Updates the expiration information for your managed rule set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_managed_rule_set_version_expiry_date)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_managed_rule_set_version_expiry_date)
         """
@@ -701,39 +701,39 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_rule_group)
         """
     async def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: DefaultActionTypeDef,
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[RuleTypeDef] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: AssociationConfigTypeDef = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/client/#update_web_acl)
         """
```

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/literals.py` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/literals.pyi` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/type_defs.py` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_wafv2.type_defs import APIKeySummaryTypeDef
 
-    data: APIKeySummaryTypeDef = {...}
+    data: APIKeySummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -56,38 +56,39 @@
 
 
 __all__ = (
     "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
+    "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    "BlobTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
-    "CheckCapacityResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "LabelNameConditionTypeDef",
+    "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
-    "CreateAPIKeyResponseTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
     "CustomHTTPHeaderTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DescribeAllManagedProductsRequestRequestTypeDef",
@@ -99,34 +100,33 @@
     "EmailFieldTypeDef",
     "ExcludedRuleTypeDef",
     "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyRequestRequestTypeDef",
-    "GetDecryptedAPIKeyResponseTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
-    "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
+    "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
     "LabelMatchStatementTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
@@ -135,50 +135,66 @@
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListManagedRuleSetsRequestRequestTypeDef",
     "ManagedRuleSetSummaryTypeDef",
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
     "NotStatementTypeDef",
+    "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
-    "PutManagedRuleSetVersionsResponseTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RateLimitLabelNamespaceTypeDef",
+    "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
+    "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
+    "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
+    "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateIPSetResponseTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
-    "UpdateRegexPatternSetResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
-    "UpdateWebACLResponseTypeDef",
-    "ListAPIKeysResponseTypeDef",
+    "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
+    "RateLimitCookieOutputTypeDef",
     "RateLimitCookieTypeDef",
+    "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
+    "RateLimitQueryArgumentOutputTypeDef",
     "RateLimitQueryArgumentTypeDef",
+    "RateLimitQueryStringOutputTypeDef",
     "RateLimitQueryStringTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
+    "CheckCapacityResponseTypeDef",
+    "CreateAPIKeyResponseTypeDef",
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    "GetDecryptedAPIKeyResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "ListAPIKeysResponseTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    "UpdateIPSetResponseTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    "UpdateRegexPatternSetResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
+    "UpdateWebACLResponseTypeDef",
     "ConditionTypeDef",
+    "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "MobileSdkReleaseTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
@@ -187,83 +203,125 @@
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
+    "CustomRequestHandlingOutputTypeDef",
     "CustomRequestHandlingTypeDef",
+    "CustomResponseOutputTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
+    "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
+    "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
+    "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
+    "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
+    "TimeWindowTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    "AssociationConfigUnionTypeDef",
+    "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
+    "AllowActionOutputTypeDef",
+    "CaptchaActionOutputTypeDef",
+    "ChallengeActionOutputTypeDef",
+    "CountActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
+    "BlockActionOutputTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
+    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
+    "AWSManagedRulesACFPRuleSetOutputTypeDef",
+    "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
+    "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
+    "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
+    "OverrideActionOutputTypeDef",
     "OverrideActionTypeDef",
+    "DefaultActionOutputTypeDef",
+    "RuleActionOutputTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
+    "ByteMatchStatementOutputTypeDef",
+    "RegexMatchStatementOutputTypeDef",
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    "SizeConstraintStatementOutputTypeDef",
+    "SqliMatchStatementOutputTypeDef",
+    "XssMatchStatementOutputTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
     "RegexPatternSetReferenceStatementTypeDef",
     "SizeConstraintStatementTypeDef",
     "SqliMatchStatementTypeDef",
     "XssMatchStatementTypeDef",
+    "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "RuleActionOverrideTypeDef",
+    "RuleActionOverrideOutputTypeDef",
+    "RuleOutputTypeDef",
     "RuleSummaryTypeDef",
+    "DefaultActionUnionTypeDef",
+    "RuleActionOverrideTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    "ManagedRuleGroupStatementOutputTypeDef",
+    "RuleGroupReferenceStatementOutputTypeDef",
+    "RuleGroupTypeDef",
+    "DescribeManagedRuleGroupResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
-    "DescribeManagedRuleGroupResponseTypeDef",
+    "RuleUnionTypeDef",
+    "FirewallManagerStatementTypeDef",
+    "StatementOutputTypeDef",
+    "GetRuleGroupResponseTypeDef",
+    "StatementTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
-    "RuleGroupTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
-    "FirewallManagerStatementTypeDef",
-    "StatementTypeDef",
-    "GetRuleGroupResponseTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -294,14 +352,21 @@
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
+AndStatementOutputTypeDef = TypedDict(
+    "AndStatementOutputTypeDef",
+    {
+        "Statements": List["StatementOutputTypeDef"],
+    },
+)
+
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -316,14 +381,15 @@
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
@@ -359,29 +425,42 @@
         "ResponseCode": int,
         "SolveTimestamp": int,
         "FailureReason": FailureReasonType,
     },
     total=False,
 )
 
-CheckCapacityResponseTypeDef = TypedDict(
-    "CheckCapacityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Capacity": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
+CookieMatchPatternOutputTypeDef = TypedDict(
+    "CookieMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedCookies": List[str],
+        "ExcludedCookies": List[str],
+    },
+    total=False,
+)
+
 CookieMatchPatternTypeDef = TypedDict(
     "CookieMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
@@ -392,22 +471,14 @@
     "CreateAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "TokenDomains": Sequence[str],
     },
 )
 
-CreateAPIKeyResponseTypeDef = TypedDict(
-    "CreateAPIKeyResponseTypeDef",
-    {
-        "APIKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -497,22 +568,14 @@
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "WebACLLockToken": str,
     },
 )
 
-DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
-    {
-        "NextWebACLLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
@@ -680,39 +743,22 @@
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     {
         "Platform": PlatformType,
         "ReleaseVersion": str,
     },
 )
 
-GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDecryptedAPIKeyRequestRequestTypeDef = TypedDict(
     "GetDecryptedAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "APIKey": str,
     },
 )
 
-GetDecryptedAPIKeyResponseTypeDef = TypedDict(
-    "GetDecryptedAPIKeyResponseTypeDef",
-    {
-        "TokenDomains": List[str],
-        "CreationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIPSetRequestRequestTypeDef = TypedDict(
     "GetIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
     },
@@ -768,22 +814,14 @@
 GetPermissionPolicyRequestRequestTypeDef = TypedDict(
     "GetPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "WebACLName": str,
         "WebACLId": str,
         "RuleName": str,
@@ -830,19 +868,19 @@
         "Scope": ScopeType,
         "Id": str,
         "ARN": str,
     },
     total=False,
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
+TimeWindowOutputTypeDef = TypedDict(
+    "TimeWindowOutputTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": datetime,
+        "EndTime": datetime,
     },
 )
 
 GetWebACLForResourceRequestRequestTypeDef = TypedDict(
     "GetWebACLForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -863,14 +901,24 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+HeaderMatchPatternOutputTypeDef = TypedDict(
+    "HeaderMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedHeaders": List[str],
+        "ExcludedHeaders": List[str],
+    },
+    total=False,
+)
+
 HeaderMatchPatternTypeDef = TypedDict(
     "HeaderMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
@@ -882,14 +930,23 @@
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
 )
 
+JsonMatchPatternOutputTypeDef = TypedDict(
+    "JsonMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedPaths": List[str],
+    },
+    total=False,
+)
+
 JsonMatchPatternTypeDef = TypedDict(
     "JsonMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
@@ -1154,22 +1211,14 @@
 class ListResourcesForWebACLRequestRequestTypeDef(
     _RequiredListResourcesForWebACLRequestRequestTypeDef,
     _OptionalListResourcesForWebACLRequestRequestTypeDef,
 ):
     pass
 
 
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRuleGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleGroupsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListRuleGroupsRequestRequestTypeDef = TypedDict(
@@ -1259,15 +1308,22 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": Dict[str, Any],
+        "Statement": "StatementTypeDef",
+    },
+)
+
+OrStatementOutputTypeDef = TypedDict(
+    "OrStatementOutputTypeDef",
+    {
+        "Statements": List[Dict[str, Any]],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
@@ -1286,22 +1342,14 @@
     {
         "AssociatedRuleGroupArn": str,
         "ForecastedLifetime": int,
     },
     total=False,
 )
 
-PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
-    "PutManagedRuleSetVersionsResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutPermissionPolicyRequestRequestTypeDef = TypedDict(
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
@@ -1309,59 +1357,83 @@
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
+ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
+    "ResponseInspectionBodyContainsOutputTypeDef",
+    {
+        "SuccessStrings": List[str],
+        "FailureStrings": List[str],
+    },
+)
+
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
 
+ResponseInspectionHeaderOutputTypeDef = TypedDict(
+    "ResponseInspectionHeaderOutputTypeDef",
+    {
+        "Name": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionHeaderTypeDef = TypedDict(
     "ResponseInspectionHeaderTypeDef",
     {
         "Name": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
+ResponseInspectionJsonOutputTypeDef = TypedDict(
+    "ResponseInspectionJsonOutputTypeDef",
+    {
+        "Identifier": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionJsonTypeDef = TypedDict(
     "ResponseInspectionJsonTypeDef",
     {
         "Identifier": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionStatusCodeTypeDef = TypedDict(
-    "ResponseInspectionStatusCodeTypeDef",
+ResponseInspectionStatusCodeOutputTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeOutputTypeDef",
     {
-        "SuccessCodes": Sequence[int],
-        "FailureCodes": Sequence[int],
+        "SuccessCodes": List[int],
+        "FailureCodes": List[int],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResponseInspectionStatusCodeTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SuccessCodes": Sequence[int],
+        "FailureCodes": Sequence[int],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1387,112 +1459,87 @@
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Scope": ScopeType,
-        "Id": str,
-        "LockToken": str,
-        "VersionToExpire": str,
-        "ExpiryTimestamp": Union[datetime, str],
-    },
-)
-
-UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
-    {
-        "ExpiringVersion": str,
-        "ExpiryTimestamp": datetime,
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+AssociationConfigOutputTypeDef = TypedDict(
+    "AssociationConfigOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
     },
+    total=False,
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+AssociationConfigTypeDef = TypedDict(
+    "AssociationConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Mapping[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
+        ],
     },
+    total=False,
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+RateLimitCookieOutputTypeDef = TypedDict(
+    "RateLimitCookieOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-ListAPIKeysResponseTypeDef = TypedDict(
-    "ListAPIKeysResponseTypeDef",
+RateLimitCookieTypeDef = TypedDict(
+    "RateLimitCookieTypeDef",
     {
-        "NextMarker": str,
-        "APIKeySummaries": List[APIKeySummaryTypeDef],
-        "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-AssociationConfigTypeDef = TypedDict(
-    "AssociationConfigTypeDef",
+RateLimitHeaderOutputTypeDef = TypedDict(
+    "RateLimitHeaderOutputTypeDef",
     {
-        "RequestBody": Mapping[
-            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
-        ],
+        "Name": str,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
-    total=False,
 )
 
-RateLimitCookieTypeDef = TypedDict(
-    "RateLimitCookieTypeDef",
+RateLimitHeaderTypeDef = TypedDict(
+    "RateLimitHeaderTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderTypeDef = TypedDict(
-    "RateLimitHeaderTypeDef",
+RateLimitQueryArgumentOutputTypeDef = TypedDict(
+    "RateLimitQueryArgumentOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": Sequence[TextTransformationTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 RateLimitQueryArgumentTypeDef = TypedDict(
     "RateLimitQueryArgumentTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+RateLimitQueryStringOutputTypeDef = TypedDict(
+    "RateLimitQueryStringOutputTypeDef",
+    {
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
 RateLimitQueryStringTypeDef = TypedDict(
     "RateLimitQueryStringTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
@@ -1508,23 +1555,149 @@
     "ChallengeConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
     total=False,
 )
 
+CheckCapacityResponseTypeDef = TypedDict(
+    "CheckCapacityResponseTypeDef",
+    {
+        "Capacity": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAPIKeyResponseTypeDef = TypedDict(
+    "CreateAPIKeyResponseTypeDef",
+    {
+        "APIKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    {
+        "NextWebACLLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecryptedAPIKeyResponseTypeDef = TypedDict(
+    "GetDecryptedAPIKeyResponseTypeDef",
+    {
+        "TokenDomains": List[str],
+        "CreationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAPIKeysResponseTypeDef = TypedDict(
+    "ListAPIKeysResponseTypeDef",
+    {
+        "NextMarker": str,
+        "APIKeySummaries": List[APIKeySummaryTypeDef],
+        "ApplicationIntegrationURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    {
+        "ExpiringVersion": str,
+        "ExpiryTimestamp": datetime,
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
 )
 
+CookiesOutputTypeDef = TypedDict(
+    "CookiesOutputTypeDef",
+    {
+        "MatchPattern": CookieMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 CookiesTypeDef = TypedDict(
     "CookiesTypeDef",
     {
         "MatchPattern": CookieMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1583,24 +1756,24 @@
     },
 )
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "Summary": IPSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIPSetsResponseTypeDef = TypedDict(
     "ListIPSetsResponseTypeDef",
     {
         "NextMarker": str,
         "IPSets": List[IPSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1663,68 +1836,97 @@
     pass
 
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "Summary": RegexPatternSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexPatternSetsResponseTypeDef = TypedDict(
     "ListRegexPatternSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexPatternSets": List[RegexPatternSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "Summary": RuleGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "Summary": WebACLSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebACLsResponseTypeDef = TypedDict(
     "ListWebACLsResponseTypeDef",
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomRequestHandlingOutputTypeDef = TypedDict(
+    "CustomRequestHandlingOutputTypeDef",
+    {
+        "InsertHeaders": List[CustomHTTPHeaderTypeDef],
     },
 )
 
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
+_RequiredCustomResponseOutputTypeDef = TypedDict(
+    "_RequiredCustomResponseOutputTypeDef",
+    {
+        "ResponseCode": int,
+    },
+)
+_OptionalCustomResponseOutputTypeDef = TypedDict(
+    "_OptionalCustomResponseOutputTypeDef",
+    {
+        "CustomResponseBodyKey": str,
+        "ResponseHeaders": List[CustomHTTPHeaderTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomResponseOutputTypeDef(
+    _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomResponseTypeDef = TypedDict(
     "_RequiredCustomResponseTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseTypeDef = TypedDict(
@@ -1741,61 +1943,59 @@
     pass
 
 
 DescribeAllManagedProductsResponseTypeDef = TypedDict(
     "DescribeAllManagedProductsResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedProductsByVendorResponseTypeDef = TypedDict(
     "DescribeManagedProductsByVendorResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GeoMatchStatementOutputTypeDef = TypedDict(
+    "GeoMatchStatementOutputTypeDef",
+    {
+        "CountryCodes": List[CountryCodeType],
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+    },
+    total=False,
+)
+
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
         "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
     total=False,
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedStatementManagedKeysResponseTypeDef = TypedDict(
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclArn": str,
-        "RuleMetricName": str,
-        "Scope": ScopeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1804,14 +2004,23 @@
         "Method": str,
         "HTTPVersion": str,
         "Headers": List[HTTPHeaderTypeDef],
     },
     total=False,
 )
 
+HeadersOutputTypeDef = TypedDict(
+    "HeadersOutputTypeDef",
+    {
+        "MatchPattern": HeaderMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1834,14 +2043,35 @@
 
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
 
+_RequiredJsonBodyOutputTypeDef = TypedDict(
+    "_RequiredJsonBodyOutputTypeDef",
+    {
+        "MatchPattern": JsonMatchPatternOutputTypeDef,
+        "MatchScope": JsonMatchScopeType,
+    },
+)
+_OptionalJsonBodyOutputTypeDef = TypedDict(
+    "_OptionalJsonBodyOutputTypeDef",
+    {
+        "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+    total=False,
+)
+
+
+class JsonBodyOutputTypeDef(_RequiredJsonBodyOutputTypeDef, _OptionalJsonBodyOutputTypeDef):
+    pass
+
+
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -1861,42 +2091,42 @@
 
 ListAvailableManagedRuleGroupVersionsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[ManagedRuleGroupVersionTypeDef],
         "CurrentDefaultVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableManagedRuleGroupsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleGroups": List[ManagedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedRuleSetsResponseTypeDef = TypedDict(
     "ListManagedRuleSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleSets": List[ManagedRuleSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileSdkReleasesResponseTypeDef = TypedDict(
     "ListMobileSdkReleasesResponseTypeDef",
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
@@ -1925,14 +2155,39 @@
 )
 
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
 
+_RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_RequiredRequestInspectionACFPOutputTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+    },
+)
+_OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_OptionalRequestInspectionACFPOutputTypeDef",
+    {
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "EmailField": EmailFieldTypeDef,
+        "PhoneNumberFields": List[PhoneNumberFieldTypeDef],
+        "AddressFields": List[AddressFieldTypeDef],
+    },
+    total=False,
+)
+
+
+class RequestInspectionACFPOutputTypeDef(
+    _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
+):
+    pass
+
+
 _RequiredRequestInspectionACFPTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPTypeDef = TypedDict(
@@ -1976,25 +2231,72 @@
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ResponseInspectionOutputTypeDef = TypedDict(
+    "ResponseInspectionOutputTypeDef",
+    {
+        "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
+        "Header": ResponseInspectionHeaderOutputTypeDef,
+        "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
+        "Json": ResponseInspectionJsonOutputTypeDef,
+    },
+    total=False,
+)
+
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Scope": ScopeType,
+        "Id": str,
+        "LockToken": str,
+        "VersionToExpire": str,
+        "ExpiryTimestamp": TimestampTypeDef,
+    },
+)
+
+AssociationConfigUnionTypeDef = Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef]
+RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
+    "RateBasedStatementCustomKeyOutputTypeDef",
+    {
+        "Header": RateLimitHeaderOutputTypeDef,
+        "Cookie": RateLimitCookieOutputTypeDef,
+        "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
+        "QueryString": RateLimitQueryStringOutputTypeDef,
+        "HTTPMethod": Dict[str, Any],
+        "ForwardedIP": Dict[str, Any],
+        "IP": Dict[str, Any],
+        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+    },
+    total=False,
+)
+
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
     {
         "Header": RateLimitHeaderTypeDef,
         "Cookie": RateLimitCookieTypeDef,
         "QueryArgument": RateLimitQueryArgumentTypeDef,
         "QueryString": RateLimitQueryStringTypeDef,
@@ -2002,47 +2304,88 @@
         "ForwardedIP": Mapping[str, Any],
         "IP": Mapping[str, Any],
         "LabelNamespace": RateLimitLabelNamespaceTypeDef,
     },
     total=False,
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "Behavior": FilterBehaviorType,
+        "Requirement": FilterRequirementType,
+        "Conditions": List[ConditionTypeDef],
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionTypeDef],
+        "Conditions": Sequence[ConditionTypeDef],
     },
 )
 
 GetMobileSdkReleaseResponseTypeDef = TypedDict(
     "GetMobileSdkReleaseResponseTypeDef",
     {
         "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextMarker": str,
         "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AllowActionOutputTypeDef = TypedDict(
+    "AllowActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
+)
+
+CaptchaActionOutputTypeDef = TypedDict(
+    "CaptchaActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
+)
+
+ChallengeActionOutputTypeDef = TypedDict(
+    "ChallengeActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
+)
+
+CountActionOutputTypeDef = TypedDict(
+    "CountActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
 )
 
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
@@ -2069,14 +2412,22 @@
     "CountActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
 
+BlockActionOutputTypeDef = TypedDict(
+    "BlockActionOutputTypeDef",
+    {
+        "CustomResponse": CustomResponseOutputTypeDef,
+    },
+    total=False,
+)
+
 BlockActionTypeDef = TypedDict(
     "BlockActionTypeDef",
     {
         "CustomResponse": CustomResponseTypeDef,
     },
     total=False,
 )
@@ -2107,14 +2458,32 @@
 
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
 
+FieldToMatchOutputTypeDef = TypedDict(
+    "FieldToMatchOutputTypeDef",
+    {
+        "SingleHeader": SingleHeaderTypeDef,
+        "SingleQueryArgument": SingleQueryArgumentTypeDef,
+        "AllQueryArguments": Dict[str, Any],
+        "UriPath": Dict[str, Any],
+        "QueryString": Dict[str, Any],
+        "Body": BodyTypeDef,
+        "Method": Dict[str, Any],
+        "JsonBody": JsonBodyOutputTypeDef,
+        "Headers": HeadersOutputTypeDef,
+        "Cookies": CookiesOutputTypeDef,
+        "HeaderOrder": HeaderOrderTypeDef,
+    },
+    total=False,
+)
+
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
@@ -2130,18 +2499,66 @@
 )
 
 GetManagedRuleSetResponseTypeDef = TypedDict(
     "GetManagedRuleSetResponseTypeDef",
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "CreationPath": str,
+        "RegistrationPagePath": str,
+        "RequestInspection": RequestInspectionACFPOutputTypeDef,
+    },
+)
+_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
+    },
+    total=False,
+)
+
+
+class AWSManagedRulesACFPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef,
+    _OptionalAWSManagedRulesACFPRuleSetOutputTypeDef,
+):
+    pass
+
+
+_RequiredAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "LoginPath": str,
+    },
+)
+_OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "RequestInspection": RequestInspectionTypeDef,
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
     },
+    total=False,
 )
 
+
+class AWSManagedRulesATPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesATPRuleSetOutputTypeDef, _OptionalAWSManagedRulesATPRuleSetOutputTypeDef
+):
+    pass
+
+
 _RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPTypeDef,
     },
@@ -2181,55 +2598,129 @@
 
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
 
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
+    {
+        "WebAclArn": str,
+        "RuleMetricName": str,
+        "Scope": ScopeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
+    },
+)
+
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
+_RequiredRateBasedStatementOutputTypeDef = TypedDict(
+    "_RequiredRateBasedStatementOutputTypeDef",
+    {
+        "Limit": int,
+        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+    },
+)
+_OptionalRateBasedStatementOutputTypeDef = TypedDict(
+    "_OptionalRateBasedStatementOutputTypeDef",
+    {
+        "ScopeDownStatement": "StatementOutputTypeDef",
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+        "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RateBasedStatementOutputTypeDef(
+    _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
+):
+    pass
+
+
 _RequiredRateBasedStatementTypeDef = TypedDict(
     "_RequiredRateBasedStatementTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementTypeDef = TypedDict(
     "_OptionalRateBasedStatementTypeDef",
     {
-        "ScopeDownStatement": "StatementTypeDef",
+        "ScopeDownStatement": Dict[str, Any],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
         "CustomKeys": Sequence[RateBasedStatementCustomKeyTypeDef],
     },
     total=False,
 )
 
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
 ):
     pass
 
 
+LoggingFilterOutputTypeDef = TypedDict(
+    "LoggingFilterOutputTypeDef",
+    {
+        "Filters": List[FilterOutputTypeDef],
+        "DefaultBehavior": FilterBehaviorType,
+    },
+)
+
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
-        "Filters": List[FilterTypeDef],
+        "Filters": Sequence[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
 
+OverrideActionOutputTypeDef = TypedDict(
+    "OverrideActionOutputTypeDef",
+    {
+        "Count": CountActionOutputTypeDef,
+        "None": Dict[str, Any],
+    },
+    total=False,
+)
+
 OverrideActionTypeDef = TypedDict(
     "OverrideActionTypeDef",
     {
         "Count": CountActionTypeDef,
         "None": Mapping[str, Any],
     },
     total=False,
 )
 
+DefaultActionOutputTypeDef = TypedDict(
+    "DefaultActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+    },
+    total=False,
+)
+
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+        "Count": CountActionOutputTypeDef,
+        "Captcha": CaptchaActionOutputTypeDef,
+        "Challenge": ChallengeActionOutputTypeDef,
+    },
+    total=False,
+)
+
 DefaultActionTypeDef = TypedDict(
     "DefaultActionTypeDef",
     {
         "Block": BlockActionTypeDef,
         "Allow": AllowActionTypeDef,
     },
     total=False,
@@ -2248,23 +2739,91 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeWindow": TimeWindowOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ByteMatchStatementOutputTypeDef = TypedDict(
+    "ByteMatchStatementOutputTypeDef",
+    {
+        "SearchString": bytes,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
+RegexMatchStatementOutputTypeDef = TypedDict(
+    "RegexMatchStatementOutputTypeDef",
+    {
+        "RegexString": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
+RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
+SizeConstraintStatementOutputTypeDef = TypedDict(
+    "SizeConstraintStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
+_RequiredSqliMatchStatementOutputTypeDef = TypedDict(
+    "_RequiredSqliMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+_OptionalSqliMatchStatementOutputTypeDef = TypedDict(
+    "_OptionalSqliMatchStatementOutputTypeDef",
+    {
+        "SensitivityLevel": SensitivityLevelType,
+    },
+    total=False,
+)
+
+
+class SqliMatchStatementOutputTypeDef(
+    _RequiredSqliMatchStatementOutputTypeDef, _OptionalSqliMatchStatementOutputTypeDef
+):
+    pass
+
+
+XssMatchStatementOutputTypeDef = TypedDict(
+    "XssMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
-        "SearchString": Union[str, bytes, IO[Any], StreamingBody],
+        "SearchString": BlobTypeDef,
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 RegexMatchStatementTypeDef = TypedDict(
@@ -2321,69 +2880,142 @@
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+ManagedRuleGroupConfigOutputTypeDef = TypedDict(
+    "ManagedRuleGroupConfigOutputTypeDef",
+    {
+        "LoginPath": str,
+        "PayloadType": PayloadTypeType,
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
+        "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
+        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagedRuleGroupConfigTypeDef = TypedDict(
     "ManagedRuleGroupConfigTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
+_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
+    },
+)
+_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationOutputTypeDef",
+    {
+        "RedactedFields": List[FieldToMatchOutputTypeDef],
+        "ManagedByFirewallManager": bool,
+        "LoggingFilter": LoggingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
+        "LogDestinationConfigs": Sequence[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "RedactedFields": Sequence[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
 
-RuleActionOverrideTypeDef = TypedDict(
-    "RuleActionOverrideTypeDef",
+RuleActionOverrideOutputTypeDef = TypedDict(
+    "RuleActionOverrideOutputTypeDef",
     {
         "Name": str,
-        "ActionToUse": RuleActionTypeDef,
+        "ActionToUse": RuleActionOutputTypeDef,
     },
 )
 
+_RequiredRuleOutputTypeDef = TypedDict(
+    "_RequiredRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Priority": int,
+        "Statement": "StatementOutputTypeDef",
+        "VisibilityConfig": VisibilityConfigTypeDef,
+    },
+)
+_OptionalRuleOutputTypeDef = TypedDict(
+    "_OptionalRuleOutputTypeDef",
+    {
+        "Action": RuleActionOutputTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
+        "RuleLabels": List[LabelTypeDef],
+        "CaptchaConfig": CaptchaConfigTypeDef,
+        "ChallengeConfig": ChallengeConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+    pass
+
+
 RuleSummaryTypeDef = TypedDict(
     "RuleSummaryTypeDef",
     {
         "Name": str,
-        "Action": RuleActionTypeDef,
+        "Action": RuleActionOutputTypeDef,
     },
     total=False,
 )
 
+DefaultActionUnionTypeDef = Union[DefaultActionTypeDef, DefaultActionOutputTypeDef]
+RuleActionOverrideTypeDef = TypedDict(
+    "RuleActionOverrideTypeDef",
+    {
+        "Name": str,
+        "ActionToUse": RuleActionTypeDef,
+    },
+)
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementTypeDef",
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2405,40 +3037,134 @@
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
+    {
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+_RequiredManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_RequiredManagedRuleGroupStatementOutputTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VendorName": str,
+        "Name": str,
+    },
+)
+_OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_OptionalManagedRuleGroupStatementOutputTypeDef",
+    {
+        "Version": str,
+        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "ScopeDownStatement": "StatementOutputTypeDef",
+        "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ManagedRuleGroupStatementOutputTypeDef(
+    _RequiredManagedRuleGroupStatementOutputTypeDef, _OptionalManagedRuleGroupStatementOutputTypeDef
+):
+    pass
+
+
+_RequiredRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+    },
+)
+_OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class RuleGroupReferenceStatementOutputTypeDef(
+    _RequiredRuleGroupReferenceStatementOutputTypeDef,
+    _OptionalRuleGroupReferenceStatementOutputTypeDef,
+):
+    pass
+
+
+_RequiredRuleGroupTypeDef = TypedDict(
+    "_RequiredRuleGroupTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Capacity": int,
+        "ARN": str,
+        "VisibilityConfig": VisibilityConfigTypeDef,
+    },
+)
+_OptionalRuleGroupTypeDef = TypedDict(
+    "_OptionalRuleGroupTypeDef",
+    {
+        "Description": str,
+        "Rules": List[RuleOutputTypeDef],
+        "LabelNamespace": str,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
+    pass
+
+
+DescribeManagedRuleGroupResponseTypeDef = TypedDict(
+    "DescribeManagedRuleGroupResponseTypeDef",
+    {
+        "VersionName": str,
+        "SnsTopicArn": str,
+        "Capacity": int,
+        "Rules": List[RuleSummaryTypeDef],
+        "LabelNamespace": str,
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
         "VendorName": str,
@@ -2482,33 +3208,82 @@
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
 
-DescribeManagedRuleGroupResponseTypeDef = TypedDict(
-    "DescribeManagedRuleGroupResponseTypeDef",
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
+FirewallManagerStatementTypeDef = TypedDict(
+    "FirewallManagerStatementTypeDef",
     {
-        "VersionName": str,
-        "SnsTopicArn": str,
-        "Capacity": int,
-        "Rules": List[RuleSummaryTypeDef],
-        "LabelNamespace": str,
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
     },
+    total=False,
+)
+
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
+        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
+        "XssMatchStatement": XssMatchStatementOutputTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
+        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementTypeDef,
+        "SqliMatchStatement": SqliMatchStatementTypeDef,
+        "XssMatchStatement": XssMatchStatementTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
+        "GeoMatchStatement": GeoMatchStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementTypeDef,
+    },
+    total=False,
 )
 
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -2517,15 +3292,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
@@ -2544,15 +3319,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -2562,57 +3337,29 @@
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredRuleGroupTypeDef = TypedDict(
-    "_RequiredRuleGroupTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Capacity": int,
-        "ARN": str,
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleGroupTypeDef = TypedDict(
-    "_OptionalRuleGroupTypeDef",
-    {
-        "Description": str,
-        "Rules": List[RuleTypeDef],
-        "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
-    pass
-
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
 class UpdateRuleGroupRequestRequestTypeDef(
@@ -2632,15 +3379,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
@@ -2649,109 +3396,69 @@
 
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
 
-FirewallManagerStatementTypeDef = TypedDict(
-    "FirewallManagerStatementTypeDef",
-    {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-    },
-    total=False,
-)
-
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementTypeDef,
-        "SqliMatchStatement": SqliMatchStatementTypeDef,
-        "XssMatchStatement": XssMatchStatementTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
-        "GeoMatchStatement": GeoMatchStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementTypeDef,
-    },
-    total=False,
-)
-
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
-    {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
-        "OverrideAction": OverrideActionTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
-        "DefaultAction": DefaultActionTypeDef,
+        "DefaultAction": DefaultActionOutputTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
-        "AssociationConfig": AssociationConfigTypeDef,
+        "AssociationConfig": AssociationConfigOutputTypeDef,
     },
     total=False,
 )
 
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "LockToken": str,
         "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2/type_defs.pyi` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_wafv2.type_defs import APIKeySummaryTypeDef
 
-    data: APIKeySummaryTypeDef = {...}
+    data: APIKeySummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -55,38 +55,39 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "APIKeySummaryTypeDef",
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
+    "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    "BlobTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
-    "CheckCapacityResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "LabelNameConditionTypeDef",
+    "CookieMatchPatternOutputTypeDef",
     "CookieMatchPatternTypeDef",
     "CreateAPIKeyRequestRequestTypeDef",
-    "CreateAPIKeyResponseTypeDef",
     "TagTypeDef",
     "IPSetSummaryTypeDef",
     "RegexTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "CustomResponseBodyTypeDef",
     "VisibilityConfigTypeDef",
     "RuleGroupSummaryTypeDef",
     "WebACLSummaryTypeDef",
     "CustomHTTPHeaderTypeDef",
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
     "DescribeAllManagedProductsRequestRequestTypeDef",
@@ -98,34 +99,33 @@
     "EmailFieldTypeDef",
     "ExcludedRuleTypeDef",
     "HeaderOrderTypeDef",
     "SingleHeaderTypeDef",
     "SingleQueryArgumentTypeDef",
     "ForwardedIPConfigTypeDef",
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
     "GetDecryptedAPIKeyRequestRequestTypeDef",
-    "GetDecryptedAPIKeyResponseTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "IPSetTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
-    "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
+    "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
+    "JsonMatchPatternOutputTypeDef",
     "JsonMatchPatternTypeDef",
     "LabelMatchStatementTypeDef",
     "LabelTypeDef",
     "ListAPIKeysRequestRequestTypeDef",
     "ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef",
     "ManagedRuleGroupVersionTypeDef",
     "ListAvailableManagedRuleGroupsRequestRequestTypeDef",
@@ -134,50 +134,66 @@
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListManagedRuleSetsRequestRequestTypeDef",
     "ManagedRuleSetSummaryTypeDef",
     "ListMobileSdkReleasesRequestRequestTypeDef",
     "ReleaseSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "PasswordFieldTypeDef",
     "UsernameFieldTypeDef",
     "ManagedRuleSetVersionTypeDef",
     "NotStatementTypeDef",
+    "OrStatementOutputTypeDef",
     "OrStatementTypeDef",
     "PhoneNumberFieldTypeDef",
     "VersionToPublishTypeDef",
-    "PutManagedRuleSetVersionsResponseTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RateLimitLabelNamespaceTypeDef",
+    "ResponseInspectionBodyContainsOutputTypeDef",
     "ResponseInspectionBodyContainsTypeDef",
+    "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
+    "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
+    "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateIPSetResponseTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
-    "UpdateRegexPatternSetResponseTypeDef",
-    "UpdateRuleGroupResponseTypeDef",
-    "UpdateWebACLResponseTypeDef",
-    "ListAPIKeysResponseTypeDef",
+    "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
+    "RateLimitCookieOutputTypeDef",
     "RateLimitCookieTypeDef",
+    "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
+    "RateLimitQueryArgumentOutputTypeDef",
     "RateLimitQueryArgumentTypeDef",
+    "RateLimitQueryStringOutputTypeDef",
     "RateLimitQueryStringTypeDef",
     "CaptchaConfigTypeDef",
     "ChallengeConfigTypeDef",
+    "CheckCapacityResponseTypeDef",
+    "CreateAPIKeyResponseTypeDef",
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    "GetDecryptedAPIKeyResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "ListAPIKeysResponseTypeDef",
+    "ListResourcesForWebACLResponseTypeDef",
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    "UpdateIPSetResponseTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    "UpdateRegexPatternSetResponseTypeDef",
+    "UpdateRuleGroupResponseTypeDef",
+    "UpdateWebACLResponseTypeDef",
     "ConditionTypeDef",
+    "CookiesOutputTypeDef",
     "CookiesTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "MobileSdkReleaseTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIPSetResponseTypeDef",
     "ListIPSetsResponseTypeDef",
@@ -186,83 +202,125 @@
     "UpdateRegexPatternSetRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "ListRegexPatternSetsResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "ListRuleGroupsResponseTypeDef",
     "CreateWebACLResponseTypeDef",
     "ListWebACLsResponseTypeDef",
+    "CustomRequestHandlingOutputTypeDef",
     "CustomRequestHandlingTypeDef",
+    "CustomResponseOutputTypeDef",
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
+    "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
+    "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     "ListManagedRuleSetsResponseTypeDef",
     "ListMobileSdkReleasesResponseTypeDef",
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
+    "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
+    "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
+    "TimeWindowTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    "AssociationConfigUnionTypeDef",
+    "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
+    "AllowActionOutputTypeDef",
+    "CaptchaActionOutputTypeDef",
+    "ChallengeActionOutputTypeDef",
+    "CountActionOutputTypeDef",
     "AllowActionTypeDef",
     "CaptchaActionTypeDef",
     "ChallengeActionTypeDef",
     "CountActionTypeDef",
+    "BlockActionOutputTypeDef",
     "BlockActionTypeDef",
     "SampledHTTPRequestTypeDef",
+    "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
+    "AWSManagedRulesACFPRuleSetOutputTypeDef",
+    "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
+    "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
+    "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
+    "OverrideActionOutputTypeDef",
     "OverrideActionTypeDef",
+    "DefaultActionOutputTypeDef",
+    "RuleActionOutputTypeDef",
     "DefaultActionTypeDef",
     "RuleActionTypeDef",
     "GetSampledRequestsResponseTypeDef",
+    "ByteMatchStatementOutputTypeDef",
+    "RegexMatchStatementOutputTypeDef",
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    "SizeConstraintStatementOutputTypeDef",
+    "SqliMatchStatementOutputTypeDef",
+    "XssMatchStatementOutputTypeDef",
     "ByteMatchStatementTypeDef",
     "RegexMatchStatementTypeDef",
     "RegexPatternSetReferenceStatementTypeDef",
     "SizeConstraintStatementTypeDef",
     "SqliMatchStatementTypeDef",
     "XssMatchStatementTypeDef",
+    "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "RuleActionOverrideTypeDef",
+    "RuleActionOverrideOutputTypeDef",
+    "RuleOutputTypeDef",
     "RuleSummaryTypeDef",
+    "DefaultActionUnionTypeDef",
+    "RuleActionOverrideTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
+    "ManagedRuleGroupStatementOutputTypeDef",
+    "RuleGroupReferenceStatementOutputTypeDef",
+    "RuleGroupTypeDef",
+    "DescribeManagedRuleGroupResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
-    "DescribeManagedRuleGroupResponseTypeDef",
+    "RuleUnionTypeDef",
+    "FirewallManagerStatementTypeDef",
+    "StatementOutputTypeDef",
+    "GetRuleGroupResponseTypeDef",
+    "StatementTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
-    "RuleGroupTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
-    "FirewallManagerStatementTypeDef",
-    "StatementTypeDef",
-    "GetRuleGroupResponseTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -293,14 +351,21 @@
 AddressFieldTypeDef = TypedDict(
     "AddressFieldTypeDef",
     {
         "Identifier": str,
     },
 )
 
+AndStatementOutputTypeDef = TypedDict(
+    "AndStatementOutputTypeDef",
+    {
+        "Statements": List["StatementOutputTypeDef"],
+    },
+)
+
 AndStatementTypeDef = TypedDict(
     "AndStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
     },
 )
 
@@ -315,14 +380,15 @@
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
@@ -358,29 +424,42 @@
         "ResponseCode": int,
         "SolveTimestamp": int,
         "FailureReason": FailureReasonType,
     },
     total=False,
 )
 
-CheckCapacityResponseTypeDef = TypedDict(
-    "CheckCapacityResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Capacity": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 LabelNameConditionTypeDef = TypedDict(
     "LabelNameConditionTypeDef",
     {
         "LabelName": str,
     },
 )
 
+CookieMatchPatternOutputTypeDef = TypedDict(
+    "CookieMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedCookies": List[str],
+        "ExcludedCookies": List[str],
+    },
+    total=False,
+)
+
 CookieMatchPatternTypeDef = TypedDict(
     "CookieMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedCookies": Sequence[str],
         "ExcludedCookies": Sequence[str],
     },
@@ -391,22 +470,14 @@
     "CreateAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "TokenDomains": Sequence[str],
     },
 )
 
-CreateAPIKeyResponseTypeDef = TypedDict(
-    "CreateAPIKeyResponseTypeDef",
-    {
-        "APIKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -496,22 +567,14 @@
     "DeleteFirewallManagerRuleGroupsRequestRequestTypeDef",
     {
         "WebACLArn": str,
         "WebACLLockToken": str,
     },
 )
 
-DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
-    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
-    {
-        "NextWebACLLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "LockToken": str,
@@ -677,39 +740,22 @@
     "GenerateMobileSdkReleaseUrlRequestRequestTypeDef",
     {
         "Platform": PlatformType,
         "ReleaseVersion": str,
     },
 )
 
-GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
-    "GenerateMobileSdkReleaseUrlResponseTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDecryptedAPIKeyRequestRequestTypeDef = TypedDict(
     "GetDecryptedAPIKeyRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "APIKey": str,
     },
 )
 
-GetDecryptedAPIKeyResponseTypeDef = TypedDict(
-    "GetDecryptedAPIKeyResponseTypeDef",
-    {
-        "TokenDomains": List[str],
-        "CreationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIPSetRequestRequestTypeDef = TypedDict(
     "GetIPSetRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
     },
@@ -763,22 +809,14 @@
 GetPermissionPolicyRequestRequestTypeDef = TypedDict(
     "GetPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetPermissionPolicyResponseTypeDef = TypedDict(
-    "GetPermissionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedStatementManagedKeysRequestRequestTypeDef",
     {
         "Scope": ScopeType,
         "WebACLName": str,
         "WebACLId": str,
         "RuleName": str,
@@ -823,19 +861,19 @@
         "Scope": ScopeType,
         "Id": str,
         "ARN": str,
     },
     total=False,
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
+TimeWindowOutputTypeDef = TypedDict(
+    "TimeWindowOutputTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": datetime,
+        "EndTime": datetime,
     },
 )
 
 GetWebACLForResourceRequestRequestTypeDef = TypedDict(
     "GetWebACLForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -856,14 +894,24 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+HeaderMatchPatternOutputTypeDef = TypedDict(
+    "HeaderMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedHeaders": List[str],
+        "ExcludedHeaders": List[str],
+    },
+    total=False,
+)
+
 HeaderMatchPatternTypeDef = TypedDict(
     "HeaderMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedHeaders": Sequence[str],
         "ExcludedHeaders": Sequence[str],
     },
@@ -875,14 +923,23 @@
     {
         "HeaderName": str,
         "FallbackBehavior": FallbackBehaviorType,
         "Position": ForwardedIPPositionType,
     },
 )
 
+JsonMatchPatternOutputTypeDef = TypedDict(
+    "JsonMatchPatternOutputTypeDef",
+    {
+        "All": Dict[str, Any],
+        "IncludedPaths": List[str],
+    },
+    total=False,
+)
+
 JsonMatchPatternTypeDef = TypedDict(
     "JsonMatchPatternTypeDef",
     {
         "All": Mapping[str, Any],
         "IncludedPaths": Sequence[str],
     },
     total=False,
@@ -1129,22 +1186,14 @@
 
 class ListResourcesForWebACLRequestRequestTypeDef(
     _RequiredListResourcesForWebACLRequestRequestTypeDef,
     _OptionalListResourcesForWebACLRequestRequestTypeDef,
 ):
     pass
 
-ListResourcesForWebACLResponseTypeDef = TypedDict(
-    "ListResourcesForWebACLResponseTypeDef",
-    {
-        "ResourceArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRuleGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListRuleGroupsRequestRequestTypeDef",
     {
         "Scope": ScopeType,
     },
 )
 _OptionalListRuleGroupsRequestRequestTypeDef = TypedDict(
@@ -1228,15 +1277,22 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": Dict[str, Any],
+        "Statement": "StatementTypeDef",
+    },
+)
+
+OrStatementOutputTypeDef = TypedDict(
+    "OrStatementOutputTypeDef",
+    {
+        "Statements": List[Dict[str, Any]],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
         "Statements": Sequence["StatementTypeDef"],
@@ -1255,22 +1311,14 @@
     {
         "AssociatedRuleGroupArn": str,
         "ForecastedLifetime": int,
     },
     total=False,
 )
 
-PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
-    "PutManagedRuleSetVersionsResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutPermissionPolicyRequestRequestTypeDef = TypedDict(
     "PutPermissionPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
@@ -1278,59 +1326,83 @@
 RateLimitLabelNamespaceTypeDef = TypedDict(
     "RateLimitLabelNamespaceTypeDef",
     {
         "Namespace": str,
     },
 )
 
+ResponseInspectionBodyContainsOutputTypeDef = TypedDict(
+    "ResponseInspectionBodyContainsOutputTypeDef",
+    {
+        "SuccessStrings": List[str],
+        "FailureStrings": List[str],
+    },
+)
+
 ResponseInspectionBodyContainsTypeDef = TypedDict(
     "ResponseInspectionBodyContainsTypeDef",
     {
         "SuccessStrings": Sequence[str],
         "FailureStrings": Sequence[str],
     },
 )
 
+ResponseInspectionHeaderOutputTypeDef = TypedDict(
+    "ResponseInspectionHeaderOutputTypeDef",
+    {
+        "Name": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionHeaderTypeDef = TypedDict(
     "ResponseInspectionHeaderTypeDef",
     {
         "Name": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
+ResponseInspectionJsonOutputTypeDef = TypedDict(
+    "ResponseInspectionJsonOutputTypeDef",
+    {
+        "Identifier": str,
+        "SuccessValues": List[str],
+        "FailureValues": List[str],
+    },
+)
+
 ResponseInspectionJsonTypeDef = TypedDict(
     "ResponseInspectionJsonTypeDef",
     {
         "Identifier": str,
         "SuccessValues": Sequence[str],
         "FailureValues": Sequence[str],
     },
 )
 
-ResponseInspectionStatusCodeTypeDef = TypedDict(
-    "ResponseInspectionStatusCodeTypeDef",
+ResponseInspectionStatusCodeOutputTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeOutputTypeDef",
     {
-        "SuccessCodes": Sequence[int],
-        "FailureCodes": Sequence[int],
+        "SuccessCodes": List[int],
+        "FailureCodes": List[int],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ResponseInspectionStatusCodeTypeDef = TypedDict(
+    "ResponseInspectionStatusCodeTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SuccessCodes": Sequence[int],
+        "FailureCodes": Sequence[int],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1354,112 +1426,87 @@
 )
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Scope": ScopeType,
-        "Id": str,
-        "LockToken": str,
-        "VersionToExpire": str,
-        "ExpiryTimestamp": Union[datetime, str],
-    },
-)
-
-UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+AssociationConfigOutputTypeDef = TypedDict(
+    "AssociationConfigOutputTypeDef",
     {
-        "ExpiringVersion": str,
-        "ExpiryTimestamp": datetime,
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
-    {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
     },
+    total=False,
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+AssociationConfigTypeDef = TypedDict(
+    "AssociationConfigTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestBody": Mapping[
+            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
+        ],
     },
+    total=False,
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+RateLimitCookieOutputTypeDef = TypedDict(
+    "RateLimitCookieOutputTypeDef",
     {
-        "NextLockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
-ListAPIKeysResponseTypeDef = TypedDict(
-    "ListAPIKeysResponseTypeDef",
+RateLimitCookieTypeDef = TypedDict(
+    "RateLimitCookieTypeDef",
     {
-        "NextMarker": str,
-        "APIKeySummaries": List[APIKeySummaryTypeDef],
-        "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-AssociationConfigTypeDef = TypedDict(
-    "AssociationConfigTypeDef",
+RateLimitHeaderOutputTypeDef = TypedDict(
+    "RateLimitHeaderOutputTypeDef",
     {
-        "RequestBody": Mapping[
-            Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef
-        ],
+        "Name": str,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
-    total=False,
 )
 
-RateLimitCookieTypeDef = TypedDict(
-    "RateLimitCookieTypeDef",
+RateLimitHeaderTypeDef = TypedDict(
+    "RateLimitHeaderTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
-RateLimitHeaderTypeDef = TypedDict(
-    "RateLimitHeaderTypeDef",
+RateLimitQueryArgumentOutputTypeDef = TypedDict(
+    "RateLimitQueryArgumentOutputTypeDef",
     {
         "Name": str,
-        "TextTransformations": Sequence[TextTransformationTypeDef],
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 RateLimitQueryArgumentTypeDef = TypedDict(
     "RateLimitQueryArgumentTypeDef",
     {
         "Name": str,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+RateLimitQueryStringOutputTypeDef = TypedDict(
+    "RateLimitQueryStringOutputTypeDef",
+    {
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
 RateLimitQueryStringTypeDef = TypedDict(
     "RateLimitQueryStringTypeDef",
     {
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
@@ -1475,23 +1522,149 @@
     "ChallengeConfigTypeDef",
     {
         "ImmunityTimeProperty": ImmunityTimePropertyTypeDef,
     },
     total=False,
 )
 
+CheckCapacityResponseTypeDef = TypedDict(
+    "CheckCapacityResponseTypeDef",
+    {
+        "Capacity": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAPIKeyResponseTypeDef = TypedDict(
+    "CreateAPIKeyResponseTypeDef",
+    {
+        "APIKey": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFirewallManagerRuleGroupsResponseTypeDef = TypedDict(
+    "DeleteFirewallManagerRuleGroupsResponseTypeDef",
+    {
+        "NextWebACLLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMobileSdkReleaseUrlResponseTypeDef = TypedDict(
+    "GenerateMobileSdkReleaseUrlResponseTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecryptedAPIKeyResponseTypeDef = TypedDict(
+    "GetDecryptedAPIKeyResponseTypeDef",
+    {
+        "TokenDomains": List[str],
+        "CreationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAPIKeysResponseTypeDef = TypedDict(
+    "ListAPIKeysResponseTypeDef",
+    {
+        "NextMarker": str,
+        "APIKeySummaries": List[APIKeySummaryTypeDef],
+        "ApplicationIntegrationURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
+    {
+        "ResourceArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutManagedRuleSetVersionsResponseTypeDef = TypedDict(
+    "PutManagedRuleSetVersionsResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateResponseTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateResponseTypeDef",
+    {
+        "ExpiringVersion": str,
+        "ExpiryTimestamp": datetime,
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "NextLockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ActionCondition": ActionConditionTypeDef,
         "LabelNameCondition": LabelNameConditionTypeDef,
     },
     total=False,
 )
 
+CookiesOutputTypeDef = TypedDict(
+    "CookiesOutputTypeDef",
+    {
+        "MatchPattern": CookieMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 CookiesTypeDef = TypedDict(
     "CookiesTypeDef",
     {
         "MatchPattern": CookieMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1548,24 +1721,24 @@
     },
 )
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "Summary": IPSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIPSetsResponseTypeDef = TypedDict(
     "ListIPSetsResponseTypeDef",
     {
         "NextMarker": str,
         "IPSets": List[IPSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRegexPatternSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegexPatternSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -1624,68 +1797,95 @@
 ):
     pass
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "Summary": RegexPatternSetSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexPatternSetsResponseTypeDef = TypedDict(
     "ListRegexPatternSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexPatternSets": List[RegexPatternSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "Summary": RuleGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "Summary": WebACLSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebACLsResponseTypeDef = TypedDict(
     "ListWebACLsResponseTypeDef",
     {
         "NextMarker": str,
         "WebACLs": List[WebACLSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomRequestHandlingOutputTypeDef = TypedDict(
+    "CustomRequestHandlingOutputTypeDef",
+    {
+        "InsertHeaders": List[CustomHTTPHeaderTypeDef],
     },
 )
 
 CustomRequestHandlingTypeDef = TypedDict(
     "CustomRequestHandlingTypeDef",
     {
         "InsertHeaders": Sequence[CustomHTTPHeaderTypeDef],
     },
 )
 
+_RequiredCustomResponseOutputTypeDef = TypedDict(
+    "_RequiredCustomResponseOutputTypeDef",
+    {
+        "ResponseCode": int,
+    },
+)
+_OptionalCustomResponseOutputTypeDef = TypedDict(
+    "_OptionalCustomResponseOutputTypeDef",
+    {
+        "CustomResponseBodyKey": str,
+        "ResponseHeaders": List[CustomHTTPHeaderTypeDef],
+    },
+    total=False,
+)
+
+class CustomResponseOutputTypeDef(
+    _RequiredCustomResponseOutputTypeDef, _OptionalCustomResponseOutputTypeDef
+):
+    pass
+
 _RequiredCustomResponseTypeDef = TypedDict(
     "_RequiredCustomResponseTypeDef",
     {
         "ResponseCode": int,
     },
 )
 _OptionalCustomResponseTypeDef = TypedDict(
@@ -1700,24 +1900,33 @@
 class CustomResponseTypeDef(_RequiredCustomResponseTypeDef, _OptionalCustomResponseTypeDef):
     pass
 
 DescribeAllManagedProductsResponseTypeDef = TypedDict(
     "DescribeAllManagedProductsResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeManagedProductsByVendorResponseTypeDef = TypedDict(
     "DescribeManagedProductsByVendorResponseTypeDef",
     {
         "ManagedProducts": List[ManagedProductDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GeoMatchStatementOutputTypeDef = TypedDict(
+    "GeoMatchStatementOutputTypeDef",
+    {
+        "CountryCodes": List[CountryCodeType],
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
     },
+    total=False,
 )
 
 GeoMatchStatementTypeDef = TypedDict(
     "GeoMatchStatementTypeDef",
     {
         "CountryCodes": Sequence[CountryCodeType],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
@@ -1726,35 +1935,24 @@
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedStatementManagedKeysResponseTypeDef = TypedDict(
     "GetRateBasedStatementManagedKeysResponseTypeDef",
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclArn": str,
-        "RuleMetricName": str,
-        "Scope": ScopeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1763,14 +1961,23 @@
         "Method": str,
         "HTTPVersion": str,
         "Headers": List[HTTPHeaderTypeDef],
     },
     total=False,
 )
 
+HeadersOutputTypeDef = TypedDict(
+    "HeadersOutputTypeDef",
+    {
+        "MatchPattern": HeaderMatchPatternOutputTypeDef,
+        "MatchScope": MapMatchScopeType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+)
+
 HeadersTypeDef = TypedDict(
     "HeadersTypeDef",
     {
         "MatchPattern": HeaderMatchPatternTypeDef,
         "MatchScope": MapMatchScopeType,
         "OversizeHandling": OversizeHandlingType,
     },
@@ -1791,14 +1998,33 @@
 )
 
 class IPSetReferenceStatementTypeDef(
     _RequiredIPSetReferenceStatementTypeDef, _OptionalIPSetReferenceStatementTypeDef
 ):
     pass
 
+_RequiredJsonBodyOutputTypeDef = TypedDict(
+    "_RequiredJsonBodyOutputTypeDef",
+    {
+        "MatchPattern": JsonMatchPatternOutputTypeDef,
+        "MatchScope": JsonMatchScopeType,
+    },
+)
+_OptionalJsonBodyOutputTypeDef = TypedDict(
+    "_OptionalJsonBodyOutputTypeDef",
+    {
+        "InvalidFallbackBehavior": BodyParsingFallbackBehaviorType,
+        "OversizeHandling": OversizeHandlingType,
+    },
+    total=False,
+)
+
+class JsonBodyOutputTypeDef(_RequiredJsonBodyOutputTypeDef, _OptionalJsonBodyOutputTypeDef):
+    pass
+
 _RequiredJsonBodyTypeDef = TypedDict(
     "_RequiredJsonBodyTypeDef",
     {
         "MatchPattern": JsonMatchPatternTypeDef,
         "MatchScope": JsonMatchScopeType,
     },
 )
@@ -1816,42 +2042,42 @@
 
 ListAvailableManagedRuleGroupVersionsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[ManagedRuleGroupVersionTypeDef],
         "CurrentDefaultVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableManagedRuleGroupsResponseTypeDef = TypedDict(
     "ListAvailableManagedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleGroups": List[ManagedRuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedRuleSetsResponseTypeDef = TypedDict(
     "ListManagedRuleSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ManagedRuleSets": List[ManagedRuleSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMobileSdkReleasesResponseTypeDef = TypedDict(
     "ListMobileSdkReleasesResponseTypeDef",
     {
         "ReleaseSummaries": List[ReleaseSummaryTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestInspectionTypeDef = TypedDict(
     "RequestInspectionTypeDef",
     {
         "PayloadType": PayloadTypeType,
@@ -1878,14 +2104,37 @@
     },
     total=False,
 )
 
 class ManagedRuleSetTypeDef(_RequiredManagedRuleSetTypeDef, _OptionalManagedRuleSetTypeDef):
     pass
 
+_RequiredRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_RequiredRequestInspectionACFPOutputTypeDef",
+    {
+        "PayloadType": PayloadTypeType,
+    },
+)
+_OptionalRequestInspectionACFPOutputTypeDef = TypedDict(
+    "_OptionalRequestInspectionACFPOutputTypeDef",
+    {
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "EmailField": EmailFieldTypeDef,
+        "PhoneNumberFields": List[PhoneNumberFieldTypeDef],
+        "AddressFields": List[AddressFieldTypeDef],
+    },
+    total=False,
+)
+
+class RequestInspectionACFPOutputTypeDef(
+    _RequiredRequestInspectionACFPOutputTypeDef, _OptionalRequestInspectionACFPOutputTypeDef
+):
+    pass
+
 _RequiredRequestInspectionACFPTypeDef = TypedDict(
     "_RequiredRequestInspectionACFPTypeDef",
     {
         "PayloadType": PayloadTypeType,
     },
 )
 _OptionalRequestInspectionACFPTypeDef = TypedDict(
@@ -1925,25 +2174,72 @@
 
 class PutManagedRuleSetVersionsRequestRequestTypeDef(
     _RequiredPutManagedRuleSetVersionsRequestRequestTypeDef,
     _OptionalPutManagedRuleSetVersionsRequestRequestTypeDef,
 ):
     pass
 
+ResponseInspectionOutputTypeDef = TypedDict(
+    "ResponseInspectionOutputTypeDef",
+    {
+        "StatusCode": ResponseInspectionStatusCodeOutputTypeDef,
+        "Header": ResponseInspectionHeaderOutputTypeDef,
+        "BodyContains": ResponseInspectionBodyContainsOutputTypeDef,
+        "Json": ResponseInspectionJsonOutputTypeDef,
+    },
+    total=False,
+)
+
 ResponseInspectionTypeDef = TypedDict(
     "ResponseInspectionTypeDef",
     {
         "StatusCode": ResponseInspectionStatusCodeTypeDef,
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Scope": ScopeType,
+        "Id": str,
+        "LockToken": str,
+        "VersionToExpire": str,
+        "ExpiryTimestamp": TimestampTypeDef,
+    },
+)
+
+AssociationConfigUnionTypeDef = Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef]
+RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
+    "RateBasedStatementCustomKeyOutputTypeDef",
+    {
+        "Header": RateLimitHeaderOutputTypeDef,
+        "Cookie": RateLimitCookieOutputTypeDef,
+        "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
+        "QueryString": RateLimitQueryStringOutputTypeDef,
+        "HTTPMethod": Dict[str, Any],
+        "ForwardedIP": Dict[str, Any],
+        "IP": Dict[str, Any],
+        "LabelNamespace": RateLimitLabelNamespaceTypeDef,
+    },
+    total=False,
+)
+
 RateBasedStatementCustomKeyTypeDef = TypedDict(
     "RateBasedStatementCustomKeyTypeDef",
     {
         "Header": RateLimitHeaderTypeDef,
         "Cookie": RateLimitCookieTypeDef,
         "QueryArgument": RateLimitQueryArgumentTypeDef,
         "QueryString": RateLimitQueryStringTypeDef,
@@ -1951,47 +2247,88 @@
         "ForwardedIP": Mapping[str, Any],
         "IP": Mapping[str, Any],
         "LabelNamespace": RateLimitLabelNamespaceTypeDef,
     },
     total=False,
 )
 
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "Behavior": FilterBehaviorType,
+        "Requirement": FilterRequirementType,
+        "Conditions": List[ConditionTypeDef],
+    },
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Behavior": FilterBehaviorType,
         "Requirement": FilterRequirementType,
-        "Conditions": List[ConditionTypeDef],
+        "Conditions": Sequence[ConditionTypeDef],
     },
 )
 
 GetMobileSdkReleaseResponseTypeDef = TypedDict(
     "GetMobileSdkReleaseResponseTypeDef",
     {
         "MobileSdkRelease": MobileSdkReleaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "NextMarker": str,
         "TagInfoForResource": TagInfoForResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AllowActionOutputTypeDef = TypedDict(
+    "AllowActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
+)
+
+CaptchaActionOutputTypeDef = TypedDict(
+    "CaptchaActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
     },
+    total=False,
+)
+
+ChallengeActionOutputTypeDef = TypedDict(
+    "ChallengeActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
+)
+
+CountActionOutputTypeDef = TypedDict(
+    "CountActionOutputTypeDef",
+    {
+        "CustomRequestHandling": CustomRequestHandlingOutputTypeDef,
+    },
+    total=False,
 )
 
 AllowActionTypeDef = TypedDict(
     "AllowActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
@@ -2018,14 +2355,22 @@
     "CountActionTypeDef",
     {
         "CustomRequestHandling": CustomRequestHandlingTypeDef,
     },
     total=False,
 )
 
+BlockActionOutputTypeDef = TypedDict(
+    "BlockActionOutputTypeDef",
+    {
+        "CustomResponse": CustomResponseOutputTypeDef,
+    },
+    total=False,
+)
+
 BlockActionTypeDef = TypedDict(
     "BlockActionTypeDef",
     {
         "CustomResponse": CustomResponseTypeDef,
     },
     total=False,
 )
@@ -2054,14 +2399,32 @@
 )
 
 class SampledHTTPRequestTypeDef(
     _RequiredSampledHTTPRequestTypeDef, _OptionalSampledHTTPRequestTypeDef
 ):
     pass
 
+FieldToMatchOutputTypeDef = TypedDict(
+    "FieldToMatchOutputTypeDef",
+    {
+        "SingleHeader": SingleHeaderTypeDef,
+        "SingleQueryArgument": SingleQueryArgumentTypeDef,
+        "AllQueryArguments": Dict[str, Any],
+        "UriPath": Dict[str, Any],
+        "QueryString": Dict[str, Any],
+        "Body": BodyTypeDef,
+        "Method": Dict[str, Any],
+        "JsonBody": JsonBodyOutputTypeDef,
+        "Headers": HeadersOutputTypeDef,
+        "Cookies": CookiesOutputTypeDef,
+        "HeaderOrder": HeaderOrderTypeDef,
+    },
+    total=False,
+)
+
 FieldToMatchTypeDef = TypedDict(
     "FieldToMatchTypeDef",
     {
         "SingleHeader": SingleHeaderTypeDef,
         "SingleQueryArgument": SingleQueryArgumentTypeDef,
         "AllQueryArguments": Mapping[str, Any],
         "UriPath": Mapping[str, Any],
@@ -2077,17 +2440,61 @@
 )
 
 GetManagedRuleSetResponseTypeDef = TypedDict(
     "GetManagedRuleSetResponseTypeDef",
     {
         "ManagedRuleSet": ManagedRuleSetTypeDef,
         "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "CreationPath": str,
+        "RegistrationPagePath": str,
+        "RequestInspection": RequestInspectionACFPOutputTypeDef,
+    },
+)
+_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesACFPRuleSetOutputTypeDef",
+    {
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
+    },
+    total=False,
+)
+
+class AWSManagedRulesACFPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesACFPRuleSetOutputTypeDef,
+    _OptionalAWSManagedRulesACFPRuleSetOutputTypeDef,
+):
+    pass
+
+_RequiredAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_RequiredAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "LoginPath": str,
     },
 )
+_OptionalAWSManagedRulesATPRuleSetOutputTypeDef = TypedDict(
+    "_OptionalAWSManagedRulesATPRuleSetOutputTypeDef",
+    {
+        "RequestInspection": RequestInspectionTypeDef,
+        "ResponseInspection": ResponseInspectionOutputTypeDef,
+        "EnableRegexInPath": bool,
+    },
+    total=False,
+)
+
+class AWSManagedRulesATPRuleSetOutputTypeDef(
+    _RequiredAWSManagedRulesATPRuleSetOutputTypeDef, _OptionalAWSManagedRulesATPRuleSetOutputTypeDef
+):
+    pass
 
 _RequiredAWSManagedRulesACFPRuleSetTypeDef = TypedDict(
     "_RequiredAWSManagedRulesACFPRuleSetTypeDef",
     {
         "CreationPath": str,
         "RegistrationPagePath": str,
         "RequestInspection": RequestInspectionACFPTypeDef,
@@ -2124,53 +2531,125 @@
 )
 
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
+    {
+        "WebAclArn": str,
+        "RuleMetricName": str,
+        "Scope": ScopeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
+    },
+)
+
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
+_RequiredRateBasedStatementOutputTypeDef = TypedDict(
+    "_RequiredRateBasedStatementOutputTypeDef",
+    {
+        "Limit": int,
+        "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
+    },
+)
+_OptionalRateBasedStatementOutputTypeDef = TypedDict(
+    "_OptionalRateBasedStatementOutputTypeDef",
+    {
+        "ScopeDownStatement": "StatementOutputTypeDef",
+        "ForwardedIPConfig": ForwardedIPConfigTypeDef,
+        "CustomKeys": List[RateBasedStatementCustomKeyOutputTypeDef],
+    },
+    total=False,
+)
+
+class RateBasedStatementOutputTypeDef(
+    _RequiredRateBasedStatementOutputTypeDef, _OptionalRateBasedStatementOutputTypeDef
+):
+    pass
+
 _RequiredRateBasedStatementTypeDef = TypedDict(
     "_RequiredRateBasedStatementTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
 _OptionalRateBasedStatementTypeDef = TypedDict(
     "_OptionalRateBasedStatementTypeDef",
     {
-        "ScopeDownStatement": "StatementTypeDef",
+        "ScopeDownStatement": Dict[str, Any],
         "ForwardedIPConfig": ForwardedIPConfigTypeDef,
         "CustomKeys": Sequence[RateBasedStatementCustomKeyTypeDef],
     },
     total=False,
 )
 
 class RateBasedStatementTypeDef(
     _RequiredRateBasedStatementTypeDef, _OptionalRateBasedStatementTypeDef
 ):
     pass
 
+LoggingFilterOutputTypeDef = TypedDict(
+    "LoggingFilterOutputTypeDef",
+    {
+        "Filters": List[FilterOutputTypeDef],
+        "DefaultBehavior": FilterBehaviorType,
+    },
+)
+
 LoggingFilterTypeDef = TypedDict(
     "LoggingFilterTypeDef",
     {
-        "Filters": List[FilterTypeDef],
+        "Filters": Sequence[FilterTypeDef],
         "DefaultBehavior": FilterBehaviorType,
     },
 )
 
+OverrideActionOutputTypeDef = TypedDict(
+    "OverrideActionOutputTypeDef",
+    {
+        "Count": CountActionOutputTypeDef,
+        "None": Dict[str, Any],
+    },
+    total=False,
+)
+
 OverrideActionTypeDef = TypedDict(
     "OverrideActionTypeDef",
     {
         "Count": CountActionTypeDef,
         "None": Mapping[str, Any],
     },
     total=False,
 )
 
+DefaultActionOutputTypeDef = TypedDict(
+    "DefaultActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+    },
+    total=False,
+)
+
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "Block": BlockActionOutputTypeDef,
+        "Allow": AllowActionOutputTypeDef,
+        "Count": CountActionOutputTypeDef,
+        "Captcha": CaptchaActionOutputTypeDef,
+        "Challenge": ChallengeActionOutputTypeDef,
+    },
+    total=False,
+)
+
 DefaultActionTypeDef = TypedDict(
     "DefaultActionTypeDef",
     {
         "Block": BlockActionTypeDef,
         "Allow": AllowActionTypeDef,
     },
     total=False,
@@ -2189,23 +2668,89 @@
 )
 
 GetSampledRequestsResponseTypeDef = TypedDict(
     "GetSampledRequestsResponseTypeDef",
     {
         "SampledRequests": List[SampledHTTPRequestTypeDef],
         "PopulationSize": int,
-        "TimeWindow": TimeWindowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeWindow": TimeWindowOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ByteMatchStatementOutputTypeDef = TypedDict(
+    "ByteMatchStatementOutputTypeDef",
+    {
+        "SearchString": bytes,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
+RegexMatchStatementOutputTypeDef = TypedDict(
+    "RegexMatchStatementOutputTypeDef",
+    {
+        "RegexString": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
+RegexPatternSetReferenceStatementOutputTypeDef = TypedDict(
+    "RegexPatternSetReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
+SizeConstraintStatementOutputTypeDef = TypedDict(
+    "SizeConstraintStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+
+_RequiredSqliMatchStatementOutputTypeDef = TypedDict(
+    "_RequiredSqliMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
+    },
+)
+_OptionalSqliMatchStatementOutputTypeDef = TypedDict(
+    "_OptionalSqliMatchStatementOutputTypeDef",
+    {
+        "SensitivityLevel": SensitivityLevelType,
+    },
+    total=False,
+)
+
+class SqliMatchStatementOutputTypeDef(
+    _RequiredSqliMatchStatementOutputTypeDef, _OptionalSqliMatchStatementOutputTypeDef
+):
+    pass
+
+XssMatchStatementOutputTypeDef = TypedDict(
+    "XssMatchStatementOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchOutputTypeDef,
+        "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
-        "SearchString": Union[str, bytes, IO[Any], StreamingBody],
+        "SearchString": BlobTypeDef,
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 RegexMatchStatementTypeDef = TypedDict(
@@ -2260,67 +2805,136 @@
     "XssMatchStatementTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
     },
 )
 
+ManagedRuleGroupConfigOutputTypeDef = TypedDict(
+    "ManagedRuleGroupConfigOutputTypeDef",
+    {
+        "LoginPath": str,
+        "PayloadType": PayloadTypeType,
+        "UsernameField": UsernameFieldTypeDef,
+        "PasswordField": PasswordFieldTypeDef,
+        "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
+        "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetOutputTypeDef,
+        "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagedRuleGroupConfigTypeDef = TypedDict(
     "ManagedRuleGroupConfigTypeDef",
     {
         "LoginPath": str,
         "PayloadType": PayloadTypeType,
         "UsernameField": UsernameFieldTypeDef,
         "PasswordField": PasswordFieldTypeDef,
         "AWSManagedRulesBotControlRuleSet": AWSManagedRulesBotControlRuleSetTypeDef,
         "AWSManagedRulesATPRuleSet": AWSManagedRulesATPRuleSetTypeDef,
         "AWSManagedRulesACFPRuleSet": AWSManagedRulesACFPRuleSetTypeDef,
     },
     total=False,
 )
 
+_RequiredLoggingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "LogDestinationConfigs": List[str],
+    },
+)
+_OptionalLoggingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationOutputTypeDef",
+    {
+        "RedactedFields": List[FieldToMatchOutputTypeDef],
+        "ManagedByFirewallManager": bool,
+        "LoggingFilter": LoggingFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredLoggingConfigurationTypeDef = TypedDict(
     "_RequiredLoggingConfigurationTypeDef",
     {
         "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
+        "LogDestinationConfigs": Sequence[str],
     },
 )
 _OptionalLoggingConfigurationTypeDef = TypedDict(
     "_OptionalLoggingConfigurationTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "RedactedFields": Sequence[FieldToMatchTypeDef],
         "ManagedByFirewallManager": bool,
         "LoggingFilter": LoggingFilterTypeDef,
     },
     total=False,
 )
 
 class LoggingConfigurationTypeDef(
     _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
 ):
     pass
 
-RuleActionOverrideTypeDef = TypedDict(
-    "RuleActionOverrideTypeDef",
+RuleActionOverrideOutputTypeDef = TypedDict(
+    "RuleActionOverrideOutputTypeDef",
     {
         "Name": str,
-        "ActionToUse": RuleActionTypeDef,
+        "ActionToUse": RuleActionOutputTypeDef,
+    },
+)
+
+_RequiredRuleOutputTypeDef = TypedDict(
+    "_RequiredRuleOutputTypeDef",
+    {
+        "Name": str,
+        "Priority": int,
+        "Statement": "StatementOutputTypeDef",
+        "VisibilityConfig": VisibilityConfigTypeDef,
+    },
+)
+_OptionalRuleOutputTypeDef = TypedDict(
+    "_OptionalRuleOutputTypeDef",
+    {
+        "Action": RuleActionOutputTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
+        "RuleLabels": List[LabelTypeDef],
+        "CaptchaConfig": CaptchaConfigTypeDef,
+        "ChallengeConfig": ChallengeConfigTypeDef,
     },
+    total=False,
 )
 
+class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
+    pass
+
 RuleSummaryTypeDef = TypedDict(
     "RuleSummaryTypeDef",
     {
         "Name": str,
-        "Action": RuleActionTypeDef,
+        "Action": RuleActionOutputTypeDef,
     },
     total=False,
 )
 
+DefaultActionUnionTypeDef = Union[DefaultActionTypeDef, DefaultActionOutputTypeDef]
+RuleActionOverrideTypeDef = TypedDict(
+    "RuleActionOverrideTypeDef",
+    {
+        "Name": str,
+        "ActionToUse": RuleActionTypeDef,
+    },
+)
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "Priority": int,
         "Statement": "StatementTypeDef",
         "VisibilityConfig": VisibilityConfigTypeDef,
@@ -2340,40 +2954,128 @@
 
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
-        "LoggingConfigurations": List[LoggingConfigurationTypeDef],
+        "LoggingConfigurations": List[LoggingConfigurationOutputTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
+    {
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+_RequiredManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_RequiredManagedRuleGroupStatementOutputTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VendorName": str,
+        "Name": str,
+    },
+)
+_OptionalManagedRuleGroupStatementOutputTypeDef = TypedDict(
+    "_OptionalManagedRuleGroupStatementOutputTypeDef",
+    {
+        "Version": str,
+        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "ScopeDownStatement": "StatementOutputTypeDef",
+        "ManagedRuleGroupConfigs": List[ManagedRuleGroupConfigOutputTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+class ManagedRuleGroupStatementOutputTypeDef(
+    _RequiredManagedRuleGroupStatementOutputTypeDef, _OptionalManagedRuleGroupStatementOutputTypeDef
+):
+    pass
+
+_RequiredRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_RequiredRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ARN": str,
+    },
+)
+_OptionalRuleGroupReferenceStatementOutputTypeDef = TypedDict(
+    "_OptionalRuleGroupReferenceStatementOutputTypeDef",
+    {
+        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "RuleActionOverrides": List[RuleActionOverrideOutputTypeDef],
+    },
+    total=False,
+)
+
+class RuleGroupReferenceStatementOutputTypeDef(
+    _RequiredRuleGroupReferenceStatementOutputTypeDef,
+    _OptionalRuleGroupReferenceStatementOutputTypeDef,
+):
+    pass
+
+_RequiredRuleGroupTypeDef = TypedDict(
+    "_RequiredRuleGroupTypeDef",
+    {
+        "Name": str,
+        "Id": str,
+        "Capacity": int,
+        "ARN": str,
+        "VisibilityConfig": VisibilityConfigTypeDef,
+    },
+)
+_OptionalRuleGroupTypeDef = TypedDict(
+    "_OptionalRuleGroupTypeDef",
+    {
+        "Description": str,
+        "Rules": List[RuleOutputTypeDef],
+        "LabelNamespace": str,
+        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+    },
+    total=False,
+)
+
+class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
+    pass
+
+DescribeManagedRuleGroupResponseTypeDef = TypedDict(
+    "DescribeManagedRuleGroupResponseTypeDef",
+    {
+        "VersionName": str,
+        "SnsTopicArn": str,
+        "Capacity": int,
+        "Rules": List[RuleSummaryTypeDef],
+        "LabelNamespace": str,
+        "AvailableLabels": List[LabelSummaryTypeDef],
+        "ConsumedLabels": List[LabelSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleGroupStatementTypeDef = TypedDict(
     "_RequiredManagedRuleGroupStatementTypeDef",
     {
         "VendorName": str,
@@ -2413,33 +3115,82 @@
 )
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
-DescribeManagedRuleGroupResponseTypeDef = TypedDict(
-    "DescribeManagedRuleGroupResponseTypeDef",
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
+FirewallManagerStatementTypeDef = TypedDict(
+    "FirewallManagerStatementTypeDef",
     {
-        "VersionName": str,
-        "SnsTopicArn": str,
-        "Capacity": int,
-        "Rules": List[RuleSummaryTypeDef],
-        "LabelNamespace": str,
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
     },
+    total=False,
+)
+
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
+        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
+        "XssMatchStatement": XssMatchStatementOutputTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
+        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementTypeDef,
+        "SqliMatchStatement": SqliMatchStatementTypeDef,
+        "XssMatchStatement": XssMatchStatementTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
+        "GeoMatchStatement": GeoMatchStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementTypeDef,
+    },
+    total=False,
 )
 
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -2448,15 +3199,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
@@ -2473,15 +3224,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -2489,55 +3240,29 @@
 )
 
 class CreateWebACLRequestRequestTypeDef(
     _RequiredCreateWebACLRequestRequestTypeDef, _OptionalCreateWebACLRequestRequestTypeDef
 ):
     pass
 
-_RequiredRuleGroupTypeDef = TypedDict(
-    "_RequiredRuleGroupTypeDef",
-    {
-        "Name": str,
-        "Id": str,
-        "Capacity": int,
-        "ARN": str,
-        "VisibilityConfig": VisibilityConfigTypeDef,
-    },
-)
-_OptionalRuleGroupTypeDef = TypedDict(
-    "_OptionalRuleGroupTypeDef",
-    {
-        "Description": str,
-        "Rules": List[RuleTypeDef],
-        "LabelNamespace": str,
-        "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
-        "AvailableLabels": List[LabelSummaryTypeDef],
-        "ConsumedLabels": List[LabelSummaryTypeDef],
-    },
-    total=False,
-)
-
-class RuleGroupTypeDef(_RequiredRuleGroupTypeDef, _OptionalRuleGroupTypeDef):
-    pass
-
 _RequiredUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
         "Scope": ScopeType,
         "Id": str,
         "VisibilityConfig": VisibilityConfigTypeDef,
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
@@ -2555,122 +3280,82 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
-FirewallManagerStatementTypeDef = TypedDict(
-    "FirewallManagerStatementTypeDef",
-    {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-    },
-    total=False,
-)
-
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementTypeDef,
-        "SqliMatchStatement": SqliMatchStatementTypeDef,
-        "XssMatchStatement": XssMatchStatementTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
-        "GeoMatchStatement": GeoMatchStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementTypeDef,
-    },
-    total=False,
-)
-
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
-    {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
-        "OverrideAction": OverrideActionTypeDef,
+        "OverrideAction": OverrideActionOutputTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "Name": str,
         "Id": str,
         "ARN": str,
-        "DefaultAction": DefaultActionTypeDef,
+        "DefaultAction": DefaultActionOutputTypeDef,
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Description": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "Capacity": int,
         "PreProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "PostProcessFirewallManagerRuleGroups": List[FirewallManagerRuleGroupTypeDef],
         "ManagedByFirewallManager": bool,
         "LabelNamespace": str,
         "CustomResponseBodies": Dict[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": List[str],
-        "AssociationConfig": AssociationConfigTypeDef,
+        "AssociationConfig": AssociationConfigOutputTypeDef,
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "LockToken": str,
         "ApplicationIntegrationURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/PKG-INFO` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wafv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WAFV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore wafv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-wafv2"></a>
 
 # types-aiobotocore-wafv2
 
 [![PyPI - types-aiobotocore-wafv2](https://img.shields.io/pypi/v/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wafv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wafv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wafv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-wafv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wafv2)](https://pepy.tech/project/types-aiobotocore-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAFV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [types-aiobotocore-wafv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -304,51 +303,52 @@
 )
 
 
 def check_value(value: ActionValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wafv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wafv2.type_defs import (
     APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
     AddressFieldTypeDef,
+    AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BlobTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
-    CheckCapacityResponseTypeDef,
+    ResponseMetadataTypeDef,
     LabelNameConditionTypeDef,
+    CookieMatchPatternOutputTypeDef,
     CookieMatchPatternTypeDef,
     CreateAPIKeyRequestRequestTypeDef,
-    CreateAPIKeyResponseTypeDef,
     TagTypeDef,
     IPSetSummaryTypeDef,
     RegexTypeDef,
     RegexPatternSetSummaryTypeDef,
     CustomResponseBodyTypeDef,
     VisibilityConfigTypeDef,
     RuleGroupSummaryTypeDef,
     WebACLSummaryTypeDef,
     CustomHTTPHeaderTypeDef,
     DeleteFirewallManagerRuleGroupsRequestRequestTypeDef,
-    DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
     DeleteWebACLRequestRequestTypeDef,
     DescribeAllManagedProductsRequestRequestTypeDef,
@@ -360,34 +360,33 @@
     EmailFieldTypeDef,
     ExcludedRuleTypeDef,
     HeaderOrderTypeDef,
     SingleHeaderTypeDef,
     SingleQueryArgumentTypeDef,
     ForwardedIPConfigTypeDef,
     GenerateMobileSdkReleaseUrlRequestRequestTypeDef,
-    GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyRequestRequestTypeDef,
-    GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetRequestRequestTypeDef,
     IPSetTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
+    HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
+    JsonMatchPatternOutputTypeDef,
     JsonMatchPatternTypeDef,
     LabelMatchStatementTypeDef,
     LabelTypeDef,
     ListAPIKeysRequestRequestTypeDef,
     ListAvailableManagedRuleGroupVersionsRequestRequestTypeDef,
     ManagedRuleGroupVersionTypeDef,
     ListAvailableManagedRuleGroupsRequestRequestTypeDef,
@@ -396,50 +395,66 @@
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListManagedRuleSetsRequestRequestTypeDef,
     ManagedRuleSetSummaryTypeDef,
     ListMobileSdkReleasesRequestRequestTypeDef,
     ReleaseSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     PasswordFieldTypeDef,
     UsernameFieldTypeDef,
     ManagedRuleSetVersionTypeDef,
     NotStatementTypeDef,
+    OrStatementOutputTypeDef,
     OrStatementTypeDef,
     PhoneNumberFieldTypeDef,
     VersionToPublishTypeDef,
-    PutManagedRuleSetVersionsResponseTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RateLimitLabelNamespaceTypeDef,
+    ResponseInspectionBodyContainsOutputTypeDef,
     ResponseInspectionBodyContainsTypeDef,
+    ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
+    ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
+    ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateIPSetResponseTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
-    UpdateRegexPatternSetResponseTypeDef,
-    UpdateRuleGroupResponseTypeDef,
-    UpdateWebACLResponseTypeDef,
-    ListAPIKeysResponseTypeDef,
+    AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
+    RateLimitCookieOutputTypeDef,
     RateLimitCookieTypeDef,
+    RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
+    RateLimitQueryArgumentOutputTypeDef,
     RateLimitQueryArgumentTypeDef,
+    RateLimitQueryStringOutputTypeDef,
     RateLimitQueryStringTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
+    CheckCapacityResponseTypeDef,
+    CreateAPIKeyResponseTypeDef,
+    DeleteFirewallManagerRuleGroupsResponseTypeDef,
+    GenerateMobileSdkReleaseUrlResponseTypeDef,
+    GetDecryptedAPIKeyResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    ListAPIKeysResponseTypeDef,
+    ListResourcesForWebACLResponseTypeDef,
+    PutManagedRuleSetVersionsResponseTypeDef,
+    UpdateIPSetResponseTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
+    UpdateRegexPatternSetResponseTypeDef,
+    UpdateRuleGroupResponseTypeDef,
+    UpdateWebACLResponseTypeDef,
     ConditionTypeDef,
+    CookiesOutputTypeDef,
     CookiesTypeDef,
     CreateIPSetRequestRequestTypeDef,
     MobileSdkReleaseTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIPSetResponseTypeDef,
     ListIPSetsResponseTypeDef,
@@ -448,91 +463,133 @@
     UpdateRegexPatternSetRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     CreateWebACLResponseTypeDef,
     ListWebACLsResponseTypeDef,
+    CustomRequestHandlingOutputTypeDef,
     CustomRequestHandlingTypeDef,
+    CustomResponseOutputTypeDef,
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
+    GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
+    JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
     ListAvailableManagedRuleGroupsResponseTypeDef,
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
+    RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
+    ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    TimeWindowTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
+    AssociationConfigUnionTypeDef,
+    RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
+    AllowActionOutputTypeDef,
+    CaptchaActionOutputTypeDef,
+    ChallengeActionOutputTypeDef,
+    CountActionOutputTypeDef,
     AllowActionTypeDef,
     CaptchaActionTypeDef,
     ChallengeActionTypeDef,
     CountActionTypeDef,
+    BlockActionOutputTypeDef,
     BlockActionTypeDef,
     SampledHTTPRequestTypeDef,
+    FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
+    AWSManagedRulesACFPRuleSetOutputTypeDef,
+    AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
+    RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
+    LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
+    OverrideActionOutputTypeDef,
     OverrideActionTypeDef,
+    DefaultActionOutputTypeDef,
+    RuleActionOutputTypeDef,
     DefaultActionTypeDef,
     RuleActionTypeDef,
     GetSampledRequestsResponseTypeDef,
+    ByteMatchStatementOutputTypeDef,
+    RegexMatchStatementOutputTypeDef,
+    RegexPatternSetReferenceStatementOutputTypeDef,
+    SizeConstraintStatementOutputTypeDef,
+    SqliMatchStatementOutputTypeDef,
+    XssMatchStatementOutputTypeDef,
     ByteMatchStatementTypeDef,
     RegexMatchStatementTypeDef,
     RegexPatternSetReferenceStatementTypeDef,
     SizeConstraintStatementTypeDef,
     SqliMatchStatementTypeDef,
     XssMatchStatementTypeDef,
+    ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
-    RuleActionOverrideTypeDef,
+    RuleActionOverrideOutputTypeDef,
+    RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    DefaultActionUnionTypeDef,
+    RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
+    ManagedRuleGroupStatementOutputTypeDef,
+    RuleGroupReferenceStatementOutputTypeDef,
+    RuleGroupTypeDef,
+    DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
-    DescribeManagedRuleGroupResponseTypeDef,
+    RuleUnionTypeDef,
+    FirewallManagerStatementTypeDef,
+    StatementOutputTypeDef,
+    GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
-    RuleGroupTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
-    FirewallManagerStatementTypeDef,
-    StatementTypeDef,
-    GetRuleGroupResponseTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> APIKeySummaryTypeDef:
+def get_value() -> APIKeySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wafv2-2.5.2/types_aiobotocore_wafv2.egg-info/SOURCES.txt` & `types-aiobotocore-wafv2-2.5.2.post1/types_aiobotocore_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


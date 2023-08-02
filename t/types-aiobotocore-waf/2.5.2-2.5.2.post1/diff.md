# Comparing `tmp/types-aiobotocore-waf-2.5.2.tar.gz` & `tmp/types-aiobotocore-waf-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-2.5.2.tar", last modified: Sat Jul  8 01:44:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
```

## Comparing `types-aiobotocore-waf-2.5.2.tar` & `types-aiobotocore-waf-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.387033 types-aiobotocore-waf-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24721 2023-07-08 01:44:27.387033 types-aiobotocore-waf-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:27.387033 types-aiobotocore-waf-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.387033 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52660 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52558 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18511 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18493 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59262 2023-07-08 01:42:21.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59215 2023-07-08 01:42:20.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:19.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.387033 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24721 2023-07-08 01:44:27.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:27.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:27.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:27.000000 types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24895 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23393 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52680 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52578 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61264 2023-08-02 14:50:57.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61213 2023-08-02 14:50:56.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:55.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.233430 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24895 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:09.000000 types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-2.5.2/LICENSE` & `types-aiobotocore-waf-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2/PKG-INFO` & `types-aiobotocore-waf-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore waf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore waf type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-waf"></a>
 
 # types-aiobotocore-waf
 
 [![PyPI - types-aiobotocore-waf](https://img.shields.io/pypi/v/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-waf?color=blue)](https://pypistats.org/packages/types-aiobotocore-waf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [types-aiobotocore-waf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/).
 
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
@@ -387,174 +386,178 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_waf.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_waf.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
-    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
-    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
-    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
-    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
-    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
-    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
-    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
-    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
-    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
-    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
-    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ActivatedRuleOutputTypeDef,
+    ActivatedRuleTypeDef,
+    ByteMatchTupleOutputTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationOutputTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
+    DeleteIPSetResponseTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    DeleteRuleResponseTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
+    DeleteWebACLResponseTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
+    GetChangeTokenResponseTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
+    ListByteMatchSetsResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
-    ActivatedRuleTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
+    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
+    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
+    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
+    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
+    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
+    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
+    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
+    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
+    ListWebACLsRequestListWebACLsPaginateTypeDef,
+    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListRegexMatchSetsResponseTypeDef,
@@ -565,24 +568,26 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
-    RuleGroupUpdateTypeDef,
     WebACLTypeDef,
+    RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
     ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
     RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetTypeDef,
@@ -597,17 +602,19 @@
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleGroupRequestRequestTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
+    UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
     UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
     UpdateRegexMatchSetRequestRequestTypeDef,
@@ -620,15 +627,15 @@
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_value() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-waf-2.5.2/README.md` & `types-aiobotocore-waf-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-waf"></a>
 
 # types-aiobotocore-waf
 
 [![PyPI - types-aiobotocore-waf](https://img.shields.io/pypi/v/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-waf?color=blue)](https://pypistats.org/packages/types-aiobotocore-waf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [types-aiobotocore-waf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/).
 
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
@@ -354,174 +354,178 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_waf.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_waf.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
-    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
-    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
-    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
-    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
-    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
-    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
-    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
-    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
-    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
-    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
-    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ActivatedRuleOutputTypeDef,
+    ActivatedRuleTypeDef,
+    ByteMatchTupleOutputTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationOutputTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
+    DeleteIPSetResponseTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    DeleteRuleResponseTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
+    DeleteWebACLResponseTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
+    GetChangeTokenResponseTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
+    ListByteMatchSetsResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
-    ActivatedRuleTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
+    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
+    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
+    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
+    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
+    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
+    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
+    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
+    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
+    ListWebACLsRequestListWebACLsPaginateTypeDef,
+    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListRegexMatchSetsResponseTypeDef,
@@ -532,24 +536,26 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
-    RuleGroupUpdateTypeDef,
     WebACLTypeDef,
+    RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
     ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
     RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetTypeDef,
@@ -564,17 +570,19 @@
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleGroupRequestRequestTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
+    UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
     UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
     UpdateRegexMatchSetRequestRequestTypeDef,
@@ -587,15 +595,15 @@
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_value() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-waf-2.5.2/setup.py` & `types-aiobotocore-waf-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore waf type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore waf type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_waf": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/__init__.py` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/__init__.pyi` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/__main__.py` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAF 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WAF 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/client.py` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,24 +97,24 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -600,15 +600,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_rule_group)
         """
 
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_sampled_requests)
         """
@@ -806,15 +806,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#list_xss_match_sets)
         """
 
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/client.pyi` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -97,24 +97,24 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -552,15 +552,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_rule_group)
         """
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#get_sampled_requests)
         """
@@ -737,15 +737,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#list_xss_match_sets)
         """
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/literals.py` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/literals.pyi` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/paginator.py` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,238 +108,238 @@
 class GetRateBasedRuleManagedKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#getratebasedrulemanagedkeyspaginator)
     """
 
     def paginate(
-        self, *, RuleId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRateBasedRuleManagedKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#getratebasedrulemanagedkeyspaginator)
         """
 
 
 class ListActivatedRulesInRuleGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listactivatedrulesinrulegrouppaginator)
     """
 
     def paginate(
-        self, *, RuleGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActivatedRulesInRuleGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listactivatedrulesinrulegrouppaginator)
         """
 
 
 class ListByteMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listbytematchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListByteMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listbytematchsetspaginator)
         """
 
 
 class ListGeoMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listgeomatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeoMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listgeomatchsetspaginator)
         """
 
 
 class ListIPSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listipsetspaginator)
         """
 
 
 class ListLoggingConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listloggingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLoggingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listloggingconfigurationspaginator)
         """
 
 
 class ListRateBasedRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listratebasedrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRateBasedRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listratebasedrulespaginator)
         """
 
 
 class ListRegexMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRegexMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexmatchsetspaginator)
         """
 
 
 class ListRegexPatternSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexpatternsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRegexPatternSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexpatternsetspaginator)
         """
 
 
 class ListRuleGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulegroupspaginator)
         """
 
 
 class ListRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulespaginator)
         """
 
 
 class ListSizeConstraintSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsizeconstraintsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSizeConstraintSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsizeconstraintsetspaginator)
         """
 
 
 class ListSqlInjectionMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsqlinjectionmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSqlInjectionMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsqlinjectionmatchsetspaginator)
         """
 
 
 class ListSubscribedRuleGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsubscribedrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSubscribedRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsubscribedrulegroupspaginator)
         """
 
 
 class ListWebACLsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listwebaclspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWebACLsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listwebaclspaginator)
         """
 
 
 class ListXssMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listxssmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListXssMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listxssmatchsetspaginator)
         """
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/paginator.pyi` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -105,223 +105,223 @@
 class GetRateBasedRuleManagedKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#getratebasedrulemanagedkeyspaginator)
     """
 
     def paginate(
-        self, *, RuleId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRateBasedRuleManagedKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.GetRateBasedRuleManagedKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#getratebasedrulemanagedkeyspaginator)
         """
 
 class ListActivatedRulesInRuleGroupPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listactivatedrulesinrulegrouppaginator)
     """
 
     def paginate(
-        self, *, RuleGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RuleGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActivatedRulesInRuleGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListActivatedRulesInRuleGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listactivatedrulesinrulegrouppaginator)
         """
 
 class ListByteMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listbytematchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListByteMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListByteMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listbytematchsetspaginator)
         """
 
 class ListGeoMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listgeomatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeoMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListGeoMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listgeomatchsetspaginator)
         """
 
 class ListIPSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListIPSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listipsetspaginator)
         """
 
 class ListLoggingConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listloggingconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLoggingConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListLoggingConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listloggingconfigurationspaginator)
         """
 
 class ListRateBasedRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listratebasedrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRateBasedRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRateBasedRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listratebasedrulespaginator)
         """
 
 class ListRegexMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRegexMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexmatchsetspaginator)
         """
 
 class ListRegexPatternSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexpatternsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRegexPatternSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRegexPatternSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listregexpatternsetspaginator)
         """
 
 class ListRuleGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulegroupspaginator)
         """
 
 class ListRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listrulespaginator)
         """
 
 class ListSizeConstraintSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsizeconstraintsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSizeConstraintSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSizeConstraintSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsizeconstraintsetspaginator)
         """
 
 class ListSqlInjectionMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsqlinjectionmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSqlInjectionMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSqlInjectionMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsqlinjectionmatchsetspaginator)
         """
 
 class ListSubscribedRuleGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsubscribedrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSubscribedRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListSubscribedRuleGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listsubscribedrulegroupspaginator)
         """
 
 class ListWebACLsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listwebaclspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWebACLsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListWebACLs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listwebaclspaginator)
         """
 
 class ListXssMatchSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listxssmatchsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListXssMatchSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Paginator.ListXssMatchSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/paginators/#listxssmatchsetspaginator)
         """
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/type_defs.py` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_waf.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import IO, Any, Dict, List, Sequence, Union
+
+from aiobotocore.response import StreamingBody
 
 from .literals import (
     ChangeActionType,
     ChangeTokenStatusType,
     ComparisonOperatorType,
     GeoMatchConstraintValueType,
     IPSetDescriptorTypeType,
@@ -40,162 +42,166 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
+    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
     "RegexPatternSetTypeDef",
     "RuleGroupTypeDef",
     "CreateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateWebACLMigrationStackRequestRequestTypeDef",
-    "CreateWebACLMigrationStackResponseTypeDef",
     "CreateXssMatchSetRequestRequestTypeDef",
     "DeleteByteMatchSetRequestRequestTypeDef",
-    "DeleteByteMatchSetResponseTypeDef",
     "DeleteGeoMatchSetRequestRequestTypeDef",
-    "DeleteGeoMatchSetResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
-    "DeleteIPSetResponseTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRateBasedRuleRequestRequestTypeDef",
-    "DeleteRateBasedRuleResponseTypeDef",
     "DeleteRegexMatchSetRequestRequestTypeDef",
-    "DeleteRegexMatchSetResponseTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
-    "DeleteRegexPatternSetResponseTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
     "DeleteRuleRequestRequestTypeDef",
-    "DeleteRuleResponseTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
-    "DeleteSizeConstraintSetResponseTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
-    "DeleteWebACLResponseTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
-    "DeleteXssMatchSetResponseTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
-    "GetChangeTokenResponseTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
-    "GetChangeTokenStatusResponseTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ActivatedRuleOutputTypeDef",
+    "ActivatedRuleTypeDef",
+    "ByteMatchTupleOutputTypeDef",
+    "ByteMatchTupleTypeDef",
+    "LoggingConfigurationOutputTypeDef",
+    "LoggingConfigurationTypeDef",
+    "RegexMatchTupleTypeDef",
+    "SizeConstraintTypeDef",
+    "SqlInjectionMatchTupleTypeDef",
+    "XssMatchTupleTypeDef",
+    "CreateWebACLMigrationStackResponseTypeDef",
+    "DeleteByteMatchSetResponseTypeDef",
+    "DeleteGeoMatchSetResponseTypeDef",
+    "DeleteIPSetResponseTypeDef",
+    "DeleteRateBasedRuleResponseTypeDef",
+    "DeleteRegexMatchSetResponseTypeDef",
+    "DeleteRegexPatternSetResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "DeleteRuleResponseTypeDef",
+    "DeleteSizeConstraintSetResponseTypeDef",
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    "DeleteWebACLResponseTypeDef",
+    "DeleteXssMatchSetResponseTypeDef",
+    "GetChangeTokenResponseTypeDef",
+    "GetChangeTokenStatusResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    "ListByteMatchSetsResponseTypeDef",
     "UpdateByteMatchSetResponseTypeDef",
     "UpdateGeoMatchSetResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateRateBasedRuleResponseTypeDef",
     "UpdateRegexMatchSetResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateRuleResponseTypeDef",
     "UpdateSizeConstraintSetResponseTypeDef",
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
-    "ActivatedRuleTypeDef",
-    "ListByteMatchSetsResponseTypeDef",
-    "ByteMatchTupleTypeDef",
-    "LoggingConfigurationTypeDef",
-    "RegexMatchTupleTypeDef",
-    "SizeConstraintTypeDef",
-    "SqlInjectionMatchTupleTypeDef",
-    "XssMatchTupleTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
     "ListGeoMatchSetsResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
+    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListRegexMatchSetsResponseTypeDef",
@@ -206,24 +212,26 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
-    "RuleGroupUpdateTypeDef",
     "WebACLTypeDef",
+    "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
     "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
     "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetTypeDef",
@@ -238,17 +246,19 @@
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleGroupRequestRequestTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
+    "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
     "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
     "UpdateRegexMatchSetRequestRequestTypeDef",
@@ -281,14 +291,15 @@
 WafOverrideActionTypeDef = TypedDict(
     "WafOverrideActionTypeDef",
     {
         "Type": WafOverrideActionTypeType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ByteMatchSetSummaryTypeDef = TypedDict(
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
@@ -316,14 +327,25 @@
     "CreateByteMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
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
 CreateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "CreateGeoMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -421,22 +443,14 @@
     {
         "WebACLId": str,
         "S3BucketName": str,
         "IgnoreUnsupportedType": bool,
     },
 )
 
-CreateWebACLMigrationStackResponseTypeDef = TypedDict(
-    "CreateWebACLMigrationStackResponseTypeDef",
-    {
-        "S3ObjectUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateXssMatchSetRequestRequestTypeDef = TypedDict(
     "CreateXssMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -445,54 +459,30 @@
     "DeleteByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteByteMatchSetResponseTypeDef = TypedDict(
-    "DeleteByteMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGeoMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteGeoMatchSetResponseTypeDef = TypedDict(
-    "DeleteGeoMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteIPSetResponseTypeDef = TypedDict(
-    "DeleteIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -507,150 +497,78 @@
     "DeleteRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRateBasedRuleResponseTypeDef = TypedDict(
-    "DeleteRateBasedRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexMatchSetResponseTypeDef = TypedDict(
-    "DeleteRegexMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexPatternSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexPatternSetRequestRequestTypeDef",
     {
         "RegexPatternSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexPatternSetResponseTypeDef = TypedDict(
-    "DeleteRegexPatternSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleGroupRequestRequestTypeDef = TypedDict(
     "DeleteRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleResponseTypeDef = TypedDict(
-    "DeleteRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSizeConstraintSetResponseTypeDef = TypedDict(
-    "DeleteSizeConstraintSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebACLRequestRequestTypeDef = TypedDict(
     "DeleteWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteWebACLResponseTypeDef = TypedDict(
-    "DeleteWebACLResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteXssMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteXssMatchSetResponseTypeDef = TypedDict(
-    "DeleteXssMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
         "Value": GeoMatchConstraintValueType,
     },
 )
@@ -666,37 +584,21 @@
 GetByteMatchSetRequestRequestTypeDef = TypedDict(
     "GetByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
     },
 )
 
-GetChangeTokenResponseTypeDef = TypedDict(
-    "GetChangeTokenResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChangeTokenStatusRequestRequestTypeDef = TypedDict(
     "GetChangeTokenStatusRequestRequestTypeDef",
     {
         "ChangeToken": str,
     },
 )
 
-GetChangeTokenStatusResponseTypeDef = TypedDict(
-    "GetChangeTokenStatusResponseTypeDef",
-    {
-        "ChangeTokenStatus": ChangeTokenStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGeoMatchSetRequestRequestTypeDef = TypedDict(
     "GetGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
     },
 )
 
@@ -717,44 +619,24 @@
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
-_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
-    {
-        "RuleId": str,
-    },
-)
-_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
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
-class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
-    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -769,23 +651,14 @@
 class GetRateBasedRuleManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef,
 ):
     pass
 
 
-GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    {
-        "ManagedKeys": List[str],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRateBasedRuleRequestRequestTypeDef = TypedDict(
     "GetRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -813,19 +686,19 @@
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
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
 
 GetSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "GetSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
@@ -874,109 +747,60 @@
     "IPSetSummaryTypeDef",
     {
         "IPSetId": str,
         "Name": str,
     },
 )
 
-ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
-    {
-        "RuleGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivatedRulesInRuleGroupRequestRequestTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListByteMatchSetsRequestRequestTypeDef = TypedDict(
     "ListByteMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeoMatchSetsRequestRequestTypeDef = TypedDict(
     "ListGeoMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIPSetsRequestRequestTypeDef = TypedDict(
     "ListIPSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLoggingConfigurationsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRateBasedRulesRequestRequestTypeDef = TypedDict(
     "ListRateBasedRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -986,22 +810,14 @@
     "RuleSummaryTypeDef",
     {
         "RuleId": str,
         "Name": str,
     },
 )
 
-ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexMatchSetsRequestRequestTypeDef = TypedDict(
     "ListRegexMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1011,22 +827,14 @@
     "RegexMatchSetSummaryTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
     },
 )
 
-ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexPatternSetsRequestRequestTypeDef = TypedDict(
     "ListRegexPatternSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1036,22 +844,14 @@
     "RegexPatternSetSummaryTypeDef",
     {
         "RegexPatternSetId": str,
         "Name": str,
     },
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1061,39 +861,23 @@
     "RuleGroupSummaryTypeDef",
     {
         "RuleGroupId": str,
         "Name": str,
     },
 )
 
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSizeConstraintSetsRequestRequestTypeDef = TypedDict(
     "ListSizeConstraintSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1103,22 +887,14 @@
     "SizeConstraintSetSummaryTypeDef",
     {
         "SizeConstraintSetId": str,
         "Name": str,
     },
 )
 
-ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSqlInjectionMatchSetsRequestRequestTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1128,22 +904,14 @@
     "SqlInjectionMatchSetSummaryTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "Name": str,
     },
 )
 
-ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribedRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1177,22 +945,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebACLsRequestRequestTypeDef = TypedDict(
     "ListWebACLsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1202,22 +962,14 @@
     "WebACLSummaryTypeDef",
     {
         "WebACLId": str,
         "Name": str,
     },
 )
 
-ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListXssMatchSetsRequestRequestTypeDef = TypedDict(
     "ListXssMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1227,24 +979,14 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
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
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
         "DataId": str,
     },
@@ -1262,225 +1004,409 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
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
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateByteMatchSetResponseTypeDef = TypedDict(
-    "UpdateByteMatchSetResponseTypeDef",
+_RequiredActivatedRuleOutputTypeDef = TypedDict(
+    "_RequiredActivatedRuleOutputTypeDef",
     {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Priority": int,
+        "RuleId": str,
+    },
+)
+_OptionalActivatedRuleOutputTypeDef = TypedDict(
+    "_OptionalActivatedRuleOutputTypeDef",
+    {
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": List[ExcludedRuleTypeDef],
     },
+    total=False,
 )
 
-UpdateGeoMatchSetResponseTypeDef = TypedDict(
-    "UpdateGeoMatchSetResponseTypeDef",
+
+class ActivatedRuleOutputTypeDef(
+    _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
+):
+    pass
+
+
+_RequiredActivatedRuleTypeDef = TypedDict(
+    "_RequiredActivatedRuleTypeDef",
+    {
+        "Priority": int,
+        "RuleId": str,
+    },
+)
+_OptionalActivatedRuleTypeDef = TypedDict(
+    "_OptionalActivatedRuleTypeDef",
+    {
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": Sequence[ExcludedRuleTypeDef],
+    },
+    total=False,
+)
+
+
+class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
+    pass
+
+
+ByteMatchTupleOutputTypeDef = TypedDict(
+    "ByteMatchTupleOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": bytes,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
+ByteMatchTupleTypeDef = TypedDict(
+    "ByteMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": BlobTypeDef,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
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
+        "RedactedFields": List[FieldToMatchTypeDef],
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
+_RequiredLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationTypeDef",
+    {
+        "ResourceArn": str,
+        "LogDestinationConfigs": Sequence[str],
+    },
+)
+_OptionalLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationTypeDef",
+    {
+        "RedactedFields": Sequence[FieldToMatchTypeDef],
+    },
+    total=False,
+)
+
+
+class LoggingConfigurationTypeDef(
+    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
+):
+    pass
+
+
+RegexMatchTupleTypeDef = TypedDict(
+    "RegexMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "RegexPatternSetId": str,
+    },
+)
+
+SizeConstraintTypeDef = TypedDict(
+    "SizeConstraintTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
+    },
+)
+
+SqlInjectionMatchTupleTypeDef = TypedDict(
+    "SqlInjectionMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+    },
+)
+
+XssMatchTupleTypeDef = TypedDict(
+    "XssMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+    },
+)
+
+CreateWebACLMigrationStackResponseTypeDef = TypedDict(
+    "CreateWebACLMigrationStackResponseTypeDef",
+    {
+        "S3ObjectUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteByteMatchSetResponseTypeDef = TypedDict(
+    "DeleteByteMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
+DeleteGeoMatchSetResponseTypeDef = TypedDict(
+    "DeleteGeoMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRateBasedRuleResponseTypeDef = TypedDict(
-    "UpdateRateBasedRuleResponseTypeDef",
+DeleteIPSetResponseTypeDef = TypedDict(
+    "DeleteIPSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRegexMatchSetResponseTypeDef = TypedDict(
-    "UpdateRegexMatchSetResponseTypeDef",
+DeleteRateBasedRuleResponseTypeDef = TypedDict(
+    "DeleteRateBasedRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+DeleteRegexMatchSetResponseTypeDef = TypedDict(
+    "DeleteRegexMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+DeleteRegexPatternSetResponseTypeDef = TypedDict(
+    "DeleteRegexPatternSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSizeConstraintSetResponseTypeDef = TypedDict(
-    "UpdateSizeConstraintSetResponseTypeDef",
+DeleteRuleResponseTypeDef = TypedDict(
+    "DeleteRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetResponseTypeDef",
+DeleteSizeConstraintSetResponseTypeDef = TypedDict(
+    "DeleteSizeConstraintSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateXssMatchSetResponseTypeDef = TypedDict(
-    "UpdateXssMatchSetResponseTypeDef",
+DeleteWebACLResponseTypeDef = TypedDict(
+    "DeleteWebACLResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActivatedRuleTypeDef = TypedDict(
-    "_RequiredActivatedRuleTypeDef",
+DeleteXssMatchSetResponseTypeDef = TypedDict(
+    "DeleteXssMatchSetResponseTypeDef",
     {
-        "Priority": int,
-        "RuleId": str,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalActivatedRuleTypeDef = TypedDict(
-    "_OptionalActivatedRuleTypeDef",
+
+GetChangeTokenResponseTypeDef = TypedDict(
+    "GetChangeTokenResponseTypeDef",
     {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetChangeTokenStatusResponseTypeDef = TypedDict(
+    "GetChangeTokenStatusResponseTypeDef",
+    {
+        "ChangeTokenStatus": ChangeTokenStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
-    pass
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    {
+        "ManagedKeys": List[str],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListByteMatchSetsResponseTypeDef = TypedDict(
     "ListByteMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ByteMatchTupleTypeDef = TypedDict(
-    "ByteMatchTupleTypeDef",
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingConfigurationTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationTypeDef",
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
     {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalLoggingConfigurationTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationTypeDef",
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class LoggingConfigurationTypeDef(
-    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
-):
-    pass
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RegexMatchTupleTypeDef = TypedDict(
-    "RegexMatchTupleTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "RegexPatternSetId": str,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SizeConstraintTypeDef = TypedDict(
-    "SizeConstraintTypeDef",
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SqlInjectionMatchTupleTypeDef = TypedDict(
-    "SqlInjectionMatchTupleTypeDef",
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-XssMatchTupleTypeDef = TypedDict(
-    "XssMatchTupleTypeDef",
+UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateXssMatchSetResponseTypeDef = TypedDict(
+    "UpdateXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRateBasedRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -1594,40 +1520,40 @@
 )
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
@@ -1656,27 +1582,160 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
+_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
     {
-        "WebAclId": str,
         "RuleId": str,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
     },
 )
+_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
+    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+):
+    pass
+
+
+ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    {
+        "RuleGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
         "Country": str,
         "URI": str,
@@ -1716,105 +1775,105 @@
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
 
 ListRateBasedRulesResponseTypeDef = TypedDict(
     "ListRateBasedRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexMatchSetsResponseTypeDef = TypedDict(
     "ListRegexMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexMatchSets": List[RegexMatchSetSummaryTypeDef],
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
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSizeConstraintSetsResponseTypeDef = TypedDict(
     "ListSizeConstraintSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SizeConstraintSets": List[SizeConstraintSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSqlInjectionMatchSetsResponseTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SqlInjectionMatchSets": List[SqlInjectionMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribedRuleGroupsResponseTypeDef = TypedDict(
     "ListSubscribedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[SubscribedRuleGroupSummaryTypeDef],
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
     },
 )
 
 ListXssMatchSetsResponseTypeDef = TypedDict(
     "ListXssMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "XssMatchSets": List[XssMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
@@ -1871,37 +1930,37 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
-ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupResponseTypeDef",
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
     {
-        "NextMarker": str,
-        "ActivatedRules": List[ActivatedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 
-RuleGroupUpdateTypeDef = TypedDict(
-    "RuleGroupUpdateTypeDef",
+ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
-        "Action": ChangeActionType,
-        "ActivatedRule": ActivatedRuleTypeDef,
+        "NextMarker": str,
+        "ActivatedRules": List[ActivatedRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
         "DefaultAction": WafActionTypeDef,
-        "Rules": List[ActivatedRuleTypeDef],
+        "Rules": List[ActivatedRuleOutputTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1911,27 +1970,35 @@
 )
 
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
 
+RuleGroupUpdateTypeDef = TypedDict(
+    "RuleGroupUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ActivatedRule": ActivatedRuleTypeDef,
+    },
+)
+
 WebACLUpdateTypeDef = TypedDict(
     "WebACLUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "ActivatedRule": ActivatedRuleTypeDef,
     },
 )
 
 _RequiredByteMatchSetTypeDef = TypedDict(
     "_RequiredByteMatchSetTypeDef",
     {
         "ByteMatchSetId": str,
-        "ByteMatchTuples": List[ByteMatchTupleTypeDef],
+        "ByteMatchTuples": List[ByteMatchTupleOutputTypeDef],
     },
 )
 _OptionalByteMatchSetTypeDef = TypedDict(
     "_OptionalByteMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1950,40 +2017,43 @@
         "ByteMatchTuple": ByteMatchTupleTypeDef,
     },
 )
 
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
 
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2090,32 +2160,32 @@
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
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoMatchSetResponseTypeDef = TypedDict(
     "GetGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
@@ -2149,23 +2219,23 @@
 
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIPSetRequestRequestTypeDef = TypedDict(
     "UpdateIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
@@ -2175,40 +2245,40 @@
 )
 
 CreateRateBasedRuleResponseTypeDef = TypedDict(
     "CreateRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedRuleResponseTypeDef = TypedDict(
     "GetRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "UpdateRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
@@ -2223,37 +2293,48 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
-UpdateRuleGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRuleGroupRequestRequestTypeDef",
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
     {
-        "RuleGroupId": str,
-        "Updates": Sequence[RuleGroupUpdateTypeDef],
-        "ChangeToken": str,
+        "WebAclId": str,
+        "RuleId": str,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
     },
 )
 
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRuleGroupRequestRequestTypeDef",
+    {
+        "RuleGroupId": str,
+        "Updates": Sequence[RuleGroupUpdateTypeDef],
+        "ChangeToken": str,
     },
 )
 
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
@@ -2277,23 +2358,23 @@
 
 
 CreateByteMatchSetResponseTypeDef = TypedDict(
     "CreateByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetByteMatchSetResponseTypeDef = TypedDict(
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
@@ -2303,23 +2384,23 @@
 )
 
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexMatchSetResponseTypeDef = TypedDict(
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2329,23 +2410,23 @@
 )
 
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSizeConstraintSetResponseTypeDef = TypedDict(
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "UpdateSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
@@ -2355,23 +2436,23 @@
 )
 
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
@@ -2381,23 +2462,23 @@
 )
 
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetXssMatchSetResponseTypeDef = TypedDict(
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
@@ -2407,11 +2488,11 @@
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
     },
 )
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf/type_defs.pyi` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_waf.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import IO, Any, Dict, List, Sequence, Union
+
+from aiobotocore.response import StreamingBody
 
 from .literals import (
     ChangeActionType,
     ChangeTokenStatusType,
     ComparisonOperatorType,
     GeoMatchConstraintValueType,
     IPSetDescriptorTypeType,
@@ -39,162 +41,166 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
+    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
     "CreateRegexMatchSetRequestRequestTypeDef",
     "CreateRegexPatternSetRequestRequestTypeDef",
     "RegexPatternSetTypeDef",
     "RuleGroupTypeDef",
     "CreateSizeConstraintSetRequestRequestTypeDef",
     "CreateSqlInjectionMatchSetRequestRequestTypeDef",
     "CreateWebACLMigrationStackRequestRequestTypeDef",
-    "CreateWebACLMigrationStackResponseTypeDef",
     "CreateXssMatchSetRequestRequestTypeDef",
     "DeleteByteMatchSetRequestRequestTypeDef",
-    "DeleteByteMatchSetResponseTypeDef",
     "DeleteGeoMatchSetRequestRequestTypeDef",
-    "DeleteGeoMatchSetResponseTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
-    "DeleteIPSetResponseTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeletePermissionPolicyRequestRequestTypeDef",
     "DeleteRateBasedRuleRequestRequestTypeDef",
-    "DeleteRateBasedRuleResponseTypeDef",
     "DeleteRegexMatchSetRequestRequestTypeDef",
-    "DeleteRegexMatchSetResponseTypeDef",
     "DeleteRegexPatternSetRequestRequestTypeDef",
-    "DeleteRegexPatternSetResponseTypeDef",
     "DeleteRuleGroupRequestRequestTypeDef",
-    "DeleteRuleGroupResponseTypeDef",
     "DeleteRuleRequestRequestTypeDef",
-    "DeleteRuleResponseTypeDef",
     "DeleteSizeConstraintSetRequestRequestTypeDef",
-    "DeleteSizeConstraintSetResponseTypeDef",
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
     "DeleteWebACLRequestRequestTypeDef",
-    "DeleteWebACLResponseTypeDef",
     "DeleteXssMatchSetRequestRequestTypeDef",
-    "DeleteXssMatchSetResponseTypeDef",
     "GeoMatchConstraintTypeDef",
     "GeoMatchSetSummaryTypeDef",
     "GetByteMatchSetRequestRequestTypeDef",
-    "GetChangeTokenResponseTypeDef",
     "GetChangeTokenStatusRequestRequestTypeDef",
-    "GetChangeTokenStatusResponseTypeDef",
     "GetGeoMatchSetRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
-    "GetPermissionPolicyResponseTypeDef",
-    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowTypeDef",
+    "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "IPSetDescriptorTypeDef",
     "IPSetSummaryTypeDef",
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
     "ListByteMatchSetsRequestRequestTypeDef",
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
     "ListGeoMatchSetsRequestRequestTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     "SubscribedRuleGroupSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ActivatedRuleOutputTypeDef",
+    "ActivatedRuleTypeDef",
+    "ByteMatchTupleOutputTypeDef",
+    "ByteMatchTupleTypeDef",
+    "LoggingConfigurationOutputTypeDef",
+    "LoggingConfigurationTypeDef",
+    "RegexMatchTupleTypeDef",
+    "SizeConstraintTypeDef",
+    "SqlInjectionMatchTupleTypeDef",
+    "XssMatchTupleTypeDef",
+    "CreateWebACLMigrationStackResponseTypeDef",
+    "DeleteByteMatchSetResponseTypeDef",
+    "DeleteGeoMatchSetResponseTypeDef",
+    "DeleteIPSetResponseTypeDef",
+    "DeleteRateBasedRuleResponseTypeDef",
+    "DeleteRegexMatchSetResponseTypeDef",
+    "DeleteRegexPatternSetResponseTypeDef",
+    "DeleteRuleGroupResponseTypeDef",
+    "DeleteRuleResponseTypeDef",
+    "DeleteSizeConstraintSetResponseTypeDef",
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
+    "DeleteWebACLResponseTypeDef",
+    "DeleteXssMatchSetResponseTypeDef",
+    "GetChangeTokenResponseTypeDef",
+    "GetChangeTokenStatusResponseTypeDef",
+    "GetPermissionPolicyResponseTypeDef",
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    "ListByteMatchSetsResponseTypeDef",
     "UpdateByteMatchSetResponseTypeDef",
     "UpdateGeoMatchSetResponseTypeDef",
     "UpdateIPSetResponseTypeDef",
     "UpdateRateBasedRuleResponseTypeDef",
     "UpdateRegexMatchSetResponseTypeDef",
     "UpdateRegexPatternSetResponseTypeDef",
     "UpdateRuleGroupResponseTypeDef",
     "UpdateRuleResponseTypeDef",
     "UpdateSizeConstraintSetResponseTypeDef",
     "UpdateSqlInjectionMatchSetResponseTypeDef",
     "UpdateWebACLResponseTypeDef",
     "UpdateXssMatchSetResponseTypeDef",
-    "ActivatedRuleTypeDef",
-    "ListByteMatchSetsResponseTypeDef",
-    "ByteMatchTupleTypeDef",
-    "LoggingConfigurationTypeDef",
-    "RegexMatchTupleTypeDef",
-    "SizeConstraintTypeDef",
-    "SqlInjectionMatchTupleTypeDef",
-    "XssMatchTupleTypeDef",
     "CreateRateBasedRuleRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
     "TagInfoForResourceTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
     "ListGeoMatchSetsResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
+    "GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListRegexMatchSetsResponseTypeDef",
@@ -205,24 +211,26 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
-    "RuleGroupUpdateTypeDef",
     "WebACLTypeDef",
+    "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
     "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
-    "PutLoggingConfigurationRequestRequestTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
+    "PutLoggingConfigurationRequestRequestTypeDef",
     "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
     "XssMatchSetTypeDef",
@@ -237,17 +245,19 @@
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleGroupRequestRequestTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
+    "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
     "UpdateByteMatchSetRequestRequestTypeDef",
     "CreateRegexMatchSetResponseTypeDef",
     "GetRegexMatchSetResponseTypeDef",
     "UpdateRegexMatchSetRequestRequestTypeDef",
@@ -280,14 +290,15 @@
 WafOverrideActionTypeDef = TypedDict(
     "WafOverrideActionTypeDef",
     {
         "Type": WafOverrideActionTypeType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ByteMatchSetSummaryTypeDef = TypedDict(
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
@@ -313,14 +324,25 @@
     "CreateByteMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
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
 CreateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "CreateGeoMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -414,22 +436,14 @@
     {
         "WebACLId": str,
         "S3BucketName": str,
         "IgnoreUnsupportedType": bool,
     },
 )
 
-CreateWebACLMigrationStackResponseTypeDef = TypedDict(
-    "CreateWebACLMigrationStackResponseTypeDef",
-    {
-        "S3ObjectUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateXssMatchSetRequestRequestTypeDef = TypedDict(
     "CreateXssMatchSetRequestRequestTypeDef",
     {
         "Name": str,
         "ChangeToken": str,
     },
 )
@@ -438,54 +452,30 @@
     "DeleteByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteByteMatchSetResponseTypeDef = TypedDict(
-    "DeleteByteMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGeoMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteGeoMatchSetResponseTypeDef = TypedDict(
-    "DeleteGeoMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIPSetRequestRequestTypeDef = TypedDict(
     "DeleteIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteIPSetResponseTypeDef = TypedDict(
-    "DeleteIPSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -500,150 +490,78 @@
     "DeleteRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRateBasedRuleResponseTypeDef = TypedDict(
-    "DeleteRateBasedRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexMatchSetResponseTypeDef = TypedDict(
-    "DeleteRegexMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRegexPatternSetRequestRequestTypeDef = TypedDict(
     "DeleteRegexPatternSetRequestRequestTypeDef",
     {
         "RegexPatternSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRegexPatternSetResponseTypeDef = TypedDict(
-    "DeleteRegexPatternSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleGroupRequestRequestTypeDef = TypedDict(
     "DeleteRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleGroupResponseTypeDef = TypedDict(
-    "DeleteRuleGroupResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "RuleId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteRuleResponseTypeDef = TypedDict(
-    "DeleteRuleResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "DeleteSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSizeConstraintSetResponseTypeDef = TypedDict(
-    "DeleteSizeConstraintSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "DeleteSqlInjectionMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebACLRequestRequestTypeDef = TypedDict(
     "DeleteWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteWebACLResponseTypeDef = TypedDict(
-    "DeleteWebACLResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteXssMatchSetRequestRequestTypeDef = TypedDict(
     "DeleteXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
         "ChangeToken": str,
     },
 )
 
-DeleteXssMatchSetResponseTypeDef = TypedDict(
-    "DeleteXssMatchSetResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GeoMatchConstraintTypeDef = TypedDict(
     "GeoMatchConstraintTypeDef",
     {
         "Type": Literal["Country"],
         "Value": GeoMatchConstraintValueType,
     },
 )
@@ -659,37 +577,21 @@
 GetByteMatchSetRequestRequestTypeDef = TypedDict(
     "GetByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
     },
 )
 
-GetChangeTokenResponseTypeDef = TypedDict(
-    "GetChangeTokenResponseTypeDef",
-    {
-        "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChangeTokenStatusRequestRequestTypeDef = TypedDict(
     "GetChangeTokenStatusRequestRequestTypeDef",
     {
         "ChangeToken": str,
     },
 )
 
-GetChangeTokenStatusResponseTypeDef = TypedDict(
-    "GetChangeTokenStatusResponseTypeDef",
-    {
-        "ChangeTokenStatus": ChangeTokenStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGeoMatchSetRequestRequestTypeDef = TypedDict(
     "GetGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
     },
 )
 
@@ -710,42 +612,24 @@
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
-_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
-    {
-        "RuleId": str,
-    },
-)
-_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
-    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
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
 
-class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
-    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -758,23 +642,14 @@
 
 class GetRateBasedRuleManagedKeysRequestRequestTypeDef(
     _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef,
     _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef,
 ):
     pass
 
-GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
-    "GetRateBasedRuleManagedKeysResponseTypeDef",
-    {
-        "ManagedKeys": List[str],
-        "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRateBasedRuleRequestRequestTypeDef = TypedDict(
     "GetRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 
@@ -802,19 +677,19 @@
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
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
 
 GetSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "GetSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
@@ -863,109 +738,60 @@
     "IPSetSummaryTypeDef",
     {
         "IPSetId": str,
         "Name": str,
     },
 )
 
-ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
-    {
-        "RuleGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivatedRulesInRuleGroupRequestRequestTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupRequestRequestTypeDef",
     {
         "RuleGroupId": str,
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
-    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListByteMatchSetsRequestRequestTypeDef = TypedDict(
     "ListByteMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
-    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeoMatchSetsRequestRequestTypeDef = TypedDict(
     "ListGeoMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIPSetsRequestRequestTypeDef = TypedDict(
     "ListIPSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
-    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLoggingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLoggingConfigurationsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
-    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRateBasedRulesRequestRequestTypeDef = TypedDict(
     "ListRateBasedRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -975,22 +801,14 @@
     "RuleSummaryTypeDef",
     {
         "RuleId": str,
         "Name": str,
     },
 )
 
-ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
-    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexMatchSetsRequestRequestTypeDef = TypedDict(
     "ListRegexMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1000,22 +818,14 @@
     "RegexMatchSetSummaryTypeDef",
     {
         "RegexMatchSetId": str,
         "Name": str,
     },
 )
 
-ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
-    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegexPatternSetsRequestRequestTypeDef = TypedDict(
     "ListRegexPatternSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1025,22 +835,14 @@
     "RegexPatternSetSummaryTypeDef",
     {
         "RegexPatternSetId": str,
         "Name": str,
     },
 )
 
-ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
-    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1050,39 +852,23 @@
     "RuleGroupSummaryTypeDef",
     {
         "RuleGroupId": str,
         "Name": str,
     },
 )
 
-ListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "ListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesRequestRequestTypeDef = TypedDict(
     "ListRulesRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
 )
 
-ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
-    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSizeConstraintSetsRequestRequestTypeDef = TypedDict(
     "ListSizeConstraintSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1092,22 +878,14 @@
     "SizeConstraintSetSummaryTypeDef",
     {
         "SizeConstraintSetId": str,
         "Name": str,
     },
 )
 
-ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
-    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSqlInjectionMatchSetsRequestRequestTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1117,22 +895,14 @@
     "SqlInjectionMatchSetSummaryTypeDef",
     {
         "SqlInjectionMatchSetId": str,
         "Name": str,
     },
 )
 
-ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
-    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscribedRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListSubscribedRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1164,22 +934,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
-    "ListWebACLsRequestListWebACLsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebACLsRequestRequestTypeDef = TypedDict(
     "ListWebACLsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1189,22 +951,14 @@
     "WebACLSummaryTypeDef",
     {
         "WebACLId": str,
         "Name": str,
     },
 )
 
-ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
-    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListXssMatchSetsRequestRequestTypeDef = TypedDict(
     "ListXssMatchSetsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1214,24 +968,14 @@
     "XssMatchSetSummaryTypeDef",
     {
         "XssMatchSetId": str,
         "Name": str,
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
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "Negated": bool,
         "Type": PredicateTypeType,
         "DataId": str,
     },
@@ -1249,221 +993,401 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
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
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateByteMatchSetResponseTypeDef = TypedDict(
-    "UpdateByteMatchSetResponseTypeDef",
+_RequiredActivatedRuleOutputTypeDef = TypedDict(
+    "_RequiredActivatedRuleOutputTypeDef",
+    {
+        "Priority": int,
+        "RuleId": str,
+    },
+)
+_OptionalActivatedRuleOutputTypeDef = TypedDict(
+    "_OptionalActivatedRuleOutputTypeDef",
+    {
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": List[ExcludedRuleTypeDef],
+    },
+    total=False,
+)
+
+class ActivatedRuleOutputTypeDef(
+    _RequiredActivatedRuleOutputTypeDef, _OptionalActivatedRuleOutputTypeDef
+):
+    pass
+
+_RequiredActivatedRuleTypeDef = TypedDict(
+    "_RequiredActivatedRuleTypeDef",
+    {
+        "Priority": int,
+        "RuleId": str,
+    },
+)
+_OptionalActivatedRuleTypeDef = TypedDict(
+    "_OptionalActivatedRuleTypeDef",
+    {
+        "Action": WafActionTypeDef,
+        "OverrideAction": WafOverrideActionTypeDef,
+        "Type": WafRuleTypeType,
+        "ExcludedRules": Sequence[ExcludedRuleTypeDef],
+    },
+    total=False,
+)
+
+class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
+    pass
+
+ByteMatchTupleOutputTypeDef = TypedDict(
+    "ByteMatchTupleOutputTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": bytes,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
+ByteMatchTupleTypeDef = TypedDict(
+    "ByteMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TargetString": BlobTypeDef,
+        "TextTransformation": TextTransformationType,
+        "PositionalConstraint": PositionalConstraintType,
+    },
+)
+
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
+        "RedactedFields": List[FieldToMatchTypeDef],
+    },
+    total=False,
+)
+
+class LoggingConfigurationOutputTypeDef(
+    _RequiredLoggingConfigurationOutputTypeDef, _OptionalLoggingConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredLoggingConfigurationTypeDef",
+    {
+        "ResourceArn": str,
+        "LogDestinationConfigs": Sequence[str],
+    },
+)
+_OptionalLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalLoggingConfigurationTypeDef",
+    {
+        "RedactedFields": Sequence[FieldToMatchTypeDef],
+    },
+    total=False,
+)
+
+class LoggingConfigurationTypeDef(
+    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
+):
+    pass
+
+RegexMatchTupleTypeDef = TypedDict(
+    "RegexMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "RegexPatternSetId": str,
+    },
+)
+
+SizeConstraintTypeDef = TypedDict(
+    "SizeConstraintTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Size": int,
+    },
+)
+
+SqlInjectionMatchTupleTypeDef = TypedDict(
+    "SqlInjectionMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+    },
+)
+
+XssMatchTupleTypeDef = TypedDict(
+    "XssMatchTupleTypeDef",
+    {
+        "FieldToMatch": FieldToMatchTypeDef,
+        "TextTransformation": TextTransformationType,
+    },
+)
+
+CreateWebACLMigrationStackResponseTypeDef = TypedDict(
+    "CreateWebACLMigrationStackResponseTypeDef",
+    {
+        "S3ObjectUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteByteMatchSetResponseTypeDef = TypedDict(
+    "DeleteByteMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateGeoMatchSetResponseTypeDef = TypedDict(
-    "UpdateGeoMatchSetResponseTypeDef",
+DeleteGeoMatchSetResponseTypeDef = TypedDict(
+    "DeleteGeoMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIPSetResponseTypeDef = TypedDict(
-    "UpdateIPSetResponseTypeDef",
+DeleteIPSetResponseTypeDef = TypedDict(
+    "DeleteIPSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRateBasedRuleResponseTypeDef = TypedDict(
-    "UpdateRateBasedRuleResponseTypeDef",
+DeleteRateBasedRuleResponseTypeDef = TypedDict(
+    "DeleteRateBasedRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRegexMatchSetResponseTypeDef = TypedDict(
-    "UpdateRegexMatchSetResponseTypeDef",
+DeleteRegexMatchSetResponseTypeDef = TypedDict(
+    "DeleteRegexMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRegexPatternSetResponseTypeDef = TypedDict(
-    "UpdateRegexPatternSetResponseTypeDef",
+DeleteRegexPatternSetResponseTypeDef = TypedDict(
+    "DeleteRegexPatternSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRuleGroupResponseTypeDef = TypedDict(
-    "UpdateRuleGroupResponseTypeDef",
+DeleteRuleGroupResponseTypeDef = TypedDict(
+    "DeleteRuleGroupResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
+DeleteRuleResponseTypeDef = TypedDict(
+    "DeleteRuleResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSizeConstraintSetResponseTypeDef = TypedDict(
-    "UpdateSizeConstraintSetResponseTypeDef",
+DeleteSizeConstraintSetResponseTypeDef = TypedDict(
+    "DeleteSizeConstraintSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
-    "UpdateSqlInjectionMatchSetResponseTypeDef",
+DeleteSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "DeleteSqlInjectionMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWebACLResponseTypeDef = TypedDict(
-    "UpdateWebACLResponseTypeDef",
+DeleteWebACLResponseTypeDef = TypedDict(
+    "DeleteWebACLResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateXssMatchSetResponseTypeDef = TypedDict(
-    "UpdateXssMatchSetResponseTypeDef",
+DeleteXssMatchSetResponseTypeDef = TypedDict(
+    "DeleteXssMatchSetResponseTypeDef",
     {
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActivatedRuleTypeDef = TypedDict(
-    "_RequiredActivatedRuleTypeDef",
+GetChangeTokenResponseTypeDef = TypedDict(
+    "GetChangeTokenResponseTypeDef",
     {
-        "Priority": int,
-        "RuleId": str,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalActivatedRuleTypeDef = TypedDict(
-    "_OptionalActivatedRuleTypeDef",
+
+GetChangeTokenStatusResponseTypeDef = TypedDict(
+    "GetChangeTokenStatusResponseTypeDef",
     {
-        "Action": WafActionTypeDef,
-        "OverrideAction": WafOverrideActionTypeDef,
-        "Type": WafRuleTypeType,
-        "ExcludedRules": List[ExcludedRuleTypeDef],
+        "ChangeTokenStatus": ChangeTokenStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ActivatedRuleTypeDef(_RequiredActivatedRuleTypeDef, _OptionalActivatedRuleTypeDef):
-    pass
+GetPermissionPolicyResponseTypeDef = TypedDict(
+    "GetPermissionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRateBasedRuleManagedKeysResponseTypeDef = TypedDict(
+    "GetRateBasedRuleManagedKeysResponseTypeDef",
+    {
+        "ManagedKeys": List[str],
+        "NextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListByteMatchSetsResponseTypeDef = TypedDict(
     "ListByteMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "ByteMatchSets": List[ByteMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ByteMatchTupleTypeDef = TypedDict(
-    "ByteMatchTupleTypeDef",
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingConfigurationTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationTypeDef",
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
     {
-        "ResourceArn": str,
-        "LogDestinationConfigs": List[str],
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalLoggingConfigurationTypeDef = TypedDict(
-    "_OptionalLoggingConfigurationTypeDef",
+
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class LoggingConfigurationTypeDef(
-    _RequiredLoggingConfigurationTypeDef, _OptionalLoggingConfigurationTypeDef
-):
-    pass
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RegexMatchTupleTypeDef = TypedDict(
-    "RegexMatchTupleTypeDef",
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "RegexPatternSetId": str,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SizeConstraintTypeDef = TypedDict(
-    "SizeConstraintTypeDef",
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
-        "ComparisonOperator": ComparisonOperatorType,
-        "Size": int,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SqlInjectionMatchTupleTypeDef = TypedDict(
-    "SqlInjectionMatchTupleTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-XssMatchTupleTypeDef = TypedDict(
-    "XssMatchTupleTypeDef",
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSqlInjectionMatchSetResponseTypeDef = TypedDict(
+    "UpdateSqlInjectionMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWebACLResponseTypeDef = TypedDict(
+    "UpdateWebACLResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateXssMatchSetResponseTypeDef = TypedDict(
+    "UpdateXssMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRateBasedRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -1569,40 +1493,40 @@
 )
 
 CreateRegexPatternSetResponseTypeDef = TypedDict(
     "CreateRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexPatternSetResponseTypeDef = TypedDict(
     "GetRegexPatternSetResponseTypeDef",
     {
         "RegexPatternSet": RegexPatternSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleGroupResponseTypeDef = TypedDict(
     "CreateRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleGroupResponseTypeDef = TypedDict(
     "GetRuleGroupResponseTypeDef",
     {
         "RuleGroup": RuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGeoMatchSetTypeDef = TypedDict(
     "_RequiredGeoMatchSetTypeDef",
     {
         "GeoMatchSetId": str,
@@ -1629,27 +1553,158 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
+_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
     {
-        "WebAclId": str,
         "RuleId": str,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
     },
 )
+_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef = TypedDict(
+    "_OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef(
+    _RequiredGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    _OptionalGetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+):
+    pass
+
+ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef",
+    {
+        "RuleGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef = TypedDict(
+    "ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef = TypedDict(
+    "ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef = TypedDict(
+    "ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef = TypedDict(
+    "ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef = TypedDict(
+    "ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef = TypedDict(
+    "ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = TypedDict(
+    "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "ListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef = TypedDict(
+    "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef = TypedDict(
+    "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef = TypedDict(
+    "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWebACLsRequestListWebACLsPaginateTypeDef = TypedDict(
+    "ListWebACLsRequestListWebACLsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef = TypedDict(
+    "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
         "Country": str,
         "URI": str,
@@ -1687,105 +1742,105 @@
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
 
 ListRateBasedRulesResponseTypeDef = TypedDict(
     "ListRateBasedRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "NextMarker": str,
         "Rules": List[RuleSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRegexMatchSetsResponseTypeDef = TypedDict(
     "ListRegexMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "RegexMatchSets": List[RegexMatchSetSummaryTypeDef],
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
 
 ListRuleGroupsResponseTypeDef = TypedDict(
     "ListRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[RuleGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSizeConstraintSetsResponseTypeDef = TypedDict(
     "ListSizeConstraintSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SizeConstraintSets": List[SizeConstraintSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSqlInjectionMatchSetsResponseTypeDef = TypedDict(
     "ListSqlInjectionMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "SqlInjectionMatchSets": List[SqlInjectionMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscribedRuleGroupsResponseTypeDef = TypedDict(
     "ListSubscribedRuleGroupsResponseTypeDef",
     {
         "NextMarker": str,
         "RuleGroups": List[SubscribedRuleGroupSummaryTypeDef],
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
     },
 )
 
 ListXssMatchSetsResponseTypeDef = TypedDict(
     "ListXssMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "XssMatchSets": List[XssMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRateBasedRuleTypeDef = TypedDict(
     "_RequiredRateBasedRuleTypeDef",
     {
         "RuleId": str,
@@ -1838,37 +1893,37 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
-ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
-    "ListActivatedRulesInRuleGroupResponseTypeDef",
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
     {
-        "NextMarker": str,
-        "ActivatedRules": List[ActivatedRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 
-RuleGroupUpdateTypeDef = TypedDict(
-    "RuleGroupUpdateTypeDef",
+ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
+    "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
-        "Action": ChangeActionType,
-        "ActivatedRule": ActivatedRuleTypeDef,
+        "NextMarker": str,
+        "ActivatedRules": List[ActivatedRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWebACLTypeDef = TypedDict(
     "_RequiredWebACLTypeDef",
     {
         "WebACLId": str,
         "DefaultAction": WafActionTypeDef,
-        "Rules": List[ActivatedRuleTypeDef],
+        "Rules": List[ActivatedRuleOutputTypeDef],
     },
 )
 _OptionalWebACLTypeDef = TypedDict(
     "_OptionalWebACLTypeDef",
     {
         "Name": str,
         "MetricName": str,
@@ -1876,27 +1931,35 @@
     },
     total=False,
 )
 
 class WebACLTypeDef(_RequiredWebACLTypeDef, _OptionalWebACLTypeDef):
     pass
 
+RuleGroupUpdateTypeDef = TypedDict(
+    "RuleGroupUpdateTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ActivatedRule": ActivatedRuleTypeDef,
+    },
+)
+
 WebACLUpdateTypeDef = TypedDict(
     "WebACLUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "ActivatedRule": ActivatedRuleTypeDef,
     },
 )
 
 _RequiredByteMatchSetTypeDef = TypedDict(
     "_RequiredByteMatchSetTypeDef",
     {
         "ByteMatchSetId": str,
-        "ByteMatchTuples": List[ByteMatchTupleTypeDef],
+        "ByteMatchTuples": List[ByteMatchTupleOutputTypeDef],
     },
 )
 _OptionalByteMatchSetTypeDef = TypedDict(
     "_OptionalByteMatchSetTypeDef",
     {
         "Name": str,
     },
@@ -1913,40 +1976,43 @@
         "ByteMatchTuple": ByteMatchTupleTypeDef,
     },
 )
 
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
 
-PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutLoggingConfigurationRequestRequestTypeDef",
+PutLoggingConfigurationResponseTypeDef = TypedDict(
+    "PutLoggingConfigurationResponseTypeDef",
     {
-        "LoggingConfiguration": LoggingConfigurationTypeDef,
+        "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutLoggingConfigurationResponseTypeDef = TypedDict(
-    "PutLoggingConfigurationResponseTypeDef",
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
+PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RegexMatchSetTypeDef = TypedDict(
     "RegexMatchSetTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2047,32 +2113,32 @@
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
 
 CreateGeoMatchSetResponseTypeDef = TypedDict(
     "CreateGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoMatchSetResponseTypeDef = TypedDict(
     "GetGeoMatchSetResponseTypeDef",
     {
         "GeoMatchSet": GeoMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGeoMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateGeoMatchSetRequestRequestTypeDef",
     {
         "GeoMatchSetId": str,
@@ -2104,23 +2170,23 @@
     pass
 
 CreateIPSetResponseTypeDef = TypedDict(
     "CreateIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIPSetResponseTypeDef = TypedDict(
     "GetIPSetResponseTypeDef",
     {
         "IPSet": IPSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIPSetRequestRequestTypeDef = TypedDict(
     "UpdateIPSetRequestRequestTypeDef",
     {
         "IPSetId": str,
@@ -2130,40 +2196,40 @@
 )
 
 CreateRateBasedRuleResponseTypeDef = TypedDict(
     "CreateRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRateBasedRuleResponseTypeDef = TypedDict(
     "GetRateBasedRuleResponseTypeDef",
     {
         "Rule": RateBasedRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Rule": RuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRateBasedRuleRequestRequestTypeDef = TypedDict(
     "UpdateRateBasedRuleRequestRequestTypeDef",
     {
         "RuleId": str,
@@ -2178,37 +2244,48 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
-UpdateRuleGroupRequestRequestTypeDef = TypedDict(
-    "UpdateRuleGroupRequestRequestTypeDef",
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
     {
-        "RuleGroupId": str,
-        "Updates": Sequence[RuleGroupUpdateTypeDef],
-        "ChangeToken": str,
+        "WebAclId": str,
+        "RuleId": str,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
     },
 )
 
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLResponseTypeDef = TypedDict(
     "GetWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleGroupRequestRequestTypeDef = TypedDict(
+    "UpdateRuleGroupRequestRequestTypeDef",
+    {
+        "RuleGroupId": str,
+        "Updates": Sequence[RuleGroupUpdateTypeDef],
+        "ChangeToken": str,
     },
 )
 
 _RequiredUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
@@ -2230,23 +2307,23 @@
     pass
 
 CreateByteMatchSetResponseTypeDef = TypedDict(
     "CreateByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetByteMatchSetResponseTypeDef = TypedDict(
     "GetByteMatchSetResponseTypeDef",
     {
         "ByteMatchSet": ByteMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateByteMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateByteMatchSetRequestRequestTypeDef",
     {
         "ByteMatchSetId": str,
@@ -2256,23 +2333,23 @@
 )
 
 CreateRegexMatchSetResponseTypeDef = TypedDict(
     "CreateRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegexMatchSetResponseTypeDef = TypedDict(
     "GetRegexMatchSetResponseTypeDef",
     {
         "RegexMatchSet": RegexMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRegexMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateRegexMatchSetRequestRequestTypeDef",
     {
         "RegexMatchSetId": str,
@@ -2282,23 +2359,23 @@
 )
 
 CreateSizeConstraintSetResponseTypeDef = TypedDict(
     "CreateSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSizeConstraintSetResponseTypeDef = TypedDict(
     "GetSizeConstraintSetResponseTypeDef",
     {
         "SizeConstraintSet": SizeConstraintSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSizeConstraintSetRequestRequestTypeDef = TypedDict(
     "UpdateSizeConstraintSetRequestRequestTypeDef",
     {
         "SizeConstraintSetId": str,
@@ -2308,23 +2385,23 @@
 )
 
 CreateSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "CreateSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSqlInjectionMatchSetResponseTypeDef = TypedDict(
     "GetSqlInjectionMatchSetResponseTypeDef",
     {
         "SqlInjectionMatchSet": SqlInjectionMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSqlInjectionMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateSqlInjectionMatchSetRequestRequestTypeDef",
     {
         "SqlInjectionMatchSetId": str,
@@ -2334,23 +2411,23 @@
 )
 
 CreateXssMatchSetResponseTypeDef = TypedDict(
     "CreateXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
         "ChangeToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetXssMatchSetResponseTypeDef = TypedDict(
     "GetXssMatchSetResponseTypeDef",
     {
         "XssMatchSet": XssMatchSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateXssMatchSetRequestRequestTypeDef = TypedDict(
     "UpdateXssMatchSetRequestRequestTypeDef",
     {
         "XssMatchSetId": str,
@@ -2360,11 +2437,11 @@
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
     },
 )
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/PKG-INFO` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WAF 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore waf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore waf type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-waf"></a>
 
 # types-aiobotocore-waf
 
 [![PyPI - types-aiobotocore-waf](https://img.shields.io/pypi/v/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-waf?color=blue)](https://pypistats.org/packages/types-aiobotocore-waf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf)](https://pepy.tech/project/types-aiobotocore-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [types-aiobotocore-waf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf/).
 
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
@@ -387,174 +386,178 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_waf.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_waf.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
     CreateRegexMatchSetRequestRequestTypeDef,
     CreateRegexPatternSetRequestRequestTypeDef,
     RegexPatternSetTypeDef,
     RuleGroupTypeDef,
     CreateSizeConstraintSetRequestRequestTypeDef,
     CreateSqlInjectionMatchSetRequestRequestTypeDef,
     CreateWebACLMigrationStackRequestRequestTypeDef,
-    CreateWebACLMigrationStackResponseTypeDef,
     CreateXssMatchSetRequestRequestTypeDef,
     DeleteByteMatchSetRequestRequestTypeDef,
-    DeleteByteMatchSetResponseTypeDef,
     DeleteGeoMatchSetRequestRequestTypeDef,
-    DeleteGeoMatchSetResponseTypeDef,
     DeleteIPSetRequestRequestTypeDef,
-    DeleteIPSetResponseTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeletePermissionPolicyRequestRequestTypeDef,
     DeleteRateBasedRuleRequestRequestTypeDef,
-    DeleteRateBasedRuleResponseTypeDef,
     DeleteRegexMatchSetRequestRequestTypeDef,
-    DeleteRegexMatchSetResponseTypeDef,
     DeleteRegexPatternSetRequestRequestTypeDef,
-    DeleteRegexPatternSetResponseTypeDef,
     DeleteRuleGroupRequestRequestTypeDef,
-    DeleteRuleGroupResponseTypeDef,
     DeleteRuleRequestRequestTypeDef,
-    DeleteRuleResponseTypeDef,
     DeleteSizeConstraintSetRequestRequestTypeDef,
-    DeleteSizeConstraintSetResponseTypeDef,
     DeleteSqlInjectionMatchSetRequestRequestTypeDef,
-    DeleteSqlInjectionMatchSetResponseTypeDef,
     DeleteWebACLRequestRequestTypeDef,
-    DeleteWebACLResponseTypeDef,
     DeleteXssMatchSetRequestRequestTypeDef,
-    DeleteXssMatchSetResponseTypeDef,
     GeoMatchConstraintTypeDef,
     GeoMatchSetSummaryTypeDef,
     GetByteMatchSetRequestRequestTypeDef,
-    GetChangeTokenResponseTypeDef,
     GetChangeTokenStatusRequestRequestTypeDef,
-    GetChangeTokenStatusResponseTypeDef,
     GetGeoMatchSetRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
-    GetPermissionPolicyResponseTypeDef,
-    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
-    GetRateBasedRuleManagedKeysResponseTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     IPSetDescriptorTypeDef,
     IPSetSummaryTypeDef,
-    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
     ListActivatedRulesInRuleGroupRequestRequestTypeDef,
-    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
     ListByteMatchSetsRequestRequestTypeDef,
-    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
     ListGeoMatchSetsRequestRequestTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
-    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
-    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
-    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
-    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
-    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
-    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestRequestTypeDef,
     SubscribedRuleGroupSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
-    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ActivatedRuleOutputTypeDef,
+    ActivatedRuleTypeDef,
+    ByteMatchTupleOutputTypeDef,
+    ByteMatchTupleTypeDef,
+    LoggingConfigurationOutputTypeDef,
+    LoggingConfigurationTypeDef,
+    RegexMatchTupleTypeDef,
+    SizeConstraintTypeDef,
+    SqlInjectionMatchTupleTypeDef,
+    XssMatchTupleTypeDef,
+    CreateWebACLMigrationStackResponseTypeDef,
+    DeleteByteMatchSetResponseTypeDef,
+    DeleteGeoMatchSetResponseTypeDef,
+    DeleteIPSetResponseTypeDef,
+    DeleteRateBasedRuleResponseTypeDef,
+    DeleteRegexMatchSetResponseTypeDef,
+    DeleteRegexPatternSetResponseTypeDef,
+    DeleteRuleGroupResponseTypeDef,
+    DeleteRuleResponseTypeDef,
+    DeleteSizeConstraintSetResponseTypeDef,
+    DeleteSqlInjectionMatchSetResponseTypeDef,
+    DeleteWebACLResponseTypeDef,
+    DeleteXssMatchSetResponseTypeDef,
+    GetChangeTokenResponseTypeDef,
+    GetChangeTokenStatusResponseTypeDef,
+    GetPermissionPolicyResponseTypeDef,
+    GetRateBasedRuleManagedKeysResponseTypeDef,
+    ListByteMatchSetsResponseTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateSizeConstraintSetResponseTypeDef,
     UpdateSqlInjectionMatchSetResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     UpdateXssMatchSetResponseTypeDef,
-    ActivatedRuleTypeDef,
-    ListByteMatchSetsResponseTypeDef,
-    ByteMatchTupleTypeDef,
-    LoggingConfigurationTypeDef,
-    RegexMatchTupleTypeDef,
-    SizeConstraintTypeDef,
-    SqlInjectionMatchTupleTypeDef,
-    XssMatchTupleTypeDef,
     CreateRateBasedRuleRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     TagInfoForResourceTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
+    GetRateBasedRuleManagedKeysRequestGetRateBasedRuleManagedKeysPaginateTypeDef,
+    ListActivatedRulesInRuleGroupRequestListActivatedRulesInRuleGroupPaginateTypeDef,
+    ListByteMatchSetsRequestListByteMatchSetsPaginateTypeDef,
+    ListGeoMatchSetsRequestListGeoMatchSetsPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListLoggingConfigurationsRequestListLoggingConfigurationsPaginateTypeDef,
+    ListRateBasedRulesRequestListRateBasedRulesPaginateTypeDef,
+    ListRegexMatchSetsRequestListRegexMatchSetsPaginateTypeDef,
+    ListRegexPatternSetsRequestListRegexPatternSetsPaginateTypeDef,
+    ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
+    ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
+    ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
+    ListWebACLsRequestListWebACLsPaginateTypeDef,
+    ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListRegexMatchSetsResponseTypeDef,
@@ -565,24 +568,26 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
-    RuleGroupUpdateTypeDef,
     WebACLTypeDef,
+    RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
     ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
-    PutLoggingConfigurationRequestRequestTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
+    PutLoggingConfigurationRequestRequestTypeDef,
     RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     XssMatchSetTypeDef,
@@ -597,17 +602,19 @@
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleGroupRequestRequestTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
+    UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
     UpdateByteMatchSetRequestRequestTypeDef,
     CreateRegexMatchSetResponseTypeDef,
     GetRegexMatchSetResponseTypeDef,
     UpdateRegexMatchSetRequestRequestTypeDef,
@@ -620,15 +627,15 @@
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_value() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-waf-2.5.2/types_aiobotocore_waf.egg-info/SOURCES.txt` & `types-aiobotocore-waf-2.5.2.post1/types_aiobotocore_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


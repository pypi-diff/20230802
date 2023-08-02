# Comparing `tmp/types-aiobotocore-waf-regional-2.5.2.tar.gz` & `tmp/types-aiobotocore-waf-regional-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-waf-regional-2.5.2.tar", last modified: Sat Jul  8 01:44:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-waf-regional-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
```

## Comparing `types-aiobotocore-waf-regional-2.5.2.tar` & `types-aiobotocore-waf-regional-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.411033 types-aiobotocore-waf-regional-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-07-08 01:44:27.411033 types-aiobotocore-waf-regional-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:27.411033 types-aiobotocore-waf-regional-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.411033 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49296 2023-07-08 01:42:22.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49206 2023-07-08 01:42:22.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-08 01:42:22.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-07-08 01:42:22.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55506 2023-07-08 01:42:23.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55459 2023-07-08 01:42:23.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:21.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.411033 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-07-08 01:44:27.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-08 01:44:27.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:27.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:44:27.000000 types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.309430 types-aiobotocore-waf-regional-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-02 14:53:09.301430 types-aiobotocore-waf-regional-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.309430 types-aiobotocore-waf-regional-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:50:57.000000 types-aiobotocore-waf-regional-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.301430 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49316 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49226 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57536 2023-08-02 14:50:59.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57485 2023-08-02 14:50:59.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:58.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.301430 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:53:09.000000 types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-waf-regional-2.5.2/LICENSE` & `types-aiobotocore-waf-regional-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2/PKG-INFO` & `types-aiobotocore-waf-regional-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-waf-regional
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore waf-regional type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore waf-regional type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-waf-regional"></a>
 
 # types-aiobotocore-waf-regional
 
 [![PyPI - types-aiobotocore-waf-regional](https://img.shields.io/pypi/v/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-waf-regional?color=blue)](https://pypistats.org/packages/types-aiobotocore-waf-regional)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf-regional)](https://pepy.tech/project/types-aiobotocore-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAFRegional 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [types-aiobotocore-waf-regional docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/).
 
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
@@ -295,88 +294,73 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_waf_regional.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_waf_regional.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
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
     DisassociateWebACLRequestRequestTypeDef,
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
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
@@ -390,15 +374,14 @@
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
@@ -407,50 +390,70 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
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
+    ListResourcesForWebACLResponseTypeDef,
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
     GetWebACLForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
@@ -462,24 +465,26 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
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
@@ -494,17 +499,19 @@
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
@@ -517,15 +524,15 @@
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

### Comparing `types-aiobotocore-waf-regional-2.5.2/README.md` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-waf-regional
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore waf-regional type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-waf-regional"></a>
 
 # types-aiobotocore-waf-regional
 
 [![PyPI - types-aiobotocore-waf-regional](https://img.shields.io/pypi/v/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-waf-regional?color=blue)](https://pypistats.org/packages/types-aiobotocore-waf-regional)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf-regional)](https://pepy.tech/project/types-aiobotocore-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAFRegional 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [types-aiobotocore-waf-regional docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +72,15 @@
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
@@ -262,88 +294,73 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_waf_regional.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_waf_regional.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
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
     DisassociateWebACLRequestRequestTypeDef,
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
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
@@ -357,15 +374,14 @@
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
@@ -374,50 +390,70 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
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
+    ListResourcesForWebACLResponseTypeDef,
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
     GetWebACLForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
@@ -429,24 +465,26 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
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
@@ -461,17 +499,19 @@
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
@@ -484,15 +524,15 @@
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

### Comparing `types-aiobotocore-waf-regional-2.5.2/setup.py` & `types-aiobotocore-waf-regional-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-waf-regional",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with"
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
-    keywords="aiobotocore waf-regional type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore waf-regional type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_waf_regional": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/"
```

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/__main__.py` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WAFRegional 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WAFRegional 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
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

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/client.py` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,24 +82,24 @@
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
@@ -602,15 +602,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_rule_group)
         """
 
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_sampled_requests)
         """
@@ -828,15 +828,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#list_xss_match_sets)
         """
 
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/client.pyi` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,24 +82,24 @@
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_rule_group)
         """
     async def get_sampled_requests(
-        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowTypeDef, MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#get_sampled_requests)
         """
@@ -755,15 +755,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#list_xss_match_sets)
         """
     async def put_logging_configuration(
-        self, *, LoggingConfiguration: LoggingConfigurationTypeDef
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/literals.py` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/literals.pyi` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/type_defs.py` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_waf_regional.type_defs import ExcludedRuleTypeDef
 
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
@@ -42,75 +44,60 @@
 
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
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
     "DisassociateWebACLRequestRequestTypeDef",
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
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
@@ -124,15 +111,14 @@
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
@@ -141,50 +127,70 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
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
+    "ListResourcesForWebACLResponseTypeDef",
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
     "GetWebACLForResourceResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
@@ -196,24 +202,26 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
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
@@ -228,17 +236,19 @@
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
@@ -279,14 +289,15 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ResourceArn": str,
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
@@ -314,14 +325,25 @@
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
@@ -419,22 +441,14 @@
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
@@ -443,54 +457,30 @@
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
 
@@ -505,150 +495,78 @@
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
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -671,37 +589,21 @@
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
 
@@ -722,22 +624,14 @@
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
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -752,23 +646,14 @@
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
 
@@ -796,19 +681,19 @@
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
@@ -991,22 +876,14 @@
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
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1151,225 +1028,417 @@
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
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
+        "ResourceArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingConfigurationTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationTypeDef",
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
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
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
     {
-        "RedactedFields": List[FieldToMatchTypeDef],
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
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
 
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RegexMatchTupleTypeDef = TypedDict(
-    "RegexMatchTupleTypeDef",
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
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
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
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
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-XssMatchTupleTypeDef = TypedDict(
-    "XssMatchTupleTypeDef",
+UpdateSizeConstraintSetResponseTypeDef = TypedDict(
+    "UpdateSizeConstraintSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
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
@@ -1483,40 +1552,40 @@
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
@@ -1545,42 +1614,32 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclId": str,
-        "RuleId": str,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
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
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1622,96 +1681,96 @@
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
@@ -1768,37 +1827,37 @@
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
@@ -1808,27 +1867,35 @@
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
@@ -1847,40 +1914,43 @@
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
@@ -1987,32 +2057,32 @@
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
@@ -2046,23 +2116,23 @@
 
 
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
@@ -2072,40 +2142,40 @@
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
@@ -2120,37 +2190,48 @@
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
@@ -2174,23 +2255,23 @@
 
 
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
@@ -2200,23 +2281,23 @@
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
@@ -2226,23 +2307,23 @@
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
@@ -2252,23 +2333,23 @@
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
@@ -2278,23 +2359,23 @@
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
@@ -2304,11 +2385,11 @@
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

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional/type_defs.pyi` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_waf_regional.type_defs import ExcludedRuleTypeDef
 
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
@@ -41,75 +43,60 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
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
     "DisassociateWebACLRequestRequestTypeDef",
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
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
@@ -123,15 +110,14 @@
     "ListRateBasedRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
     "ListRegexMatchSetsRequestRequestTypeDef",
     "RegexMatchSetSummaryTypeDef",
     "ListRegexPatternSetsRequestRequestTypeDef",
     "RegexPatternSetSummaryTypeDef",
     "ListResourcesForWebACLRequestRequestTypeDef",
-    "ListResourcesForWebACLResponseTypeDef",
     "ListRuleGroupsRequestRequestTypeDef",
     "RuleGroupSummaryTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListSizeConstraintSetsRequestRequestTypeDef",
     "SizeConstraintSetSummaryTypeDef",
     "ListSqlInjectionMatchSetsRequestRequestTypeDef",
     "SqlInjectionMatchSetSummaryTypeDef",
@@ -140,50 +126,70 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
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
+    "ListResourcesForWebACLResponseTypeDef",
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
     "GetWebACLForResourceResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
@@ -195,24 +201,26 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
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
@@ -227,17 +235,19 @@
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
@@ -278,14 +288,15 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ResourceArn": str,
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
@@ -311,14 +322,25 @@
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
@@ -412,22 +434,14 @@
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
@@ -436,54 +450,30 @@
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
 
@@ -498,150 +488,78 @@
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
 DisassociateWebACLRequestRequestTypeDef = TypedDict(
     "DisassociateWebACLRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -664,37 +582,21 @@
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
 
@@ -715,22 +617,14 @@
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
 _RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
     "_RequiredGetRateBasedRuleManagedKeysRequestRequestTypeDef",
     {
         "RuleId": str,
     },
 )
 _OptionalGetRateBasedRuleManagedKeysRequestRequestTypeDef = TypedDict(
@@ -743,23 +637,14 @@
 
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
 
@@ -787,19 +672,19 @@
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
@@ -980,22 +865,14 @@
 
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
 ListRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListRuleGroupsRequestRequestTypeDef",
     {
         "NextMarker": str,
         "Limit": int,
     },
     total=False,
@@ -1138,221 +1015,409 @@
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
+ListResourcesForWebACLResponseTypeDef = TypedDict(
+    "ListResourcesForWebACLResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": bytes,
-        "TextTransformation": TextTransformationType,
-        "PositionalConstraint": PositionalConstraintType,
+        "ResourceArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingConfigurationTypeDef = TypedDict(
-    "_RequiredLoggingConfigurationTypeDef",
+UpdateByteMatchSetResponseTypeDef = TypedDict(
+    "UpdateByteMatchSetResponseTypeDef",
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
+UpdateGeoMatchSetResponseTypeDef = TypedDict(
+    "UpdateGeoMatchSetResponseTypeDef",
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
+UpdateIPSetResponseTypeDef = TypedDict(
+    "UpdateIPSetResponseTypeDef",
+    {
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RegexMatchTupleTypeDef = TypedDict(
-    "RegexMatchTupleTypeDef",
+UpdateRateBasedRuleResponseTypeDef = TypedDict(
+    "UpdateRateBasedRuleResponseTypeDef",
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
+UpdateRegexMatchSetResponseTypeDef = TypedDict(
+    "UpdateRegexMatchSetResponseTypeDef",
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
+UpdateRegexPatternSetResponseTypeDef = TypedDict(
+    "UpdateRegexPatternSetResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-XssMatchTupleTypeDef = TypedDict(
-    "XssMatchTupleTypeDef",
+UpdateRuleGroupResponseTypeDef = TypedDict(
+    "UpdateRuleGroupResponseTypeDef",
     {
-        "FieldToMatch": FieldToMatchTypeDef,
-        "TextTransformation": TextTransformationType,
+        "ChangeToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
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
@@ -1458,40 +1523,40 @@
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
@@ -1518,42 +1583,32 @@
 )
 
 ListGeoMatchSetsResponseTypeDef = TypedDict(
     "ListGeoMatchSetsResponseTypeDef",
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclId": str,
-        "RuleId": str,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
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
 
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
@@ -1593,96 +1648,96 @@
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
@@ -1735,37 +1790,37 @@
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
@@ -1773,27 +1828,35 @@
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
@@ -1810,40 +1873,43 @@
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
@@ -1944,32 +2010,32 @@
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
@@ -2001,23 +2067,23 @@
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
@@ -2027,40 +2093,40 @@
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
@@ -2075,37 +2141,48 @@
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
@@ -2127,23 +2204,23 @@
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
@@ -2153,23 +2230,23 @@
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
@@ -2179,23 +2256,23 @@
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
@@ -2205,23 +2282,23 @@
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
@@ -2231,23 +2308,23 @@
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
@@ -2257,11 +2334,11 @@
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

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/PKG-INFO` & `types-aiobotocore-waf-regional-2.5.2.post1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-waf-regional
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WAFRegional 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore waf-regional type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-waf-regional"></a>
 
 # types-aiobotocore-waf-regional
 
 [![PyPI - types-aiobotocore-waf-regional](https://img.shields.io/pypi/v/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-waf-regional.svg?color=blue)](https://pypi.org/project/types-aiobotocore-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-waf-regional?color=blue)](https://pypistats.org/packages/types-aiobotocore-waf-regional)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-waf-regional)](https://pepy.tech/project/types-aiobotocore-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WAFRegional 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [types-aiobotocore-waf-regional docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_waf_regional/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +40,15 @@
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
@@ -295,88 +262,73 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_waf_regional.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_waf_regional.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
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
     DisassociateWebACLRequestRequestTypeDef,
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
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
@@ -390,15 +342,14 @@
     ListRateBasedRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
     ListRegexMatchSetsRequestRequestTypeDef,
     RegexMatchSetSummaryTypeDef,
     ListRegexPatternSetsRequestRequestTypeDef,
     RegexPatternSetSummaryTypeDef,
     ListResourcesForWebACLRequestRequestTypeDef,
-    ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsRequestRequestTypeDef,
     RuleGroupSummaryTypeDef,
     ListRulesRequestRequestTypeDef,
     ListSizeConstraintSetsRequestRequestTypeDef,
     SizeConstraintSetSummaryTypeDef,
     ListSqlInjectionMatchSetsRequestRequestTypeDef,
     SqlInjectionMatchSetSummaryTypeDef,
@@ -407,50 +358,70 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
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
+    ListResourcesForWebACLResponseTypeDef,
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
     GetWebACLForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
@@ -462,24 +433,26 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
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
@@ -494,17 +467,19 @@
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
@@ -517,15 +492,15 @@
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

### Comparing `types-aiobotocore-waf-regional-2.5.2/types_aiobotocore_waf_regional.egg-info/SOURCES.txt` & `types-aiobotocore-waf-regional-2.5.2.post1/types_aiobotocore_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*


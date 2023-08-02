# Comparing `tmp/types-aiobotocore-billingconductor-2.5.2.tar.gz` & `tmp/types-aiobotocore-billingconductor-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-billingconductor-2.5.2.tar", last modified: Sat Jul  8 01:43:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-billingconductor-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-billingconductor-2.5.2.tar` & `types-aiobotocore-billingconductor-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.293764 types-aiobotocore-billingconductor-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-07-08 01:43:18.289764 types-aiobotocore-billingconductor-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:18.293764 types-aiobotocore-billingconductor-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.289764 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33540 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42812 2023-07-08 01:26:24.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42765 2023-07-08 01:26:24.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:23.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.289764 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-07-08 01:43:18.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:43:18.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:18.000000 types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20795 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.485643 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33540 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-08-02 14:33:51.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42685 2023-08-02 14:33:51.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:50.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.493643 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20795 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:51:57.000000 types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/LICENSE` & `types-aiobotocore-billingconductor-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/PKG-INFO` & `types-aiobotocore-billingconductor-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-billingconductor
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore billingconductor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore billingconductor type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-billingconductor"></a>
 
 # types-aiobotocore-billingconductor
 
 [![PyPI - types-aiobotocore-billingconductor](https://img.shields.io/pypi/v/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-billingconductor?color=blue)](https://pypistats.org/packages/types-aiobotocore-billingconductor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BillingConductor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [types-aiobotocore-billingconductor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/).
 
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
@@ -360,98 +359,98 @@
 )
 
 
 def check_value(value: AssociateResourceErrorReasonType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_billingconductor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
-    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
-    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
-    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
-    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    UpdatePricingPlanOutputTypeDef,
+    AssociateAccountsOutputTypeDef,
+    AssociatePricingRulesOutputTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
+    DeletePricingPlanOutputTypeDef,
+    DeletePricingRuleOutputTypeDef,
+    DisassociateAccountsOutputTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     ListAccountAssociationsOutputTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateBillingGroupOutputTypeDef,
+    UpdatePricingPlanOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     UpdateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
     ListAccountAssociationsInputRequestTypeDef,
+    ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
@@ -482,15 +481,15 @@
     UpdatePricingRuleOutputTypeDef,
     ListPricingRulesOutputTypeDef,
     ListCustomLineItemsOutputTypeDef,
     ListCustomLineItemVersionsOutputTypeDef,
 )
 
 
-def get_structure() -> AccountAssociationsListElementTypeDef:
+def get_value() -> AccountAssociationsListElementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/README.md` & `types-aiobotocore-billingconductor-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-billingconductor"></a>
 
 # types-aiobotocore-billingconductor
 
 [![PyPI - types-aiobotocore-billingconductor](https://img.shields.io/pypi/v/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-billingconductor?color=blue)](https://pypistats.org/packages/types-aiobotocore-billingconductor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BillingConductor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [types-aiobotocore-billingconductor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/).
 
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
@@ -327,98 +327,98 @@
 )
 
 
 def check_value(value: AssociateResourceErrorReasonType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_billingconductor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
-    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
-    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
-    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
-    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    UpdatePricingPlanOutputTypeDef,
+    AssociateAccountsOutputTypeDef,
+    AssociatePricingRulesOutputTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
+    DeletePricingPlanOutputTypeDef,
+    DeletePricingRuleOutputTypeDef,
+    DisassociateAccountsOutputTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     ListAccountAssociationsOutputTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateBillingGroupOutputTypeDef,
+    UpdatePricingPlanOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     UpdateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
     ListAccountAssociationsInputRequestTypeDef,
+    ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
@@ -449,15 +449,15 @@
     UpdatePricingRuleOutputTypeDef,
     ListPricingRulesOutputTypeDef,
     ListCustomLineItemsOutputTypeDef,
     ListCustomLineItemVersionsOutputTypeDef,
 )
 
 
-def get_structure() -> AccountAssociationsListElementTypeDef:
+def get_value() -> AccountAssociationsListElementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/setup.py` & `types-aiobotocore-billingconductor-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-billingconductor",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with"
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
-    keywords="aiobotocore billingconductor type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore billingconductor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_billingconductor": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/"
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/__init__.py` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/__init__.pyi` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/__main__.py` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BillingConductor 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.BillingConductor 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor\nOther"
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

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/client.py` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/client.pyi` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/literals.py` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/literals.pyi` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/paginator.py` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 
@@ -115,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 
@@ -134,15 +134,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 
@@ -153,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomLineItemVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 
@@ -172,15 +172,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomLineItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 
@@ -191,15 +191,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 
@@ -210,15 +210,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 
@@ -229,15 +229,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 
@@ -248,15 +248,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 
@@ -268,13 +268,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/paginator.pyi` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 class ListBillingGroupCostReportsPaginator(AioPaginator):
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 class ListBillingGroupsPaginator(AioPaginator):
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 class ListCustomLineItemVersionsPaginator(AioPaginator):
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomLineItemVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 class ListCustomLineItemsPaginator(AioPaginator):
@@ -165,15 +165,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomLineItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 class ListPricingPlansPaginator(AioPaginator):
@@ -183,15 +183,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 class ListPricingPlansAssociatedWithPricingRulePaginator(AioPaginator):
@@ -201,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 class ListPricingRulesPaginator(AioPaginator):
@@ -219,15 +219,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 class ListPricingRulesAssociatedToPricingPlanPaginator(AioPaginator):
@@ -237,15 +237,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 class ListResourcesAssociatedToCustomLineItemPaginator(AioPaginator):
@@ -256,13 +256,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/type_defs.py` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_billingconductor.type_defs import AccountAssociationsListElementTypeDef
 
-    data: AccountAssociationsListElementTypeDef = {...}
+    data: AccountAssociationsListElementTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AssociateResourceErrorReasonType,
@@ -30,86 +30,86 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
-    "AssociateAccountsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
-    "AssociatePricingRulesOutputTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceTypeDef",
-    "CreateBillingGroupOutputTypeDef",
-    "CreateCustomLineItemOutputTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
-    "CreatePricingPlanOutputTypeDef",
-    "CreatePricingRuleOutputTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
-    "DeleteBillingGroupOutputTypeDef",
-    "DeleteCustomLineItemOutputTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
-    "DeletePricingPlanOutputTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
-    "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsInputRequestTypeDef",
-    "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesInputRequestTypeDef",
-    "DisassociatePricingRulesOutputTypeDef",
     "FreeTierConfigTypeDef",
     "ListAccountAssociationsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBillingGroupCostReportsFilterTypeDef",
     "ListBillingGroupsFilterTypeDef",
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     "ListCustomLineItemPercentageChargeDetailsTypeDef",
     "ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef",
     "ListCustomLineItemsFilterTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingPlansFilterTypeDef",
     "PricingPlanListElementTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateBillingGroupOutputTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
-    "UpdatePricingPlanOutputTypeDef",
+    "AssociateAccountsOutputTypeDef",
+    "AssociatePricingRulesOutputTypeDef",
+    "CreateBillingGroupOutputTypeDef",
+    "CreateCustomLineItemOutputTypeDef",
+    "CreatePricingPlanOutputTypeDef",
+    "CreatePricingRuleOutputTypeDef",
+    "DeleteBillingGroupOutputTypeDef",
+    "DeleteCustomLineItemOutputTypeDef",
+    "DeletePricingPlanOutputTypeDef",
+    "DeletePricingRuleOutputTypeDef",
+    "DisassociateAccountsOutputTypeDef",
+    "DisassociatePricingRulesOutputTypeDef",
     "ListAccountAssociationsOutputTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateBillingGroupOutputTypeDef",
+    "UpdatePricingPlanOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
     "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
     "UpdateBillingGroupInputRequestTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
-    "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     "ListAccountAssociationsInputRequestTypeDef",
+    "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     "ListBillingGroupCostReportsInputRequestTypeDef",
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsInputRequestTypeDef",
     "ListCustomLineItemChargeDetailsTypeDef",
     "ListCustomLineItemVersionsFilterTypeDef",
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
@@ -165,38 +165,33 @@
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-AssociateAccountsOutputTypeDef = TypedDict(
-    "AssociateAccountsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociatePricingRulesInputRequestTypeDef = TypedDict(
     "AssociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
-AssociatePricingRulesOutputTypeDef = TypedDict(
-    "AssociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateResourceErrorTypeDef = TypedDict(
     "AssociateResourceErrorTypeDef",
     {
         "Message": str,
         "Reason": AssociateResourceErrorReasonType,
     },
     total=False,
@@ -240,30 +235,14 @@
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
-CreateBillingGroupOutputTypeDef = TypedDict(
-    "CreateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomLineItemOutputTypeDef = TypedDict(
-    "CreateCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -287,30 +266,14 @@
 
 class CreatePricingPlanInputRequestTypeDef(
     _RequiredCreatePricingPlanInputRequestTypeDef, _OptionalCreatePricingPlanInputRequestTypeDef
 ):
     pass
 
 
-CreatePricingPlanOutputTypeDef = TypedDict(
-    "CreatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePricingRuleOutputTypeDef = TypedDict(
-    "CreatePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "CustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -339,92 +302,44 @@
 DeleteBillingGroupInputRequestTypeDef = TypedDict(
     "DeleteBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteBillingGroupOutputTypeDef = TypedDict(
-    "DeleteBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteCustomLineItemOutputTypeDef = TypedDict(
-    "DeleteCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePricingPlanInputRequestTypeDef = TypedDict(
     "DeletePricingPlanInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeletePricingPlanOutputTypeDef = TypedDict(
-    "DeletePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePricingRuleInputRequestTypeDef = TypedDict(
     "DeletePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeletePricingRuleOutputTypeDef = TypedDict(
-    "DeletePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateAccountsInputRequestTypeDef = TypedDict(
     "DisassociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-DisassociateAccountsOutputTypeDef = TypedDict(
-    "DisassociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociatePricingRulesInputRequestTypeDef = TypedDict(
     "DisassociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
-DisassociatePricingRulesOutputTypeDef = TypedDict(
-    "DisassociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FreeTierConfigTypeDef = TypedDict(
     "FreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -434,14 +349,24 @@
         "Association": str,
         "AccountId": str,
         "AccountIds": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ListBillingGroupCostReportsFilterTypeDef = TypedDict(
     "ListBillingGroupCostReportsFilterTypeDef",
     {
         "BillingGroupArns": Sequence[str],
     },
     total=False,
 )
@@ -485,37 +410,14 @@
         "Names": Sequence[str],
         "BillingGroups": Sequence[str],
         "Arns": Sequence[str],
     },
     total=False,
 )
 
-_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "PricingRuleArn": str,
-    },
-)
-_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
-    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
     {
         "PricingRuleArn": str,
     },
 )
 _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
@@ -532,25 +434,14 @@
 class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(
     _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
     _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
 ):
     pass
 
 
-ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingRuleArn": str,
-        "PricingPlanArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPricingPlansFilterTypeDef = TypedDict(
     "ListPricingPlansFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -564,37 +455,14 @@
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
     },
     total=False,
 )
 
-_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "PricingPlanArn": str,
-    },
-)
-_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
-    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
     "_RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
@@ -611,25 +479,14 @@
 class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(
     _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
     _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
 ):
     pass
 
 
-ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingPlanArn": str,
-        "PricingRuleArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPricingRulesFilterTypeDef = TypedDict(
     "ListPricingRulesFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -655,43 +512,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -700,30 +528,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateBillingGroupOutputTypeDef = TypedDict(
-    "UpdateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "PrimaryAccountId": str,
-        "PricingPlanArn": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -759,32 +571,174 @@
 
 class UpdatePricingPlanInputRequestTypeDef(
     _RequiredUpdatePricingPlanInputRequestTypeDef, _OptionalUpdatePricingPlanInputRequestTypeDef
 ):
     pass
 
 
-UpdatePricingPlanOutputTypeDef = TypedDict(
-    "UpdatePricingPlanOutputTypeDef",
+AssociateAccountsOutputTypeDef = TypedDict(
+    "AssociateAccountsOutputTypeDef",
     {
         "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociatePricingRulesOutputTypeDef = TypedDict(
+    "AssociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBillingGroupOutputTypeDef = TypedDict(
+    "CreateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomLineItemOutputTypeDef = TypedDict(
+    "CreateCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePricingPlanOutputTypeDef = TypedDict(
+    "CreatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePricingRuleOutputTypeDef = TypedDict(
+    "CreatePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBillingGroupOutputTypeDef = TypedDict(
+    "DeleteBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomLineItemOutputTypeDef = TypedDict(
+    "DeleteCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePricingPlanOutputTypeDef = TypedDict(
+    "DeletePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePricingRuleOutputTypeDef = TypedDict(
+    "DeletePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateAccountsOutputTypeDef = TypedDict(
+    "DisassociateAccountsOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociatePricingRulesOutputTypeDef = TypedDict(
+    "DisassociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountAssociationsOutputTypeDef = TypedDict(
     "ListAccountAssociationsOutputTypeDef",
     {
         "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingRuleArn": str,
+        "PricingPlanArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingPlanArn": str,
+        "PricingRuleArns": List[str],
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
+    },
+)
+
+UpdateBillingGroupOutputTypeDef = TypedDict(
+    "UpdateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "PrimaryAccountId": str,
+        "PricingPlanArn": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePricingPlanOutputTypeDef = TypedDict(
+    "UpdatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResourceResponseElementTypeDef = TypedDict(
     "AssociateResourceResponseElementTypeDef",
     {
         "Arn": str,
@@ -871,15 +825,15 @@
 
 
 ListBillingGroupCostReportsOutputTypeDef = TypedDict(
     "ListBillingGroupCostReportsOutputTypeDef",
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BillingGroupListElementTypeDef = TypedDict(
     "BillingGroupListElementTypeDef",
     {
         "Name": str,
@@ -978,40 +932,86 @@
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "FreeTier": FreeTierConfigTypeDef,
     },
 )
 
+ListAccountAssociationsInputRequestTypeDef = TypedDict(
+    "ListAccountAssociationsInputRequestTypeDef",
+    {
+        "BillingPeriod": str,
+        "Filters": ListAccountAssociationsFilterTypeDef,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef = TypedDict(
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListAccountAssociationsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAccountAssociationsInputRequestTypeDef = TypedDict(
-    "ListAccountAssociationsInputRequestTypeDef",
+_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "PricingRuleArn": str,
+    },
+)
+_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     {
         "BillingPeriod": str,
-        "Filters": ListAccountAssociationsFilterTypeDef,
-        "NextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
+    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "PricingPlanArn": str,
+    },
+)
+_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
+    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+):
+    pass
+
+
 ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupCostReportsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListBillingGroupCostReportsInputRequestTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputRequestTypeDef",
     {
@@ -1024,15 +1024,15 @@
 )
 
 ListBillingGroupsInputListBillingGroupsPaginateTypeDef = TypedDict(
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListBillingGroupsInputRequestTypeDef = TypedDict(
     "ListBillingGroupsInputRequestTypeDef",
     {
@@ -1075,15 +1075,15 @@
 )
 
 ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef = TypedDict(
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListCustomLineItemsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCustomLineItemsInputRequestTypeDef = TypedDict(
     "ListCustomLineItemsInputRequestTypeDef",
     {
@@ -1096,15 +1096,15 @@
 )
 
 ListPricingPlansInputListPricingPlansPaginateTypeDef = TypedDict(
     "ListPricingPlansInputListPricingPlansPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingPlansFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPricingPlansInputRequestTypeDef = TypedDict(
     "ListPricingPlansInputRequestTypeDef",
     {
@@ -1118,24 +1118,24 @@
 
 ListPricingPlansOutputTypeDef = TypedDict(
     "ListPricingPlansOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingPlans": List[PricingPlanListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPricingRulesInputListPricingRulesPaginateTypeDef = TypedDict(
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingRulesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPricingRulesInputRequestTypeDef = TypedDict(
     "ListPricingRulesInputRequestTypeDef",
     {
@@ -1154,15 +1154,15 @@
     },
 )
 _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef = TypedDict(
     "_OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListResourcesAssociatedToCustomLineItemFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef(
     _RequiredListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
@@ -1198,15 +1198,15 @@
 
 ListResourcesAssociatedToCustomLineItemOutputTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomLineItemChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": UpdateCustomLineItemFlatChargeDetailsTypeDef,
@@ -1223,33 +1223,33 @@
 )
 
 BatchAssociateResourcesToCustomLineItemOutputTypeDef = TypedDict(
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     {
         "SuccessfullyAssociatedResources": List[AssociateResourceResponseElementTypeDef],
         "FailedAssociatedResources": List[AssociateResourceResponseElementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateResourcesFromCustomLineItemOutputTypeDef = TypedDict(
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     {
         "SuccessfullyDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
         "FailedDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBillingGroupsOutputTypeDef = TypedDict(
     "ListBillingGroupsOutputTypeDef",
     {
         "BillingGroups": List[BillingGroupListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreatePricingRuleInputRequestTypeDef",
     {
         "Name": str,
@@ -1371,29 +1371,29 @@
         "Arn": str,
         "BillingGroupArn": str,
         "Name": str,
         "Description": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
         "LastModifiedTime": int,
         "AssociationSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Filters": ListCustomLineItemVersionsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef(
     _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
@@ -1488,38 +1488,38 @@
         "Service": str,
         "AssociatedPricingPlanCount": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": UpdateTieringInputTypeDef,
         "UsageType": str,
         "Operation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPricingRulesOutputTypeDef = TypedDict(
     "ListPricingRulesOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingRules": List[PricingRuleListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomLineItemsOutputTypeDef = TypedDict(
     "ListCustomLineItemsOutputTypeDef",
     {
         "CustomLineItems": List[CustomLineItemListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomLineItemVersionsOutputTypeDef = TypedDict(
     "ListCustomLineItemVersionsOutputTypeDef",
     {
         "CustomLineItemVersions": List[CustomLineItemVersionListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor/type_defs.pyi` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_billingconductor.type_defs import AccountAssociationsListElementTypeDef
 
-    data: AccountAssociationsListElementTypeDef = {...}
+    data: AccountAssociationsListElementTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AssociateResourceErrorReasonType,
@@ -29,86 +29,86 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
-    "AssociateAccountsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
-    "AssociatePricingRulesOutputTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceTypeDef",
-    "CreateBillingGroupOutputTypeDef",
-    "CreateCustomLineItemOutputTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
-    "CreatePricingPlanOutputTypeDef",
-    "CreatePricingRuleOutputTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
-    "DeleteBillingGroupOutputTypeDef",
-    "DeleteCustomLineItemOutputTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
-    "DeletePricingPlanOutputTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
-    "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsInputRequestTypeDef",
-    "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesInputRequestTypeDef",
-    "DisassociatePricingRulesOutputTypeDef",
     "FreeTierConfigTypeDef",
     "ListAccountAssociationsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBillingGroupCostReportsFilterTypeDef",
     "ListBillingGroupsFilterTypeDef",
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     "ListCustomLineItemPercentageChargeDetailsTypeDef",
     "ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef",
     "ListCustomLineItemsFilterTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingPlansFilterTypeDef",
     "PricingPlanListElementTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateBillingGroupOutputTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
-    "UpdatePricingPlanOutputTypeDef",
+    "AssociateAccountsOutputTypeDef",
+    "AssociatePricingRulesOutputTypeDef",
+    "CreateBillingGroupOutputTypeDef",
+    "CreateCustomLineItemOutputTypeDef",
+    "CreatePricingPlanOutputTypeDef",
+    "CreatePricingRuleOutputTypeDef",
+    "DeleteBillingGroupOutputTypeDef",
+    "DeleteCustomLineItemOutputTypeDef",
+    "DeletePricingPlanOutputTypeDef",
+    "DeletePricingRuleOutputTypeDef",
+    "DisassociateAccountsOutputTypeDef",
+    "DisassociatePricingRulesOutputTypeDef",
     "ListAccountAssociationsOutputTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateBillingGroupOutputTypeDef",
+    "UpdatePricingPlanOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
     "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
     "UpdateBillingGroupInputRequestTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
-    "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     "ListAccountAssociationsInputRequestTypeDef",
+    "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     "ListBillingGroupCostReportsInputRequestTypeDef",
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsInputRequestTypeDef",
     "ListCustomLineItemChargeDetailsTypeDef",
     "ListCustomLineItemVersionsFilterTypeDef",
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
@@ -164,38 +164,33 @@
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-AssociateAccountsOutputTypeDef = TypedDict(
-    "AssociateAccountsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociatePricingRulesInputRequestTypeDef = TypedDict(
     "AssociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
-AssociatePricingRulesOutputTypeDef = TypedDict(
-    "AssociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateResourceErrorTypeDef = TypedDict(
     "AssociateResourceErrorTypeDef",
     {
         "Message": str,
         "Reason": AssociateResourceErrorReasonType,
     },
     total=False,
@@ -237,30 +232,14 @@
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
-CreateBillingGroupOutputTypeDef = TypedDict(
-    "CreateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomLineItemOutputTypeDef = TypedDict(
-    "CreateCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -282,30 +261,14 @@
 )
 
 class CreatePricingPlanInputRequestTypeDef(
     _RequiredCreatePricingPlanInputRequestTypeDef, _OptionalCreatePricingPlanInputRequestTypeDef
 ):
     pass
 
-CreatePricingPlanOutputTypeDef = TypedDict(
-    "CreatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePricingRuleOutputTypeDef = TypedDict(
-    "CreatePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "CustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -332,92 +295,44 @@
 DeleteBillingGroupInputRequestTypeDef = TypedDict(
     "DeleteBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteBillingGroupOutputTypeDef = TypedDict(
-    "DeleteBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteCustomLineItemOutputTypeDef = TypedDict(
-    "DeleteCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePricingPlanInputRequestTypeDef = TypedDict(
     "DeletePricingPlanInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeletePricingPlanOutputTypeDef = TypedDict(
-    "DeletePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePricingRuleInputRequestTypeDef = TypedDict(
     "DeletePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeletePricingRuleOutputTypeDef = TypedDict(
-    "DeletePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateAccountsInputRequestTypeDef = TypedDict(
     "DisassociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-DisassociateAccountsOutputTypeDef = TypedDict(
-    "DisassociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociatePricingRulesInputRequestTypeDef = TypedDict(
     "DisassociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
-DisassociatePricingRulesOutputTypeDef = TypedDict(
-    "DisassociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FreeTierConfigTypeDef = TypedDict(
     "FreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -427,14 +342,24 @@
         "Association": str,
         "AccountId": str,
         "AccountIds": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ListBillingGroupCostReportsFilterTypeDef = TypedDict(
     "ListBillingGroupCostReportsFilterTypeDef",
     {
         "BillingGroupArns": Sequence[str],
     },
     total=False,
 )
@@ -478,35 +403,14 @@
         "Names": Sequence[str],
         "BillingGroups": Sequence[str],
         "Arns": Sequence[str],
     },
     total=False,
 )
 
-_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "PricingRuleArn": str,
-    },
-)
-_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
-    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-):
-    pass
-
 _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
     {
         "PricingRuleArn": str,
     },
 )
 _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
@@ -521,25 +425,14 @@
 
 class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(
     _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
     _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
 ):
     pass
 
-ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingRuleArn": str,
-        "PricingPlanArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPricingPlansFilterTypeDef = TypedDict(
     "ListPricingPlansFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -553,35 +446,14 @@
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
     },
     total=False,
 )
 
-_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "PricingPlanArn": str,
-    },
-)
-_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
-    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-):
-    pass
-
 _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
     "_RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
@@ -596,25 +468,14 @@
 
 class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(
     _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
     _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
 ):
     pass
 
-ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingPlanArn": str,
-        "PricingRuleArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPricingRulesFilterTypeDef = TypedDict(
     "ListPricingRulesFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -640,43 +501,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -685,30 +517,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateBillingGroupOutputTypeDef = TypedDict(
-    "UpdateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "PrimaryAccountId": str,
-        "PricingPlanArn": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "Status": BillingGroupStatusType,
-        "StatusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -742,32 +558,174 @@
 )
 
 class UpdatePricingPlanInputRequestTypeDef(
     _RequiredUpdatePricingPlanInputRequestTypeDef, _OptionalUpdatePricingPlanInputRequestTypeDef
 ):
     pass
 
-UpdatePricingPlanOutputTypeDef = TypedDict(
-    "UpdatePricingPlanOutputTypeDef",
+AssociateAccountsOutputTypeDef = TypedDict(
+    "AssociateAccountsOutputTypeDef",
     {
         "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociatePricingRulesOutputTypeDef = TypedDict(
+    "AssociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBillingGroupOutputTypeDef = TypedDict(
+    "CreateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomLineItemOutputTypeDef = TypedDict(
+    "CreateCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePricingPlanOutputTypeDef = TypedDict(
+    "CreatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePricingRuleOutputTypeDef = TypedDict(
+    "CreatePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBillingGroupOutputTypeDef = TypedDict(
+    "DeleteBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCustomLineItemOutputTypeDef = TypedDict(
+    "DeleteCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePricingPlanOutputTypeDef = TypedDict(
+    "DeletePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePricingRuleOutputTypeDef = TypedDict(
+    "DeletePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateAccountsOutputTypeDef = TypedDict(
+    "DisassociateAccountsOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociatePricingRulesOutputTypeDef = TypedDict(
+    "DisassociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountAssociationsOutputTypeDef = TypedDict(
     "ListAccountAssociationsOutputTypeDef",
     {
         "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingRuleArn": str,
+        "PricingPlanArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingPlanArn": str,
+        "PricingRuleArns": List[str],
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
+    },
+)
+
+UpdateBillingGroupOutputTypeDef = TypedDict(
+    "UpdateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "PrimaryAccountId": str,
+        "PricingPlanArn": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "Status": BillingGroupStatusType,
+        "StatusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePricingPlanOutputTypeDef = TypedDict(
+    "UpdatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResourceResponseElementTypeDef = TypedDict(
     "AssociateResourceResponseElementTypeDef",
     {
         "Arn": str,
@@ -848,15 +806,15 @@
     pass
 
 ListBillingGroupCostReportsOutputTypeDef = TypedDict(
     "ListBillingGroupCostReportsOutputTypeDef",
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BillingGroupListElementTypeDef = TypedDict(
     "BillingGroupListElementTypeDef",
     {
         "Name": str,
@@ -949,40 +907,82 @@
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "FreeTier": FreeTierConfigTypeDef,
     },
 )
 
+ListAccountAssociationsInputRequestTypeDef = TypedDict(
+    "ListAccountAssociationsInputRequestTypeDef",
+    {
+        "BillingPeriod": str,
+        "Filters": ListAccountAssociationsFilterTypeDef,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef = TypedDict(
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListAccountAssociationsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAccountAssociationsInputRequestTypeDef = TypedDict(
-    "ListAccountAssociationsInputRequestTypeDef",
+_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "PricingRuleArn": str,
+    },
+)
+_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     {
         "BillingPeriod": str,
-        "Filters": ListAccountAssociationsFilterTypeDef,
-        "NextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
+    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+):
+    pass
+
+_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "PricingPlanArn": str,
+    },
+)
+_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
+    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+):
+    pass
+
 ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupCostReportsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListBillingGroupCostReportsInputRequestTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputRequestTypeDef",
     {
@@ -995,15 +995,15 @@
 )
 
 ListBillingGroupsInputListBillingGroupsPaginateTypeDef = TypedDict(
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListBillingGroupsInputRequestTypeDef = TypedDict(
     "ListBillingGroupsInputRequestTypeDef",
     {
@@ -1044,15 +1044,15 @@
 )
 
 ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef = TypedDict(
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListCustomLineItemsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCustomLineItemsInputRequestTypeDef = TypedDict(
     "ListCustomLineItemsInputRequestTypeDef",
     {
@@ -1065,15 +1065,15 @@
 )
 
 ListPricingPlansInputListPricingPlansPaginateTypeDef = TypedDict(
     "ListPricingPlansInputListPricingPlansPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingPlansFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPricingPlansInputRequestTypeDef = TypedDict(
     "ListPricingPlansInputRequestTypeDef",
     {
@@ -1087,24 +1087,24 @@
 
 ListPricingPlansOutputTypeDef = TypedDict(
     "ListPricingPlansOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingPlans": List[PricingPlanListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPricingRulesInputListPricingRulesPaginateTypeDef = TypedDict(
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingRulesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPricingRulesInputRequestTypeDef = TypedDict(
     "ListPricingRulesInputRequestTypeDef",
     {
@@ -1123,15 +1123,15 @@
     },
 )
 _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef = TypedDict(
     "_OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListResourcesAssociatedToCustomLineItemFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef(
     _RequiredListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
     _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
@@ -1163,15 +1163,15 @@
 
 ListResourcesAssociatedToCustomLineItemOutputTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomLineItemChargeDetailsTypeDef = TypedDict(
     "UpdateCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": UpdateCustomLineItemFlatChargeDetailsTypeDef,
@@ -1188,33 +1188,33 @@
 )
 
 BatchAssociateResourcesToCustomLineItemOutputTypeDef = TypedDict(
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     {
         "SuccessfullyAssociatedResources": List[AssociateResourceResponseElementTypeDef],
         "FailedAssociatedResources": List[AssociateResourceResponseElementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateResourcesFromCustomLineItemOutputTypeDef = TypedDict(
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     {
         "SuccessfullyDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
         "FailedDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBillingGroupsOutputTypeDef = TypedDict(
     "ListBillingGroupsOutputTypeDef",
     {
         "BillingGroups": List[BillingGroupListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreatePricingRuleInputRequestTypeDef",
     {
         "Name": str,
@@ -1332,29 +1332,29 @@
         "Arn": str,
         "BillingGroupArn": str,
         "Name": str,
         "Description": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
         "LastModifiedTime": int,
         "AssociationSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Filters": ListCustomLineItemVersionsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef(
     _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
     _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
@@ -1441,38 +1441,38 @@
         "Service": str,
         "AssociatedPricingPlanCount": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": UpdateTieringInputTypeDef,
         "UsageType": str,
         "Operation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPricingRulesOutputTypeDef = TypedDict(
     "ListPricingRulesOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingRules": List[PricingRuleListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomLineItemsOutputTypeDef = TypedDict(
     "ListCustomLineItemsOutputTypeDef",
     {
         "CustomLineItems": List[CustomLineItemListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomLineItemVersionsOutputTypeDef = TypedDict(
     "ListCustomLineItemVersionsOutputTypeDef",
     {
         "CustomLineItemVersions": List[CustomLineItemVersionListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/PKG-INFO` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-billingconductor
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.BillingConductor 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore billingconductor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore billingconductor type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-billingconductor"></a>
 
 # types-aiobotocore-billingconductor
 
 [![PyPI - types-aiobotocore-billingconductor](https://img.shields.io/pypi/v/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-billingconductor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-billingconductor?color=blue)](https://pypistats.org/packages/types-aiobotocore-billingconductor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-billingconductor)](https://pepy.tech/project/types-aiobotocore-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BillingConductor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [types-aiobotocore-billingconductor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_billingconductor/).
 
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
@@ -360,98 +359,98 @@
 )
 
 
 def check_value(value: AssociateResourceErrorReasonType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_billingconductor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
-    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
-    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
-    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
-    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateBillingGroupOutputTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    UpdatePricingPlanOutputTypeDef,
+    AssociateAccountsOutputTypeDef,
+    AssociatePricingRulesOutputTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
+    DeletePricingPlanOutputTypeDef,
+    DeletePricingRuleOutputTypeDef,
+    DisassociateAccountsOutputTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     ListAccountAssociationsOutputTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateBillingGroupOutputTypeDef,
+    UpdatePricingPlanOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     UpdateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
     ListAccountAssociationsInputRequestTypeDef,
+    ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
@@ -482,15 +481,15 @@
     UpdatePricingRuleOutputTypeDef,
     ListPricingRulesOutputTypeDef,
     ListCustomLineItemsOutputTypeDef,
     ListCustomLineItemVersionsOutputTypeDef,
 )
 
 
-def get_structure() -> AccountAssociationsListElementTypeDef:
+def get_value() -> AccountAssociationsListElementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-billingconductor-2.5.2/types_aiobotocore_billingconductor.egg-info/SOURCES.txt` & `types-aiobotocore-billingconductor-2.5.2.post1/types_aiobotocore_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


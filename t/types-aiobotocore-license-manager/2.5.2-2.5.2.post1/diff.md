# Comparing `tmp/types-aiobotocore-license-manager-2.5.2.tar.gz` & `tmp/types-aiobotocore-license-manager-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-license-manager-2.5.2.tar` & `types-aiobotocore-license-manager-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.718434 types-aiobotocore-license-manager-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20631 2023-07-08 01:43:53.714434 types-aiobotocore-license-manager-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19035 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.718434 types-aiobotocore-license-manager-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.714434 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43066 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43002 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55171 2023-07-08 01:34:03.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55100 2023-07-08 01:34:03.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:02.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.714434 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20631 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:53.000000 types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.893541 types-aiobotocore-license-manager-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-08-02 14:52:33.889541 types-aiobotocore-license-manager-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19197 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.893541 types-aiobotocore-license-manager-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.889541 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43096 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43032 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56419 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56347 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.889541 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-2.5.2/LICENSE` & `types-aiobotocore-license-manager-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2/PKG-INFO` & `types-aiobotocore-license-manager-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore license-manager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore license-manager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-license-manager"></a>
 
 # types-aiobotocore-license-manager
 
 [![PyPI - types-aiobotocore-license-manager](https://img.shields.io/pypi/v/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-license-manager?color=blue)](https://pypistats.org/packages/types-aiobotocore-license-manager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LicenseManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [types-aiobotocore-license-manager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/).
 
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
@@ -348,93 +347,93 @@
 )
 
 
 def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_license_manager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
+    ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
     ConsumedLicenseSummaryTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantResponseTypeDef,
     OptionsTypeDef,
-    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
     DeleteGrantRequestRequestTypeDef,
-    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
-    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
-    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
     OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
     LicenseSpecificationTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
-    PaginatorConfigTypeDef,
+    ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
-    RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
     S3LocationTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AcceptGrantResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    CreateGrantVersionResponseTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
+    CreateTokenResponseTypeDef,
+    DeleteGrantResponseTypeDef,
+    DeleteLicenseResponseTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
+    GetAccessTokenResponseTypeDef,
+    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
@@ -444,65 +443,70 @@
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
     GetLicenseConversionTaskResponseTypeDef,
     LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
+    ReportContextUnionTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
-    UpdateLicenseConfigurationRequestRequestTypeDef,
+    ProductInformationUnionTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
     ListLicensesResponseTypeDef,
     ListLicenseConfigurationsResponseTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
+    UpdateLicenseConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptGrantRequestRequestTypeDef:
+def get_value() -> AcceptGrantRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-license-manager-2.5.2/README.md` & `types-aiobotocore-license-manager-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-license-manager"></a>
 
 # types-aiobotocore-license-manager
 
 [![PyPI - types-aiobotocore-license-manager](https://img.shields.io/pypi/v/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-license-manager?color=blue)](https://pypistats.org/packages/types-aiobotocore-license-manager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LicenseManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [types-aiobotocore-license-manager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/).
 
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
@@ -315,93 +315,93 @@
 )
 
 
 def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_license_manager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
+    ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
     ConsumedLicenseSummaryTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantResponseTypeDef,
     OptionsTypeDef,
-    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
     DeleteGrantRequestRequestTypeDef,
-    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
-    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
-    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
     OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
     LicenseSpecificationTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
-    PaginatorConfigTypeDef,
+    ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
-    RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
     S3LocationTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AcceptGrantResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    CreateGrantVersionResponseTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
+    CreateTokenResponseTypeDef,
+    DeleteGrantResponseTypeDef,
+    DeleteLicenseResponseTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
+    GetAccessTokenResponseTypeDef,
+    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
@@ -411,65 +411,70 @@
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
     GetLicenseConversionTaskResponseTypeDef,
     LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
+    ReportContextUnionTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
-    UpdateLicenseConfigurationRequestRequestTypeDef,
+    ProductInformationUnionTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
     ListLicensesResponseTypeDef,
     ListLicenseConfigurationsResponseTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
+    UpdateLicenseConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptGrantRequestRequestTypeDef:
+def get_value() -> AcceptGrantRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-license-manager-2.5.2/setup.py` & `types-aiobotocore-license-manager-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with"
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
-    keywords="aiobotocore license-manager type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore license-manager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_license_manager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/"
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/__init__.py` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/__init__.pyi` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/__main__.py` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LicenseManager 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.LicenseManager 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/client.py` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
-    ProductInformationTypeDef,
+    ProductInformationUnionTypeDef,
     RejectGrantResponseTypeDef,
-    ReportContextTypeDef,
+    ReportContextUnionTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -284,15 +284,15 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_configuration)
         """
@@ -312,15 +312,15 @@
         """
 
     async def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
@@ -757,15 +757,15 @@
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_configuration)
@@ -773,15 +773,15 @@
 
     async def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/client.pyi` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
-    ProductInformationTypeDef,
+    ProductInformationUnionTypeDef,
     RejectGrantResponseTypeDef,
-    ReportContextTypeDef,
+    ReportContextUnionTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -270,15 +270,15 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_configuration)
         """
@@ -296,15 +296,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_conversion_task_for_resource)
         """
     async def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
@@ -703,30 +703,30 @@
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_configuration)
         """
     async def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextTypeDef,
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/literals.py` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/literals.pyi` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/paginator.py` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 class ListAssociationsForLicenseConfigurationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
     """
 
     def paginate(
-        self, *, LicenseConfigurationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LicenseConfigurationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
         """
 
 
@@ -85,30 +85,30 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLicenseConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 
 class ListLicenseSpecificationsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
         """
 
 
@@ -118,15 +118,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 
@@ -137,13 +137,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/paginator.pyi` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 class ListAssociationsForLicenseConfigurationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
     """
 
     def paginate(
-        self, *, LicenseConfigurationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LicenseConfigurationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociationsForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListAssociationsForLicenseConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listassociationsforlicenseconfigurationpaginator)
         """
 
 class ListLicenseConfigurationsPaginator(AioPaginator):
@@ -81,29 +81,29 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLicenseConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicenseconfigurationspaginator)
         """
 
 class ListLicenseSpecificationsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLicenseSpecificationsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListLicenseSpecificationsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listlicensespecificationsforresourcepaginator)
         """
 
 class ListResourceInventoryPaginator(AioPaginator):
@@ -112,15 +112,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceInventoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListResourceInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listresourceinventorypaginator)
         """
 
 class ListUsageForLicenseConfigurationPaginator(AioPaginator):
@@ -130,13 +130,13 @@
     """
 
     def paginate(
         self,
         *,
         LicenseConfigurationArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsageForLicenseConfigurationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Paginator.ListUsageForLicenseConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/paginators/#listusageforlicenseconfigurationpaginator)
         """
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/type_defs.py` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
-    data: AcceptGrantRequestRequestTypeDef = {...}
+    data: AcceptGrantRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
@@ -40,86 +40,85 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
-    "AcceptGrantResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
     "ConsumedLicenseSummaryTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "CreateGrantResponseTypeDef",
     "OptionsTypeDef",
-    "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
-    "CreateLicenseConfigurationResponseTypeDef",
     "LicenseConversionContextTypeDef",
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     "ReportContextTypeDef",
     "ReportFrequencyTypeDef",
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
-    "CreateLicenseResponseTypeDef",
-    "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
     "DeleteGrantRequestRequestTypeDef",
-    "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
-    "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
-    "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
-    "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
     "OrganizationConfigurationTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
     "LicenseSpecificationTypeDef",
-    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
-    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
-    "RejectGrantResponseTypeDef",
+    "ReportContextOutputTypeDef",
     "S3LocationTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AcceptGrantResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "CreateGrantVersionResponseTypeDef",
+    "CreateLicenseConfigurationResponseTypeDef",
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    "CreateLicenseResponseTypeDef",
+    "CreateLicenseVersionResponseTypeDef",
+    "CreateTokenResponseTypeDef",
+    "DeleteGrantResponseTypeDef",
+    "DeleteLicenseResponseTypeDef",
+    "ExtendLicenseConsumptionResponseTypeDef",
+    "GetAccessTokenResponseTypeDef",
+    "RejectGrantResponseTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
     "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
     "ConsumptionConfigurationTypeDef",
     "CreateGrantVersionRequestRequestTypeDef",
@@ -129,77 +128,83 @@
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
     "GetLicenseConversionTaskResponseTypeDef",
     "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
     "ListLicenseManagerReportGeneratorsRequestRequestTypeDef",
     "ListLicensesRequestRequestTypeDef",
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
-    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
+    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
+    "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
+    "ReportContextUnionTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
-    "UpdateLicenseConfigurationRequestRequestTypeDef",
+    "ProductInformationUnionTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
     "ListLicensesResponseTypeDef",
     "ListLicenseConfigurationsResponseTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
+    "UpdateLicenseConfigurationRequestRequestTypeDef",
 )
 
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-AcceptGrantResponseTypeDef = TypedDict(
-    "AcceptGrantResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AutomatedDiscoveryInformationTypeDef = TypedDict(
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
@@ -225,21 +230,19 @@
     "_OptionalCheckInLicenseRequestRequestTypeDef",
     {
         "Beneficiary": str,
     },
     total=False,
 )
 
-
 class CheckInLicenseRequestRequestTypeDef(
     _RequiredCheckInLicenseRequestRequestTypeDef, _OptionalCheckInLicenseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredEntitlementDataTypeDef = TypedDict(
     "_RequiredEntitlementDataTypeDef",
     {
         "Name": str,
         "Unit": EntitlementDataUnitType,
     },
 )
@@ -247,19 +250,17 @@
     "_OptionalEntitlementDataTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class EntitlementDataTypeDef(_RequiredEntitlementDataTypeDef, _OptionalEntitlementDataTypeDef):
     pass
 
-
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -289,75 +290,39 @@
         "LicenseArn": str,
         "Principals": Sequence[str],
         "HomeRegion": str,
         "AllowedOperations": Sequence[AllowedOperationType],
     },
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OptionsTypeDef = TypedDict(
     "OptionsTypeDef",
     {
         "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
     },
     total=False,
 )
 
-CreateGrantVersionResponseTypeDef = TypedDict(
-    "CreateGrantVersionResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
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
     total=False,
 )
 
-CreateLicenseConfigurationResponseTypeDef = TypedDict(
-    "CreateLicenseConfigurationResponseTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LicenseConversionContextTypeDef = TypedDict(
     "LicenseConversionContextTypeDef",
     {
         "UsageOperation": str,
     },
     total=False,
 )
 
-CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportContextTypeDef = TypedDict(
     "ReportContextTypeDef",
     {
         "licenseConfigurationArns": Sequence[str],
     },
 )
 
@@ -366,41 +331,31 @@
     {
         "value": int,
         "period": ReportFrequencyTypeType,
     },
     total=False,
 )
 
-CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    {
-        "LicenseManagerReportGeneratorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDatetimeRangeTypeDef = TypedDict(
     "_RequiredDatetimeRangeTypeDef",
     {
         "Begin": str,
     },
 )
 _OptionalDatetimeRangeTypeDef = TypedDict(
     "_OptionalDatetimeRangeTypeDef",
     {
         "End": str,
     },
     total=False,
 )
 
-
 class DatetimeRangeTypeDef(_RequiredDatetimeRangeTypeDef, _OptionalDatetimeRangeTypeDef):
     pass
 
-
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "Unit": EntitlementUnitType,
     },
 )
@@ -411,58 +366,34 @@
         "MaxCount": int,
         "Overage": bool,
         "AllowCheckIn": bool,
     },
     total=False,
 )
 
-
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
-
 _RequiredIssuerTypeDef = TypedDict(
     "_RequiredIssuerTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalIssuerTypeDef = TypedDict(
     "_OptionalIssuerTypeDef",
     {
         "SignKey": str,
     },
     total=False,
 )
 
-
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
-
-CreateLicenseResponseTypeDef = TypedDict(
-    "CreateLicenseResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Status": LicenseStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLicenseVersionResponseTypeDef = TypedDict(
-    "CreateLicenseVersionResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Version": str,
-        "Status": LicenseStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
 )
@@ -472,31 +403,19 @@
         "RoleArns": Sequence[str],
         "ExpirationInDays": int,
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
-    {
-        "TokenId": str,
-        "TokenType": Literal["REFRESH_TOKEN"],
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -504,31 +423,19 @@
     "_OptionalDeleteGrantRequestRequestTypeDef",
     {
         "StatusReason": str,
     },
     total=False,
 )
 
-
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
-
-DeleteGrantResponseTypeDef = TypedDict(
-    "DeleteGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -543,23 +450,14 @@
     "DeleteLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "SourceVersion": str,
     },
 )
 
-DeleteLicenseResponseTypeDef = TypedDict(
-    "DeleteLicenseResponseTypeDef",
-    {
-        "Status": LicenseDeletionStatusType,
-        "DeletionDate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
@@ -575,50 +473,37 @@
     "_OptionalEntitlementUsageTypeDef",
     {
         "MaxCount": str,
     },
     total=False,
 )
 
-
 class EntitlementUsageTypeDef(_RequiredEntitlementUsageTypeDef, _OptionalEntitlementUsageTypeDef):
     pass
 
-
 _RequiredExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_RequiredExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "LicenseConsumptionToken": str,
     },
 )
 _OptionalExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_OptionalExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
-
-ExtendLicenseConsumptionResponseTypeDef = TypedDict(
-    "ExtendLicenseConsumptionResponseTypeDef",
-    {
-        "LicenseConsumptionToken": str,
-        "Expiration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -634,50 +519,38 @@
     "_OptionalGetAccessTokenRequestRequestTypeDef",
     {
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
-
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
-
-GetAccessTokenResponseTypeDef = TypedDict(
-    "GetAccessTokenResponseTypeDef",
-    {
-        "AccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 _OptionalGetGrantRequestRequestTypeDef = TypedDict(
     "_OptionalGetGrantRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetGrantRequestRequestTypeDef(
     _RequiredGetGrantRequestRequestTypeDef, _OptionalGetGrantRequestRequestTypeDef
 ):
     pass
 
-
 GetLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "GetLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -714,21 +587,19 @@
     "_OptionalGetLicenseRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetLicenseRequestRequestTypeDef(
     _RequiredGetLicenseRequestRequestTypeDef, _OptionalGetLicenseRequestRequestTypeDef
 ):
     pass
 
-
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
@@ -770,19 +641,17 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 LicenseConfigurationAssociationTypeDef = TypedDict(
     "LicenseConfigurationAssociationTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
@@ -814,43 +683,29 @@
     "_OptionalLicenseSpecificationTypeDef",
     {
         "AmiAssociationScope": str,
     },
     total=False,
 )
 
-
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
-
-_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
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
-class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
-    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -858,22 +713,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationsForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
@@ -881,44 +734,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
-    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
@@ -926,22 +755,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLicenseVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseVersionsRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 _OptionalListLicenseVersionsRequestRequestTypeDef = TypedDict(
@@ -949,22 +776,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLicenseVersionsRequestRequestTypeDef(
     _RequiredListLicenseVersionsRequestRequestTypeDef,
     _OptionalListLicenseVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceInventoryTypeDef = TypedDict(
     "ResourceInventoryTypeDef",
     {
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "ResourceArn": str,
         "Platform": str,
@@ -991,24 +816,34 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredProductInformationFilterOutputTypeDef = TypedDict(
+    "_RequiredProductInformationFilterOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProductInformationFilterName": str,
+        "ProductInformationFilterComparator": str,
+    },
+)
+_OptionalProductInformationFilterOutputTypeDef = TypedDict(
+    "_OptionalProductInformationFilterOutputTypeDef",
+    {
+        "ProductInformationFilterValue": List[str],
     },
     total=False,
 )
 
+class ProductInformationFilterOutputTypeDef(
+    _RequiredProductInformationFilterOutputTypeDef, _OptionalProductInformationFilterOutputTypeDef
+):
+    pass
+
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -1016,66 +851,180 @@
     "_OptionalProductInformationFilterTypeDef",
     {
         "ProductInformationFilterValue": Sequence[str],
     },
     total=False,
 )
 
-
 class ProductInformationFilterTypeDef(
     _RequiredProductInformationFilterTypeDef, _OptionalProductInformationFilterTypeDef
 ):
     pass
 
-
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-RejectGrantResponseTypeDef = TypedDict(
-    "RejectGrantResponseTypeDef",
+ReportContextOutputTypeDef = TypedDict(
+    "ReportContextOutputTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "licenseConfigurationArns": List[str],
     },
 )
 
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AcceptGrantResponseTypeDef = TypedDict(
+    "AcceptGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantVersionResponseTypeDef = TypedDict(
+    "CreateGrantVersionResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseConfigurationResponseTypeDef = TypedDict(
+    "CreateLicenseConfigurationResponseTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    {
+        "LicenseManagerReportGeneratorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseResponseTypeDef = TypedDict(
+    "CreateLicenseResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Status": LicenseStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseVersionResponseTypeDef = TypedDict(
+    "CreateLicenseVersionResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Version": str,
+        "Status": LicenseStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
+    {
+        "TokenId": str,
+        "TokenType": Literal["REFRESH_TOKEN"],
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGrantResponseTypeDef = TypedDict(
+    "DeleteGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLicenseResponseTypeDef = TypedDict(
+    "DeleteLicenseResponseTypeDef",
+    {
+        "Status": LicenseDeletionStatusType,
+        "DeletionDate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExtendLicenseConsumptionResponseTypeDef = TypedDict(
+    "ExtendLicenseConsumptionResponseTypeDef",
+    {
+        "LicenseConsumptionToken": str,
+        "Expiration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessTokenResponseTypeDef = TypedDict(
+    "GetAccessTokenResponseTypeDef",
+    {
+        "AccessToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectGrantResponseTypeDef = TypedDict(
+    "RejectGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCheckoutLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutLicenseRequestRequestTypeDef",
     {
         "ProductSKU": str,
         "CheckoutType": CheckoutTypeType,
         "KeyFingerprint": str,
         "Entitlements": Sequence[EntitlementDataTypeDef],
@@ -1087,33 +1036,31 @@
     {
         "Beneficiary": str,
         "NodeId": str,
     },
     total=False,
 )
 
-
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
-
 CheckoutLicenseResponseTypeDef = TypedDict(
     "CheckoutLicenseResponseTypeDef",
     {
         "CheckoutType": CheckoutTypeType,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "SignedToken": str,
         "NodeId": str,
         "IssuedAt": str,
         "Expiration": str,
         "LicenseArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
@@ -1127,34 +1074,32 @@
     {
         "NodeId": str,
         "CheckoutMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
-
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
-
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
         "CheckoutMetadata": List[MetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
@@ -1195,22 +1140,20 @@
         "StatusReason": str,
         "SourceVersion": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
-
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGrantTypeDef = TypedDict(
     "_RequiredGrantTypeDef",
     {
         "GrantArn": str,
         "GrantName": str,
         "ParentArn": str,
         "LicenseArn": str,
@@ -1226,24 +1169,22 @@
     {
         "StatusReason": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
-
 class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1268,15 +1209,15 @@
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
         "StatusMessage": str,
         "Status": LicenseConversionTaskStatusType,
         "StartTime": datetime,
         "LicenseConversionTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConversionTaskTypeDef = TypedDict(
     "LicenseConversionTaskTypeDef",
     {
         "LicenseConversionTaskId": str,
@@ -1307,22 +1248,20 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
@@ -1334,22 +1273,20 @@
     "_OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
-
 LicenseUsageTypeDef = TypedDict(
     "LicenseUsageTypeDef",
     {
         "EntitlementUsages": List[EntitlementUsageTypeDef],
     },
     total=False,
 )
@@ -1361,24 +1298,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    {
-        "LicenseConfigurationArns": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLicenseConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1429,22 +1356,20 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListReceivedGrantsForOrganizationRequestRequestTypeDef(
     _RequiredListReceivedGrantsForOrganizationRequestRequestTypeDef,
     _OptionalListReceivedGrantsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 ListReceivedGrantsRequestRequestTypeDef = TypedDict(
     "ListReceivedGrantsRequestRequestTypeDef",
     {
         "GrantArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
@@ -1480,37 +1405,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -1519,54 +1421,43 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingsRequestRequestTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
     },
     total=False,
 )
 
-ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
-    {
-        "Filters": Sequence[InventoryFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceInventoryRequestRequestTypeDef = TypedDict(
     "ListResourceInventoryRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
@@ -1574,33 +1465,33 @@
 )
 
 ListAssociationsForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationAssociations": List[LicenseConfigurationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListUsageForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationUsageList": List[LicenseConfigurationUsageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
         "LicenseSpecifications": List[LicenseSpecificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1611,54 +1502,141 @@
     {
         "AddLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
         "RemoveLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
+    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    {
+        "LicenseConfigurationArns": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
+    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+):
+    pass
+
+ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    {
+        "Filters": Sequence[InventoryFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+):
+    pass
 
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTokensResponseTypeDef = TypedDict(
     "ListTokensResponseTypeDef",
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProductInformationOutputTypeDef = TypedDict(
+    "ProductInformationOutputTypeDef",
+    {
+        "ResourceType": str,
+        "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
     },
 )
 
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
+ReportContextUnionTypeDef = Union[ReportContextTypeDef, ReportContextOutputTypeDef]
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
-        "ReportContext": ReportContextTypeDef,
+        "ReportContext": ReportContextOutputTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
@@ -1670,15 +1648,15 @@
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
@@ -1697,21 +1675,19 @@
     "_OptionalCreateLicenseRequestRequestTypeDef",
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseRequestRequestTypeDef(
     _RequiredCreateLicenseRequestRequestTypeDef, _OptionalCreateLicenseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLicenseVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseVersionRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "Issuer": IssuerTypeDef,
@@ -1728,22 +1704,20 @@
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
         "SourceVersion": str,
     },
     total=False,
 )
 
-
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GrantedLicenseTypeDef = TypedDict(
     "GrantedLicenseTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
@@ -1783,91 +1757,62 @@
     total=False,
 )
 
 GetGrantResponseTypeDef = TypedDict(
     "GetGrantResponseTypeDef",
     {
         "Grant": GrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributedGrantsResponseTypeDef = TypedDict(
     "ListDistributedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsResponseTypeDef = TypedDict(
     "ListReceivedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseConversionTasksResponseTypeDef = TypedDict(
     "ListLicenseConversionTasksResponseTypeDef",
     {
         "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseUsageResponseTypeDef = TypedDict(
     "GetLicenseUsageResponseTypeDef",
     {
         "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1877,18 +1822,18 @@
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "Tags": List[TagTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -1901,111 +1846,137 @@
         "LicenseCountHardLimit": bool,
         "DisassociateWhenNotFound": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
-        "LicenseRules": Sequence[str],
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "Name": str,
-        "Description": str,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
-        "DisassociateWhenNotFound": bool,
-    },
-    total=False,
-)
-
-
-class UpdateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
+ProductInformationUnionTypeDef = Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseManagerReportGeneratorsResponseTypeDef = TypedDict(
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     {
         "ReportGenerators": List[ReportGeneratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesResponseTypeDef = TypedDict(
     "ListReceivedLicensesResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseResponseTypeDef = TypedDict(
     "GetLicenseResponseTypeDef",
     {
         "License": LicenseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseVersionsResponseTypeDef = TypedDict(
     "ListLicenseVersionsResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicensesResponseTypeDef = TypedDict(
     "ListLicensesResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseConfigurationsResponseTypeDef = TypedDict(
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationArn": str,
     },
 )
+_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
+        "LicenseRules": Sequence[str],
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "Name": str,
+        "Description": str,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+        "DisassociateWhenNotFound": bool,
+    },
+    total=False,
+)
+
+class UpdateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager/type_defs.pyi` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
-    data: AcceptGrantRequestRequestTypeDef = {...}
+    data: AcceptGrantRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
@@ -40,85 +40,86 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
-    "AcceptGrantResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
     "ConsumedLicenseSummaryTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "CreateGrantResponseTypeDef",
     "OptionsTypeDef",
-    "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
-    "CreateLicenseConfigurationResponseTypeDef",
     "LicenseConversionContextTypeDef",
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
     "ReportContextTypeDef",
     "ReportFrequencyTypeDef",
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
-    "CreateLicenseResponseTypeDef",
-    "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
     "DeleteGrantRequestRequestTypeDef",
-    "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
-    "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
-    "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
-    "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
     "OrganizationConfigurationTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
     "LicenseSpecificationTypeDef",
-    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
-    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
-    "PaginatorConfigTypeDef",
+    "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
-    "RejectGrantResponseTypeDef",
+    "ReportContextOutputTypeDef",
     "S3LocationTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AcceptGrantResponseTypeDef",
+    "CreateGrantResponseTypeDef",
+    "CreateGrantVersionResponseTypeDef",
+    "CreateLicenseConfigurationResponseTypeDef",
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    "CreateLicenseResponseTypeDef",
+    "CreateLicenseVersionResponseTypeDef",
+    "CreateTokenResponseTypeDef",
+    "DeleteGrantResponseTypeDef",
+    "DeleteLicenseResponseTypeDef",
+    "ExtendLicenseConsumptionResponseTypeDef",
+    "GetAccessTokenResponseTypeDef",
+    "RejectGrantResponseTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
     "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseRequestRequestTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
     "ConsumptionConfigurationTypeDef",
     "CreateGrantVersionRequestRequestTypeDef",
@@ -128,77 +129,83 @@
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
     "GetLicenseConversionTaskResponseTypeDef",
     "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
     "ListLicenseManagerReportGeneratorsRequestRequestTypeDef",
     "ListLicensesRequestRequestTypeDef",
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
-    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
+    "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
+    "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
+    "ReportContextUnionTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
-    "UpdateLicenseConfigurationRequestRequestTypeDef",
+    "ProductInformationUnionTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
     "ListLicensesResponseTypeDef",
     "ListLicenseConfigurationsResponseTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
+    "UpdateLicenseConfigurationRequestRequestTypeDef",
 )
 
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-AcceptGrantResponseTypeDef = TypedDict(
-    "AcceptGrantResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AutomatedDiscoveryInformationTypeDef = TypedDict(
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
@@ -224,19 +231,21 @@
     "_OptionalCheckInLicenseRequestRequestTypeDef",
     {
         "Beneficiary": str,
     },
     total=False,
 )
 
+
 class CheckInLicenseRequestRequestTypeDef(
     _RequiredCheckInLicenseRequestRequestTypeDef, _OptionalCheckInLicenseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredEntitlementDataTypeDef = TypedDict(
     "_RequiredEntitlementDataTypeDef",
     {
         "Name": str,
         "Unit": EntitlementDataUnitType,
     },
 )
@@ -244,17 +253,19 @@
     "_OptionalEntitlementDataTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class EntitlementDataTypeDef(_RequiredEntitlementDataTypeDef, _OptionalEntitlementDataTypeDef):
     pass
 
+
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -284,75 +295,39 @@
         "LicenseArn": str,
         "Principals": Sequence[str],
         "HomeRegion": str,
         "AllowedOperations": Sequence[AllowedOperationType],
     },
 )
 
-CreateGrantResponseTypeDef = TypedDict(
-    "CreateGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OptionsTypeDef = TypedDict(
     "OptionsTypeDef",
     {
         "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
     },
     total=False,
 )
 
-CreateGrantVersionResponseTypeDef = TypedDict(
-    "CreateGrantVersionResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
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
     total=False,
 )
 
-CreateLicenseConfigurationResponseTypeDef = TypedDict(
-    "CreateLicenseConfigurationResponseTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LicenseConversionContextTypeDef = TypedDict(
     "LicenseConversionContextTypeDef",
     {
         "UsageOperation": str,
     },
     total=False,
 )
 
-CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
-    "CreateLicenseConversionTaskForResourceResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportContextTypeDef = TypedDict(
     "ReportContextTypeDef",
     {
         "licenseConfigurationArns": Sequence[str],
     },
 )
 
@@ -361,39 +336,33 @@
     {
         "value": int,
         "period": ReportFrequencyTypeType,
     },
     total=False,
 )
 
-CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
-    "CreateLicenseManagerReportGeneratorResponseTypeDef",
-    {
-        "LicenseManagerReportGeneratorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDatetimeRangeTypeDef = TypedDict(
     "_RequiredDatetimeRangeTypeDef",
     {
         "Begin": str,
     },
 )
 _OptionalDatetimeRangeTypeDef = TypedDict(
     "_OptionalDatetimeRangeTypeDef",
     {
         "End": str,
     },
     total=False,
 )
 
+
 class DatetimeRangeTypeDef(_RequiredDatetimeRangeTypeDef, _OptionalDatetimeRangeTypeDef):
     pass
 
+
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "Unit": EntitlementUnitType,
     },
 )
@@ -404,53 +373,37 @@
         "MaxCount": int,
         "Overage": bool,
         "AllowCheckIn": bool,
     },
     total=False,
 )
 
+
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
+
 _RequiredIssuerTypeDef = TypedDict(
     "_RequiredIssuerTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalIssuerTypeDef = TypedDict(
     "_OptionalIssuerTypeDef",
     {
         "SignKey": str,
     },
     total=False,
 )
 
+
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
-CreateLicenseResponseTypeDef = TypedDict(
-    "CreateLicenseResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Status": LicenseStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLicenseVersionResponseTypeDef = TypedDict(
-    "CreateLicenseVersionResponseTypeDef",
-    {
-        "LicenseArn": str,
-        "Version": str,
-        "Status": LicenseStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
@@ -461,28 +414,20 @@
         "RoleArns": Sequence[str],
         "ExpirationInDays": int,
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
-    {
-        "TokenId": str,
-        "TokenType": Literal["REFRESH_TOKEN"],
-        "Token": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
@@ -491,28 +436,20 @@
     "_OptionalDeleteGrantRequestRequestTypeDef",
     {
         "StatusReason": str,
     },
     total=False,
 )
 
+
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
-DeleteGrantResponseTypeDef = TypedDict(
-    "DeleteGrantResponseTypeDef",
-    {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
@@ -528,23 +465,14 @@
     "DeleteLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "SourceVersion": str,
     },
 )
 
-DeleteLicenseResponseTypeDef = TypedDict(
-    "DeleteLicenseResponseTypeDef",
-    {
-        "Status": LicenseDeletionStatusType,
-        "DeletionDate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
@@ -560,45 +488,40 @@
     "_OptionalEntitlementUsageTypeDef",
     {
         "MaxCount": str,
     },
     total=False,
 )
 
+
 class EntitlementUsageTypeDef(_RequiredEntitlementUsageTypeDef, _OptionalEntitlementUsageTypeDef):
     pass
 
+
 _RequiredExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_RequiredExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "LicenseConsumptionToken": str,
     },
 )
 _OptionalExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_OptionalExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
-ExtendLicenseConsumptionResponseTypeDef = TypedDict(
-    "ExtendLicenseConsumptionResponseTypeDef",
-    {
-        "LicenseConsumptionToken": str,
-        "Expiration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
@@ -615,26 +538,20 @@
     "_OptionalGetAccessTokenRequestRequestTypeDef",
     {
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
+
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
-GetAccessTokenResponseTypeDef = TypedDict(
-    "GetAccessTokenResponseTypeDef",
-    {
-        "AccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
@@ -642,19 +559,21 @@
     "_OptionalGetGrantRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetGrantRequestRequestTypeDef(
     _RequiredGetGrantRequestRequestTypeDef, _OptionalGetGrantRequestRequestTypeDef
 ):
     pass
 
+
 GetLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "GetLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -691,19 +610,21 @@
     "_OptionalGetLicenseRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetLicenseRequestRequestTypeDef(
     _RequiredGetLicenseRequestRequestTypeDef, _OptionalGetLicenseRequestRequestTypeDef
 ):
     pass
 
+
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
@@ -745,17 +666,19 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 LicenseConfigurationAssociationTypeDef = TypedDict(
     "LicenseConfigurationAssociationTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
@@ -787,39 +710,31 @@
     "_OptionalLicenseSpecificationTypeDef",
     {
         "AmiAssociationScope": str,
     },
     total=False,
 )
 
+
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
-_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+
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
 
-class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
-    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -827,20 +742,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationsForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
@@ -848,39 +765,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
-    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
-):
-    pass
 
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
@@ -889,20 +788,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLicenseVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseVersionsRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 _OptionalListLicenseVersionsRequestRequestTypeDef = TypedDict(
@@ -910,20 +811,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLicenseVersionsRequestRequestTypeDef(
     _RequiredListLicenseVersionsRequestRequestTypeDef,
     _OptionalListLicenseVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceInventoryTypeDef = TypedDict(
     "ResourceInventoryTypeDef",
     {
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "ResourceArn": str,
         "Platform": str,
@@ -950,24 +853,36 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredProductInformationFilterOutputTypeDef = TypedDict(
+    "_RequiredProductInformationFilterOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProductInformationFilterName": str,
+        "ProductInformationFilterComparator": str,
+    },
+)
+_OptionalProductInformationFilterOutputTypeDef = TypedDict(
+    "_OptionalProductInformationFilterOutputTypeDef",
+    {
+        "ProductInformationFilterValue": List[str],
     },
     total=False,
 )
 
+
+class ProductInformationFilterOutputTypeDef(
+    _RequiredProductInformationFilterOutputTypeDef, _OptionalProductInformationFilterOutputTypeDef
+):
+    pass
+
+
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -975,64 +890,182 @@
     "_OptionalProductInformationFilterTypeDef",
     {
         "ProductInformationFilterValue": Sequence[str],
     },
     total=False,
 )
 
+
 class ProductInformationFilterTypeDef(
     _RequiredProductInformationFilterTypeDef, _OptionalProductInformationFilterTypeDef
 ):
     pass
 
+
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-RejectGrantResponseTypeDef = TypedDict(
-    "RejectGrantResponseTypeDef",
+ReportContextOutputTypeDef = TypedDict(
+    "ReportContextOutputTypeDef",
     {
-        "GrantArn": str,
-        "Status": GrantStatusType,
-        "Version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "licenseConfigurationArns": List[str],
     },
 )
 
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AcceptGrantResponseTypeDef = TypedDict(
+    "AcceptGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantResponseTypeDef = TypedDict(
+    "CreateGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGrantVersionResponseTypeDef = TypedDict(
+    "CreateGrantVersionResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseConfigurationResponseTypeDef = TypedDict(
+    "CreateLicenseConfigurationResponseTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseConversionTaskForResourceResponseTypeDef = TypedDict(
+    "CreateLicenseConversionTaskForResourceResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
+    "CreateLicenseManagerReportGeneratorResponseTypeDef",
+    {
+        "LicenseManagerReportGeneratorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseResponseTypeDef = TypedDict(
+    "CreateLicenseResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Status": LicenseStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLicenseVersionResponseTypeDef = TypedDict(
+    "CreateLicenseVersionResponseTypeDef",
+    {
+        "LicenseArn": str,
+        "Version": str,
+        "Status": LicenseStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
+    {
+        "TokenId": str,
+        "TokenType": Literal["REFRESH_TOKEN"],
+        "Token": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGrantResponseTypeDef = TypedDict(
+    "DeleteGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLicenseResponseTypeDef = TypedDict(
+    "DeleteLicenseResponseTypeDef",
+    {
+        "Status": LicenseDeletionStatusType,
+        "DeletionDate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExtendLicenseConsumptionResponseTypeDef = TypedDict(
+    "ExtendLicenseConsumptionResponseTypeDef",
+    {
+        "LicenseConsumptionToken": str,
+        "Expiration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessTokenResponseTypeDef = TypedDict(
+    "GetAccessTokenResponseTypeDef",
+    {
+        "AccessToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectGrantResponseTypeDef = TypedDict(
+    "RejectGrantResponseTypeDef",
+    {
+        "GrantArn": str,
+        "Status": GrantStatusType,
+        "Version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCheckoutLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutLicenseRequestRequestTypeDef",
     {
         "ProductSKU": str,
         "CheckoutType": CheckoutTypeType,
         "KeyFingerprint": str,
         "Entitlements": Sequence[EntitlementDataTypeDef],
@@ -1044,31 +1077,33 @@
     {
         "Beneficiary": str,
         "NodeId": str,
     },
     total=False,
 )
 
+
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
+
 CheckoutLicenseResponseTypeDef = TypedDict(
     "CheckoutLicenseResponseTypeDef",
     {
         "CheckoutType": CheckoutTypeType,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "SignedToken": str,
         "NodeId": str,
         "IssuedAt": str,
         "Expiration": str,
         "LicenseArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
@@ -1082,32 +1117,34 @@
     {
         "NodeId": str,
         "CheckoutMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
+
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
+
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
         "CheckoutMetadata": List[MetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
@@ -1148,20 +1185,22 @@
         "StatusReason": str,
         "SourceVersion": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
+
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGrantTypeDef = TypedDict(
     "_RequiredGrantTypeDef",
     {
         "GrantArn": str,
         "GrantName": str,
         "ParentArn": str,
         "LicenseArn": str,
@@ -1177,22 +1216,24 @@
     {
         "StatusReason": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
+
 class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1217,15 +1258,15 @@
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
         "StatusMessage": str,
         "Status": LicenseConversionTaskStatusType,
         "StartTime": datetime,
         "LicenseConversionTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConversionTaskTypeDef = TypedDict(
     "LicenseConversionTaskTypeDef",
     {
         "LicenseConversionTaskId": str,
@@ -1256,20 +1297,22 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
@@ -1281,20 +1324,22 @@
     "_OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
+
 LicenseUsageTypeDef = TypedDict(
     "LicenseUsageTypeDef",
     {
         "EntitlementUsages": List[EntitlementUsageTypeDef],
     },
     total=False,
 )
@@ -1306,24 +1351,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
-    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
-    {
-        "LicenseConfigurationArns": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLicenseConfigurationsRequestRequestTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1374,20 +1409,22 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListReceivedGrantsForOrganizationRequestRequestTypeDef(
     _RequiredListReceivedGrantsForOrganizationRequestRequestTypeDef,
     _OptionalListReceivedGrantsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 ListReceivedGrantsRequestRequestTypeDef = TypedDict(
     "ListReceivedGrantsRequestRequestTypeDef",
     {
         "GrantArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
@@ -1423,35 +1460,14 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
-    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
-    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredListUsageForLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef = TypedDict(
@@ -1460,52 +1476,45 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingsRequestRequestTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
     },
     total=False,
 )
 
-ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
-    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
-    {
-        "Filters": Sequence[InventoryFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceInventoryRequestRequestTypeDef = TypedDict(
     "ListResourceInventoryRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
@@ -1513,33 +1522,33 @@
 )
 
 ListAssociationsForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationAssociations": List[LicenseConfigurationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageForLicenseConfigurationResponseTypeDef = TypedDict(
     "ListUsageForLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationUsageList": List[LicenseConfigurationUsageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
         "LicenseSpecifications": List[LicenseSpecificationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1550,52 +1559,149 @@
     {
         "AddLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
         "RemoveLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
+    _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+
+ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
+    "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
+    {
+        "LicenseConfigurationArns": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
+    _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
+    "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
+    {
+        "Filters": Sequence[InventoryFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef = TypedDict(
+    "_OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
+    _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+    _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
+):
+    pass
+
+
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTokensResponseTypeDef = TypedDict(
     "ListTokensResponseTypeDef",
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProductInformationOutputTypeDef = TypedDict(
+    "ProductInformationOutputTypeDef",
+    {
+        "ResourceType": str,
+        "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
     },
 )
 
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
+ReportContextUnionTypeDef = Union[ReportContextTypeDef, ReportContextOutputTypeDef]
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
-        "ReportContext": ReportContextTypeDef,
+        "ReportContext": ReportContextOutputTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
@@ -1607,15 +1713,15 @@
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
@@ -1634,19 +1740,21 @@
     "_OptionalCreateLicenseRequestRequestTypeDef",
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseRequestRequestTypeDef(
     _RequiredCreateLicenseRequestRequestTypeDef, _OptionalCreateLicenseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLicenseVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseVersionRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "Issuer": IssuerTypeDef,
@@ -1663,20 +1771,22 @@
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
         "SourceVersion": str,
     },
     total=False,
 )
 
+
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GrantedLicenseTypeDef = TypedDict(
     "GrantedLicenseTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
@@ -1716,89 +1826,62 @@
     total=False,
 )
 
 GetGrantResponseTypeDef = TypedDict(
     "GetGrantResponseTypeDef",
     {
         "Grant": GrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDistributedGrantsResponseTypeDef = TypedDict(
     "ListDistributedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedGrantsResponseTypeDef = TypedDict(
     "ListReceivedGrantsResponseTypeDef",
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseConversionTasksResponseTypeDef = TypedDict(
     "ListLicenseConversionTasksResponseTypeDef",
     {
         "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseUsageResponseTypeDef = TypedDict(
     "GetLicenseUsageResponseTypeDef",
     {
         "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
-    },
-    total=False,
-)
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1808,18 +1891,18 @@
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "Tags": List[TagTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
     "LicenseConfigurationTypeDef",
     {
         "LicenseConfigurationId": str,
@@ -1832,109 +1915,140 @@
         "LicenseCountHardLimit": bool,
         "DisassociateWhenNotFound": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
-        "LicenseRules": Sequence[str],
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "Name": str,
-        "Description": str,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
-        "DisassociateWhenNotFound": bool,
-    },
-    total=False,
-)
-
-class UpdateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
+ProductInformationUnionTypeDef = Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseManagerReportGeneratorsResponseTypeDef = TypedDict(
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     {
         "ReportGenerators": List[ReportGeneratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesForOrganizationResponseTypeDef = TypedDict(
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReceivedLicensesResponseTypeDef = TypedDict(
     "ListReceivedLicensesResponseTypeDef",
     {
         "Licenses": List[GrantedLicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLicenseResponseTypeDef = TypedDict(
     "GetLicenseResponseTypeDef",
     {
         "License": LicenseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseVersionsResponseTypeDef = TypedDict(
     "ListLicenseVersionsResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicensesResponseTypeDef = TypedDict(
     "ListLicensesResponseTypeDef",
     {
         "Licenses": List[LicenseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLicenseConfigurationsResponseTypeDef = TypedDict(
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
     },
 )
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
+        "LicenseRules": Sequence[str],
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "Name": str,
+        "Description": str,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+        "DisassociateWhenNotFound": bool,
+    },
+    total=False,
+)
+
+
+class UpdateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore license-manager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore license-manager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-license-manager"></a>
 
 # types-aiobotocore-license-manager
 
 [![PyPI - types-aiobotocore-license-manager](https://img.shields.io/pypi/v/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-license-manager?color=blue)](https://pypistats.org/packages/types-aiobotocore-license-manager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-license-manager)](https://pepy.tech/project/types-aiobotocore-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LicenseManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [types-aiobotocore-license-manager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/).
 
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
@@ -348,93 +347,93 @@
 )
 
 
 def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_license_manager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
-    AcceptGrantResponseTypeDef,
+    ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
     ConsumedLicenseSummaryTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
-    CreateGrantResponseTypeDef,
     OptionsTypeDef,
-    CreateGrantVersionResponseTypeDef,
     TagTypeDef,
-    CreateLicenseConfigurationResponseTypeDef,
     LicenseConversionContextTypeDef,
-    CreateLicenseConversionTaskForResourceResponseTypeDef,
     ReportContextTypeDef,
     ReportFrequencyTypeDef,
-    CreateLicenseManagerReportGeneratorResponseTypeDef,
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
-    CreateLicenseResponseTypeDef,
-    CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
     DeleteGrantRequestRequestTypeDef,
-    DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
-    DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
-    ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
-    GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
     OrganizationConfigurationTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
     LicenseSpecificationTypeDef,
-    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
-    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
-    PaginatorConfigTypeDef,
+    ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
-    RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
     S3LocationTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AcceptGrantResponseTypeDef,
+    CreateGrantResponseTypeDef,
+    CreateGrantVersionResponseTypeDef,
+    CreateLicenseConfigurationResponseTypeDef,
+    CreateLicenseConversionTaskForResourceResponseTypeDef,
+    CreateLicenseManagerReportGeneratorResponseTypeDef,
+    CreateLicenseResponseTypeDef,
+    CreateLicenseVersionResponseTypeDef,
+    CreateTokenResponseTypeDef,
+    DeleteGrantResponseTypeDef,
+    DeleteLicenseResponseTypeDef,
+    ExtendLicenseConsumptionResponseTypeDef,
+    GetAccessTokenResponseTypeDef,
+    RejectGrantResponseTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
     CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
@@ -444,65 +443,70 @@
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
     GetLicenseConversionTaskResponseTypeDef,
     LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
-    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
     ListLicenseManagerReportGeneratorsRequestRequestTypeDef,
     ListLicensesRequestRequestTypeDef,
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
-    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
-    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
+    ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
+    ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
+    ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
+    ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
+    ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
+    ReportContextUnionTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
-    UpdateLicenseConfigurationRequestRequestTypeDef,
+    ProductInformationUnionTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
     ListLicensesResponseTypeDef,
     ListLicenseConfigurationsResponseTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
+    UpdateLicenseConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptGrantRequestRequestTypeDef:
+def get_value() -> AcceptGrantRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-license-manager-2.5.2/types_aiobotocore_license_manager.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


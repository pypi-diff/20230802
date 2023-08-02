# Comparing `tmp/types-aiobotocore-servicecatalog-2.5.2.tar.gz` & `tmp/types-aiobotocore-servicecatalog-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicecatalog-2.5.2.tar", last modified: Sat Jul  8 01:44:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicecatalog-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:00 2023, max compression
```

## Comparing `types-aiobotocore-servicecatalog-2.5.2.tar` & `types-aiobotocore-servicecatalog-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.110896 types-aiobotocore-servicecatalog-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28159 2023-07-08 01:44:19.110896 types-aiobotocore-servicecatalog-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:19.110896 types-aiobotocore-servicecatalog-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.106896 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79727 2023-07-08 01:40:53.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-07-08 01:40:53.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-08 01:40:53.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-07-08 01:40:53.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-07-08 01:40:53.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102873 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102728 2023-07-08 01:40:54.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:52.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.110896 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28159 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26549 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:49:31.000000 types-aiobotocore-servicecatalog-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.705458 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79727 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22687 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   102707 2023-08-02 14:49:34.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102562 2023-08-02 14:49:33.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/LICENSE` & `types-aiobotocore-servicecatalog-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/PKG-INFO` & `types-aiobotocore-servicecatalog-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServiceCatalog 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServiceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore servicecatalog type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicecatalog"></a>
 
 # types-aiobotocore-servicecatalog
 
 [![PyPI - types-aiobotocore-servicecatalog](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicecatalog?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicecatalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog)](https://pepy.tech/project/types-aiobotocore-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [types-aiobotocore-servicecatalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/).
 
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
@@ -417,62 +416,58 @@
 )
 
 
 def check_value(value: AccessLevelFilterKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicecatalog.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_servicecatalog.type_defs import (
     AcceptPortfolioShareInputRequestTypeDef,
     AccessLevelFilterTypeDef,
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
     AssociateProductWithPortfolioInputRequestTypeDef,
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
+    ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
-    CopyProductOutputTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
     OrganizationNodeTypeDef,
-    CreatePortfolioShareOutputTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
-    CreateProvisionedProductPlanOutputTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
     DeleteConstraintInputRequestTypeDef,
     DeletePortfolioInputRequestTypeDef,
-    DeletePortfolioShareOutputTypeDef,
     DeleteProductInputRequestTypeDef,
     DeleteProvisionedProductPlanInputRequestTypeDef,
     DeleteProvisioningArtifactInputRequestTypeDef,
     DeleteServiceActionInputRequestTypeDef,
     DeleteTagOptionInputRequestTypeDef,
     DescribeConstraintInputRequestTypeDef,
     DescribeCopyProductStatusInputRequestTypeDef,
-    DescribeCopyProductStatusOutputTypeDef,
     DescribePortfolioInputRequestTypeDef,
     DescribePortfolioShareStatusInputRequestTypeDef,
     DescribePortfolioSharesInputRequestTypeDef,
     PortfolioShareDetailTypeDef,
     DescribeProductAsAdminInputRequestTypeDef,
     ProvisioningArtifactSummaryTypeDef,
     DescribeProductInputRequestTypeDef,
@@ -499,85 +494,75 @@
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
     UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
-    GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
-    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
-    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
-    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListLaunchPathsInputRequestTypeDef,
-    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
-    ListPortfolioAccessOutputTypeDef,
-    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
-    ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPortfoliosInputRequestTypeDef,
-    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
-    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     ListProvisioningArtifactsInputRequestTypeDef,
     ListRecordHistorySearchFilterTypeDef,
-    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListResourcesForTagOptionInputRequestTypeDef,
     ResourceDetailTypeDef,
-    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
-    ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
-    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
     TerminateProvisionedProductInputRequestTypeDef,
     UpdateConstraintInputRequestTypeDef,
-    UpdatePortfolioShareOutputTypeDef,
     UpdateProvisioningPreferencesTypeDef,
     UpdateProvisionedProductPropertiesInputRequestTypeDef,
-    UpdateProvisionedProductPropertiesOutputTypeDef,
     UpdateProvisioningArtifactInputRequestTypeDef,
     UpdateServiceActionInputRequestTypeDef,
     UpdateTagOptionInputRequestTypeDef,
-    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisionedProductPlansInputRequestTypeDef,
     ScanProvisionedProductsInputRequestTypeDef,
-    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProvisionedProductsInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef,
+    CopyProductOutputTypeDef,
+    CreatePortfolioShareOutputTypeDef,
+    CreateProvisionedProductPlanOutputTypeDef,
+    DeletePortfolioShareOutputTypeDef,
+    DescribeCopyProductStatusOutputTypeDef,
+    GetAWSOrganizationsAccessStatusOutputTypeDef,
+    ListPortfolioAccessOutputTypeDef,
+    UpdatePortfolioShareOutputTypeDef,
+    UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
@@ -610,14 +595,28 @@
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     EngineWorkflowResourceIdentifierTypeDef,
+    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    ListPortfoliosInputListPortfoliosPaginateTypeDef,
+    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
+    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    ListServiceActionsInputListServiceActionsPaginateTypeDef,
+    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
+    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
@@ -660,15 +659,15 @@
     CreateProductOutputTypeDef,
     DescribeProductAsAdminOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     UpdateProductOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptPortfolioShareInputRequestTypeDef:
+def get_value() -> AcceptPortfolioShareInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/README.md` & `types-aiobotocore-servicecatalog-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-servicecatalog"></a>
 
 # types-aiobotocore-servicecatalog
 
 [![PyPI - types-aiobotocore-servicecatalog](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicecatalog?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicecatalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog)](https://pepy.tech/project/types-aiobotocore-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [types-aiobotocore-servicecatalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/).
 
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
@@ -384,62 +384,58 @@
 )
 
 
 def check_value(value: AccessLevelFilterKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicecatalog.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_servicecatalog.type_defs import (
     AcceptPortfolioShareInputRequestTypeDef,
     AccessLevelFilterTypeDef,
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
     AssociateProductWithPortfolioInputRequestTypeDef,
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
+    ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
-    CopyProductOutputTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
     OrganizationNodeTypeDef,
-    CreatePortfolioShareOutputTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
-    CreateProvisionedProductPlanOutputTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
     DeleteConstraintInputRequestTypeDef,
     DeletePortfolioInputRequestTypeDef,
-    DeletePortfolioShareOutputTypeDef,
     DeleteProductInputRequestTypeDef,
     DeleteProvisionedProductPlanInputRequestTypeDef,
     DeleteProvisioningArtifactInputRequestTypeDef,
     DeleteServiceActionInputRequestTypeDef,
     DeleteTagOptionInputRequestTypeDef,
     DescribeConstraintInputRequestTypeDef,
     DescribeCopyProductStatusInputRequestTypeDef,
-    DescribeCopyProductStatusOutputTypeDef,
     DescribePortfolioInputRequestTypeDef,
     DescribePortfolioShareStatusInputRequestTypeDef,
     DescribePortfolioSharesInputRequestTypeDef,
     PortfolioShareDetailTypeDef,
     DescribeProductAsAdminInputRequestTypeDef,
     ProvisioningArtifactSummaryTypeDef,
     DescribeProductInputRequestTypeDef,
@@ -466,85 +462,75 @@
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
     UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
-    GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
-    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
-    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
-    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListLaunchPathsInputRequestTypeDef,
-    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
-    ListPortfolioAccessOutputTypeDef,
-    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
-    ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPortfoliosInputRequestTypeDef,
-    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
-    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     ListProvisioningArtifactsInputRequestTypeDef,
     ListRecordHistorySearchFilterTypeDef,
-    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListResourcesForTagOptionInputRequestTypeDef,
     ResourceDetailTypeDef,
-    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
-    ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
-    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
     TerminateProvisionedProductInputRequestTypeDef,
     UpdateConstraintInputRequestTypeDef,
-    UpdatePortfolioShareOutputTypeDef,
     UpdateProvisioningPreferencesTypeDef,
     UpdateProvisionedProductPropertiesInputRequestTypeDef,
-    UpdateProvisionedProductPropertiesOutputTypeDef,
     UpdateProvisioningArtifactInputRequestTypeDef,
     UpdateServiceActionInputRequestTypeDef,
     UpdateTagOptionInputRequestTypeDef,
-    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisionedProductPlansInputRequestTypeDef,
     ScanProvisionedProductsInputRequestTypeDef,
-    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProvisionedProductsInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef,
+    CopyProductOutputTypeDef,
+    CreatePortfolioShareOutputTypeDef,
+    CreateProvisionedProductPlanOutputTypeDef,
+    DeletePortfolioShareOutputTypeDef,
+    DescribeCopyProductStatusOutputTypeDef,
+    GetAWSOrganizationsAccessStatusOutputTypeDef,
+    ListPortfolioAccessOutputTypeDef,
+    UpdatePortfolioShareOutputTypeDef,
+    UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
@@ -577,14 +563,28 @@
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     EngineWorkflowResourceIdentifierTypeDef,
+    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    ListPortfoliosInputListPortfoliosPaginateTypeDef,
+    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
+    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    ListServiceActionsInputListServiceActionsPaginateTypeDef,
+    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
+    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
@@ -627,15 +627,15 @@
     CreateProductOutputTypeDef,
     DescribeProductAsAdminOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     UpdateProductOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptPortfolioShareInputRequestTypeDef:
+def get_value() -> AcceptPortfolioShareInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/setup.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicecatalog",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServiceCatalog 2.5.2 service generated with"
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
-    keywords="aiobotocore servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore servicecatalog type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_servicecatalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/"
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/__init__.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/__init__.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/__main__.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceCatalog 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ServiceCatalog 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
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

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/client.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/client.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/literals.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/literals.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/paginator.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         PortfolioShareType: PortfolioShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAcceptedPortfolioSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listacceptedportfoliosharespaginator)
         """
 
 
@@ -149,15 +149,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConstraintsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listconstraintsforportfoliopaginator)
         """
 
 
@@ -168,15 +168,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchPathsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listlaunchpathspaginator)
         """
 
 
@@ -188,30 +188,30 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationPortfolioAccessOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listorganizationportfolioaccesspaginator)
         """
 
 
 class ListPortfoliosPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliospaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPortfoliosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliospaginator)
         """
 
 
@@ -222,15 +222,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPortfoliosForProductOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliosforproductpaginator)
         """
 
 
@@ -241,15 +241,15 @@
     """
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPrincipalsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprincipalsforportfoliopaginator)
         """
 
 
@@ -261,15 +261,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisionedProductPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisionedproductplanspaginator)
         """
 
 
@@ -280,15 +280,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceActionId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisioningartifactsforserviceactionpaginator)
         """
 
 
@@ -300,15 +300,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecordHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listrecordhistorypaginator)
         """
 
 
@@ -319,30 +319,30 @@
     """
 
     def paginate(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesForTagOptionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listresourcesfortagoptionpaginator)
         """
 
 
 class ListServiceActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionspaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionspaginator)
         """
 
 
@@ -354,15 +354,15 @@
 
     def paginate(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionsforprovisioningartifactpaginator)
         """
 
 
@@ -372,15 +372,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagOptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
         """
 
 
@@ -391,15 +391,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScanProvisionedProductsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#scanprovisionedproductspaginator)
         """
 
 
@@ -414,13 +414,13 @@
         *,
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         ProductSource: Literal["ACCOUNT"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchProductsAsAdminOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#searchproductsasadminpaginator)
         """
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/paginator.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         PortfolioShareType: PortfolioShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAcceptedPortfolioSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listacceptedportfoliosharespaginator)
         """
 
 class ListConstraintsForPortfolioPaginator(AioPaginator):
@@ -144,15 +144,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConstraintsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listconstraintsforportfoliopaginator)
         """
 
 class ListLaunchPathsPaginator(AioPaginator):
@@ -162,15 +162,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchPathsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listlaunchpathspaginator)
         """
 
 class ListOrganizationPortfolioAccessPaginator(AioPaginator):
@@ -181,29 +181,29 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationPortfolioAccessOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listorganizationportfolioaccesspaginator)
         """
 
 class ListPortfoliosPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliospaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPortfoliosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliospaginator)
         """
 
 class ListPortfoliosForProductPaginator(AioPaginator):
@@ -213,15 +213,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPortfoliosForProductOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listportfoliosforproductpaginator)
         """
 
 class ListPrincipalsForPortfolioPaginator(AioPaginator):
@@ -231,15 +231,15 @@
     """
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPrincipalsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprincipalsforportfoliopaginator)
         """
 
 class ListProvisionedProductPlansPaginator(AioPaginator):
@@ -250,15 +250,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisionedProductPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisionedproductplanspaginator)
         """
 
 class ListProvisioningArtifactsForServiceActionPaginator(AioPaginator):
@@ -268,15 +268,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceActionId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listprovisioningartifactsforserviceactionpaginator)
         """
 
 class ListRecordHistoryPaginator(AioPaginator):
@@ -287,15 +287,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecordHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listrecordhistorypaginator)
         """
 
 class ListResourcesForTagOptionPaginator(AioPaginator):
@@ -305,29 +305,29 @@
     """
 
     def paginate(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesForTagOptionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listresourcesfortagoptionpaginator)
         """
 
 class ListServiceActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionspaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionspaginator)
         """
 
 class ListServiceActionsForProvisioningArtifactPaginator(AioPaginator):
@@ -338,15 +338,15 @@
 
     def paginate(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listserviceactionsforprovisioningartifactpaginator)
         """
 
 class ListTagOptionsPaginator(AioPaginator):
@@ -355,15 +355,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagOptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#listtagoptionspaginator)
         """
 
 class ScanProvisionedProductsPaginator(AioPaginator):
@@ -373,15 +373,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScanProvisionedProductsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#scanprovisionedproductspaginator)
         """
 
 class SearchProductsAsAdminPaginator(AioPaginator):
@@ -395,13 +395,13 @@
         *,
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         ProductSource: Literal["ACCOUNT"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchProductsAsAdminOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/paginators/#searchproductsasadminpaginator)
         """
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/type_defs.py` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_servicecatalog.type_defs import AcceptPortfolioShareInputRequestTypeDef
 
-    data: AcceptPortfolioShareInputRequestTypeDef = {...}
+    data: AcceptPortfolioShareInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -53,55 +53,50 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptPortfolioShareInputRequestTypeDef",
     "AccessLevelFilterTypeDef",
     "AssociateBudgetWithResourceInputRequestTypeDef",
     "AssociatePrincipalWithPortfolioInputRequestTypeDef",
     "AssociateProductWithPortfolioInputRequestTypeDef",
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     "ServiceActionAssociationTypeDef",
     "FailedServiceActionAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "BudgetDetailTypeDef",
     "CloudWatchDashboardTypeDef",
     "CodeStarParametersTypeDef",
     "ConstraintDetailTypeDef",
     "ConstraintSummaryTypeDef",
     "CopyProductInputRequestTypeDef",
-    "CopyProductOutputTypeDef",
     "CreateConstraintInputRequestTypeDef",
     "TagTypeDef",
     "PortfolioDetailTypeDef",
     "OrganizationNodeTypeDef",
-    "CreatePortfolioShareOutputTypeDef",
     "ProvisioningArtifactPropertiesTypeDef",
     "ProvisioningArtifactDetailTypeDef",
     "UpdateProvisioningParameterTypeDef",
-    "CreateProvisionedProductPlanOutputTypeDef",
     "CreateServiceActionInputRequestTypeDef",
     "CreateTagOptionInputRequestTypeDef",
     "TagOptionDetailTypeDef",
     "DeleteConstraintInputRequestTypeDef",
     "DeletePortfolioInputRequestTypeDef",
-    "DeletePortfolioShareOutputTypeDef",
     "DeleteProductInputRequestTypeDef",
     "DeleteProvisionedProductPlanInputRequestTypeDef",
     "DeleteProvisioningArtifactInputRequestTypeDef",
     "DeleteServiceActionInputRequestTypeDef",
     "DeleteTagOptionInputRequestTypeDef",
     "DescribeConstraintInputRequestTypeDef",
     "DescribeCopyProductStatusInputRequestTypeDef",
-    "DescribeCopyProductStatusOutputTypeDef",
     "DescribePortfolioInputRequestTypeDef",
     "DescribePortfolioShareStatusInputRequestTypeDef",
     "DescribePortfolioSharesInputRequestTypeDef",
     "PortfolioShareDetailTypeDef",
     "DescribeProductAsAdminInputRequestTypeDef",
     "ProvisioningArtifactSummaryTypeDef",
     "DescribeProductInputRequestTypeDef",
@@ -128,85 +123,75 @@
     "DisassociatePrincipalFromPortfolioInputRequestTypeDef",
     "DisassociateProductFromPortfolioInputRequestTypeDef",
     "DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     "UniqueTagResourceIdentifierTypeDef",
     "ExecuteProvisionedProductPlanInputRequestTypeDef",
     "ExecuteProvisionedProductServiceActionInputRequestTypeDef",
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
     "GetProvisionedProductOutputsInputRequestTypeDef",
     "ImportAsProvisionedProductInputRequestTypeDef",
     "LastSyncTypeDef",
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     "ListBudgetsForResourceInputRequestTypeDef",
-    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
     "ListConstraintsForPortfolioInputRequestTypeDef",
-    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
     "ListLaunchPathsInputRequestTypeDef",
-    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
     "ListOrganizationPortfolioAccessInputRequestTypeDef",
     "ListPortfolioAccessInputRequestTypeDef",
-    "ListPortfolioAccessOutputTypeDef",
-    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
     "ListPortfoliosForProductInputRequestTypeDef",
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
     "ListPortfoliosInputRequestTypeDef",
-    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
     "ListPrincipalsForPortfolioInputRequestTypeDef",
     "PrincipalTypeDef",
     "ProvisionedProductPlanSummaryTypeDef",
-    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
     "ListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     "ListProvisioningArtifactsInputRequestTypeDef",
     "ListRecordHistorySearchFilterTypeDef",
-    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
     "ListResourcesForTagOptionInputRequestTypeDef",
     "ResourceDetailTypeDef",
-    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
     "ListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     "ServiceActionSummaryTypeDef",
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
     "ListServiceActionsInputRequestTypeDef",
     "ListStackInstancesForProvisionedProductInputRequestTypeDef",
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
     "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchProductsAsAdminInputRequestTypeDef",
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
     "SearchProductsInputRequestTypeDef",
     "ShareErrorTypeDef",
     "TerminateProvisionedProductInputRequestTypeDef",
     "UpdateConstraintInputRequestTypeDef",
-    "UpdatePortfolioShareOutputTypeDef",
     "UpdateProvisioningPreferencesTypeDef",
     "UpdateProvisionedProductPropertiesInputRequestTypeDef",
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "UpdateProvisioningArtifactInputRequestTypeDef",
     "UpdateServiceActionInputRequestTypeDef",
     "UpdateTagOptionInputRequestTypeDef",
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
     "ListProvisionedProductPlansInputRequestTypeDef",
     "ScanProvisionedProductsInputRequestTypeDef",
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
     "SearchProvisionedProductsInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
+    "CopyProductOutputTypeDef",
+    "CreatePortfolioShareOutputTypeDef",
+    "CreateProvisionedProductPlanOutputTypeDef",
+    "DeletePortfolioShareOutputTypeDef",
+    "DescribeCopyProductStatusOutputTypeDef",
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    "ListPortfolioAccessOutputTypeDef",
+    "UpdatePortfolioShareOutputTypeDef",
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "ListBudgetsForResourceOutputTypeDef",
     "SourceConnectionParametersTypeDef",
     "CreateConstraintOutputTypeDef",
     "DescribeConstraintOutputTypeDef",
     "ListConstraintsForPortfolioOutputTypeDef",
     "UpdateConstraintOutputTypeDef",
     "CreatePortfolioInputRequestTypeDef",
@@ -239,14 +224,28 @@
     "ProvisioningArtifactViewTypeDef",
     "DescribeProvisionedProductOutputTypeDef",
     "ScanProvisionedProductsOutputTypeDef",
     "GetProvisionedProductOutputsOutputTypeDef",
     "NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     "EngineWorkflowResourceIdentifierTypeDef",
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
     "ListPrincipalsForPortfolioOutputTypeDef",
     "ListProvisionedProductPlansOutputTypeDef",
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     "ListRecordHistoryInputRequestTypeDef",
     "ListResourcesForTagOptionOutputTypeDef",
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     "ListServiceActionsOutputTypeDef",
@@ -303,22 +302,20 @@
     {
         "AcceptLanguage": str,
         "PortfolioShareType": PortfolioShareTypeType,
     },
     total=False,
 )
 
-
 class AcceptPortfolioShareInputRequestTypeDef(
     _RequiredAcceptPortfolioShareInputRequestTypeDef,
     _OptionalAcceptPortfolioShareInputRequestTypeDef,
 ):
     pass
 
-
 AccessLevelFilterTypeDef = TypedDict(
     "AccessLevelFilterTypeDef",
     {
         "Key": AccessLevelFilterKeyType,
         "Value": str,
     },
     total=False,
@@ -344,22 +341,20 @@
     "_OptionalAssociatePrincipalWithPortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class AssociatePrincipalWithPortfolioInputRequestTypeDef(
     _RequiredAssociatePrincipalWithPortfolioInputRequestTypeDef,
     _OptionalAssociatePrincipalWithPortfolioInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredAssociateProductWithPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredAssociateProductWithPortfolioInputRequestTypeDef",
     {
         "ProductId": str,
         "PortfolioId": str,
     },
 )
@@ -368,22 +363,20 @@
     {
         "AcceptLanguage": str,
         "SourcePortfolioId": str,
     },
     total=False,
 )
 
-
 class AssociateProductWithPortfolioInputRequestTypeDef(
     _RequiredAssociateProductWithPortfolioInputRequestTypeDef,
     _OptionalAssociateProductWithPortfolioInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
         "ServiceActionId": str,
     },
@@ -392,22 +385,20 @@
     "_OptionalAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef(
     _RequiredAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     _OptionalAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 AssociateTagOptionWithResourceInputRequestTypeDef = TypedDict(
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagOptionId": str,
     },
 )
@@ -429,14 +420,25 @@
         "ProvisioningArtifactId": str,
         "ErrorCode": ServiceActionAssociationErrorCodeType,
         "ErrorMessage": str,
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
 BudgetDetailTypeDef = TypedDict(
     "BudgetDetailTypeDef",
     {
         "BudgetName": str,
     },
     total=False,
 )
@@ -496,29 +498,19 @@
         "TargetProductName": str,
         "SourceProvisioningArtifactIdentifiers": Sequence[Mapping[Literal["Id"], str]],
         "CopyOptions": Sequence[Literal["CopyTags"]],
     },
     total=False,
 )
 
-
 class CopyProductInputRequestTypeDef(
     _RequiredCopyProductInputRequestTypeDef, _OptionalCopyProductInputRequestTypeDef
 ):
     pass
 
-
-CopyProductOutputTypeDef = TypedDict(
-    "CopyProductOutputTypeDef",
-    {
-        "CopyProductToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConstraintInputRequestTypeDef = TypedDict(
     "_RequiredCreateConstraintInputRequestTypeDef",
     {
         "PortfolioId": str,
         "ProductId": str,
         "Parameters": str,
         "Type": str,
@@ -530,21 +522,19 @@
     {
         "AcceptLanguage": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateConstraintInputRequestTypeDef(
     _RequiredCreateConstraintInputRequestTypeDef, _OptionalCreateConstraintInputRequestTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -567,22 +557,14 @@
     {
         "Type": OrganizationNodeTypeType,
         "Value": str,
     },
     total=False,
 )
 
-CreatePortfolioShareOutputTypeDef = TypedDict(
-    "CreatePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ProvisioningArtifactPropertiesTypeDef = TypedDict(
     "ProvisioningArtifactPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
         "Info": Mapping[str, str],
         "Type": ProvisioningArtifactTypeType,
@@ -612,26 +594,14 @@
         "Key": str,
         "Value": str,
         "UsePreviousValue": bool,
     },
     total=False,
 )
 
-CreateProvisionedProductPlanOutputTypeDef = TypedDict(
-    "CreateProvisionedProductPlanOutputTypeDef",
-    {
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionedProductName": str,
-        "ProvisioningArtifactId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceActionInputRequestTypeDef",
     {
         "Name": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
         "Definition": Mapping[ServiceActionDefinitionKeyType, str],
         "IdempotencyToken": str,
@@ -642,21 +612,19 @@
     {
         "Description": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class CreateServiceActionInputRequestTypeDef(
     _RequiredCreateServiceActionInputRequestTypeDef, _OptionalCreateServiceActionInputRequestTypeDef
 ):
     pass
 
-
 CreateTagOptionInputRequestTypeDef = TypedDict(
     "CreateTagOptionInputRequestTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -683,71 +651,57 @@
     "_OptionalDeleteConstraintInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DeleteConstraintInputRequestTypeDef(
     _RequiredDeleteConstraintInputRequestTypeDef, _OptionalDeleteConstraintInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeletePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDeletePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeletePortfolioInputRequestTypeDef = TypedDict(
     "_OptionalDeletePortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DeletePortfolioInputRequestTypeDef(
     _RequiredDeletePortfolioInputRequestTypeDef, _OptionalDeletePortfolioInputRequestTypeDef
 ):
     pass
 
-
-DeletePortfolioShareOutputTypeDef = TypedDict(
-    "DeletePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProductInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProductInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteProductInputRequestTypeDef = TypedDict(
     "_OptionalDeleteProductInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DeleteProductInputRequestTypeDef(
     _RequiredDeleteProductInputRequestTypeDef, _OptionalDeleteProductInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanId": str,
     },
 )
 _OptionalDeleteProvisionedProductPlanInputRequestTypeDef = TypedDict(
@@ -755,22 +709,20 @@
     {
         "AcceptLanguage": str,
         "IgnoreErrors": bool,
     },
     total=False,
 )
 
-
 class DeleteProvisionedProductPlanInputRequestTypeDef(
     _RequiredDeleteProvisionedProductPlanInputRequestTypeDef,
     _OptionalDeleteProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -778,43 +730,39 @@
     "_OptionalDeleteProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DeleteProvisioningArtifactInputRequestTypeDef(
     _RequiredDeleteProvisioningArtifactInputRequestTypeDef,
     _OptionalDeleteProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredDeleteServiceActionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteServiceActionInputRequestTypeDef = TypedDict(
     "_OptionalDeleteServiceActionInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DeleteServiceActionInputRequestTypeDef(
     _RequiredDeleteServiceActionInputRequestTypeDef, _OptionalDeleteServiceActionInputRequestTypeDef
 ):
     pass
 
-
 DeleteTagOptionInputRequestTypeDef = TypedDict(
     "DeleteTagOptionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -828,74 +776,58 @@
     "_OptionalDescribeConstraintInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DescribeConstraintInputRequestTypeDef(
     _RequiredDescribeConstraintInputRequestTypeDef, _OptionalDescribeConstraintInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeCopyProductStatusInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCopyProductStatusInputRequestTypeDef",
     {
         "CopyProductToken": str,
     },
 )
 _OptionalDescribeCopyProductStatusInputRequestTypeDef = TypedDict(
     "_OptionalDescribeCopyProductStatusInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DescribeCopyProductStatusInputRequestTypeDef(
     _RequiredDescribeCopyProductStatusInputRequestTypeDef,
     _OptionalDescribeCopyProductStatusInputRequestTypeDef,
 ):
     pass
 
-
-DescribeCopyProductStatusOutputTypeDef = TypedDict(
-    "DescribeCopyProductStatusOutputTypeDef",
-    {
-        "CopyProductStatus": CopyProductStatusType,
-        "TargetProductId": str,
-        "StatusDetail": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDescribePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribePortfolioInputRequestTypeDef = TypedDict(
     "_OptionalDescribePortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DescribePortfolioInputRequestTypeDef(
     _RequiredDescribePortfolioInputRequestTypeDef, _OptionalDescribePortfolioInputRequestTypeDef
 ):
     pass
 
-
 DescribePortfolioShareStatusInputRequestTypeDef = TypedDict(
     "DescribePortfolioShareStatusInputRequestTypeDef",
     {
         "PortfolioShareToken": str,
     },
 )
 
@@ -911,22 +843,20 @@
     {
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class DescribePortfolioSharesInputRequestTypeDef(
     _RequiredDescribePortfolioSharesInputRequestTypeDef,
     _OptionalDescribePortfolioSharesInputRequestTypeDef,
 ):
     pass
 
-
 PortfolioShareDetailTypeDef = TypedDict(
     "PortfolioShareDetailTypeDef",
     {
         "PrincipalId": str,
         "Type": DescribePortfolioShareTypeType,
         "Accepted": bool,
         "ShareTagOptions": bool,
@@ -1017,21 +947,19 @@
     "_OptionalDescribeProductViewInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DescribeProductViewInputRequestTypeDef(
     _RequiredDescribeProductViewInputRequestTypeDef, _OptionalDescribeProductViewInputRequestTypeDef
 ):
     pass
 
-
 DescribeProvisionedProductInputRequestTypeDef = TypedDict(
     "DescribeProvisionedProductInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "Id": str,
         "Name": str,
     },
@@ -1071,22 +999,20 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-
 class DescribeProvisionedProductPlanInputRequestTypeDef(
     _RequiredDescribeProvisionedProductPlanInputRequestTypeDef,
     _OptionalDescribeProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
-
 DescribeProvisioningArtifactInputRequestTypeDef = TypedDict(
     "DescribeProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisioningArtifactId": str,
         "ProductId": str,
         "ProvisioningArtifactName": str,
@@ -1159,21 +1085,19 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class DescribeRecordInputRequestTypeDef(
     _RequiredDescribeRecordInputRequestTypeDef, _OptionalDescribeRecordInputRequestTypeDef
 ):
     pass
 
-
 RecordOutputTypeDef = TypedDict(
     "RecordOutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
     },
@@ -1191,22 +1115,20 @@
     "_OptionalDescribeServiceActionExecutionParametersInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DescribeServiceActionExecutionParametersInputRequestTypeDef(
     _RequiredDescribeServiceActionExecutionParametersInputRequestTypeDef,
     _OptionalDescribeServiceActionExecutionParametersInputRequestTypeDef,
 ):
     pass
 
-
 ExecutionParameterTypeDef = TypedDict(
     "ExecutionParameterTypeDef",
     {
         "Name": str,
         "Type": str,
         "DefaultValues": List[str],
     },
@@ -1223,22 +1145,20 @@
     "_OptionalDescribeServiceActionInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DescribeServiceActionInputRequestTypeDef(
     _RequiredDescribeServiceActionInputRequestTypeDef,
     _OptionalDescribeServiceActionInputRequestTypeDef,
 ):
     pass
 
-
 DescribeTagOptionInputRequestTypeDef = TypedDict(
     "DescribeTagOptionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1262,22 +1182,20 @@
     {
         "AcceptLanguage": str,
         "PrincipalType": PrincipalTypeType,
     },
     total=False,
 )
 
-
 class DisassociatePrincipalFromPortfolioInputRequestTypeDef(
     _RequiredDisassociatePrincipalFromPortfolioInputRequestTypeDef,
     _OptionalDisassociatePrincipalFromPortfolioInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisassociateProductFromPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateProductFromPortfolioInputRequestTypeDef",
     {
         "ProductId": str,
         "PortfolioId": str,
     },
 )
@@ -1285,22 +1203,20 @@
     "_OptionalDisassociateProductFromPortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DisassociateProductFromPortfolioInputRequestTypeDef(
     _RequiredDisassociateProductFromPortfolioInputRequestTypeDef,
     _OptionalDisassociateProductFromPortfolioInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
         "ServiceActionId": str,
     },
@@ -1309,22 +1225,20 @@
     "_OptionalDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef(
     _RequiredDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     _OptionalDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 DisassociateTagOptionFromResourceInputRequestTypeDef = TypedDict(
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagOptionId": str,
     },
 )
@@ -1349,22 +1263,20 @@
     "_OptionalExecuteProvisionedProductPlanInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class ExecuteProvisionedProductPlanInputRequestTypeDef(
     _RequiredExecuteProvisionedProductPlanInputRequestTypeDef,
     _OptionalExecuteProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef",
     {
         "ProvisionedProductId": str,
         "ServiceActionId": str,
         "ExecuteToken": str,
     },
@@ -1374,30 +1286,20 @@
     {
         "AcceptLanguage": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class ExecuteProvisionedProductServiceActionInputRequestTypeDef(
     _RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef,
     _OptionalExecuteProvisionedProductServiceActionInputRequestTypeDef,
 ):
     pass
 
-
-GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
-    {
-        "AccessStatus": AccessStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProvisionedProductOutputsInputRequestTypeDef = TypedDict(
     "GetProvisionedProductOutputsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionedProductId": str,
         "ProvisionedProductName": str,
         "OutputKeys": Sequence[str],
@@ -1421,40 +1323,38 @@
     "_OptionalImportAsProvisionedProductInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class ImportAsProvisionedProductInputRequestTypeDef(
     _RequiredImportAsProvisionedProductInputRequestTypeDef,
     _OptionalImportAsProvisionedProductInputRequestTypeDef,
 ):
     pass
 
-
 LastSyncTypeDef = TypedDict(
     "LastSyncTypeDef",
     {
         "LastSyncTime": datetime,
         "LastSyncStatus": LastSyncStatusType,
         "LastSyncStatusMessage": str,
         "LastSuccessfulSyncTime": datetime,
         "LastSuccessfulSyncProvisioningArtifactId": str,
     },
     total=False,
 )
 
-ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AcceptLanguage": str,
-        "PortfolioShareType": PortfolioShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAcceptedPortfolioSharesInputRequestTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     {
@@ -1478,46 +1378,20 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-
 class ListBudgetsForResourceInputRequestTypeDef(
     _RequiredListBudgetsForResourceInputRequestTypeDef,
     _OptionalListBudgetsForResourceInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProductId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
-    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListConstraintsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1527,45 +1401,20 @@
         "ProductId": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-
 class ListConstraintsForPortfolioInputRequestTypeDef(
     _RequiredListConstraintsForPortfolioInputRequestTypeDef,
     _OptionalListConstraintsForPortfolioInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
-    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLaunchPathsInputRequestTypeDef = TypedDict(
     "_RequiredListLaunchPathsInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListLaunchPathsInputRequestTypeDef = TypedDict(
@@ -1574,45 +1423,19 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-
 class ListLaunchPathsInputRequestTypeDef(
     _RequiredListLaunchPathsInputRequestTypeDef, _OptionalListLaunchPathsInputRequestTypeDef
 ):
     pass
 
-
-_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "PortfolioId": str,
-        "OrganizationNodeType": OrganizationNodeTypeType,
-    },
-)
-_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
-    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListOrganizationPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListOrganizationPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
         "OrganizationNodeType": OrganizationNodeTypeType,
     },
 )
@@ -1622,22 +1445,20 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListOrganizationPortfolioAccessInputRequestTypeDef(
     _RequiredListOrganizationPortfolioAccessInputRequestTypeDef,
     _OptionalListOrganizationPortfolioAccessInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPortfolioAccessInputRequestTypeDef = TypedDict(
@@ -1647,53 +1468,19 @@
         "OrganizationParentId": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListPortfolioAccessInputRequestTypeDef(
     _RequiredListPortfolioAccessInputRequestTypeDef, _OptionalListPortfolioAccessInputRequestTypeDef
 ):
     pass
 
-
-ListPortfolioAccessOutputTypeDef = TypedDict(
-    "ListPortfolioAccessOutputTypeDef",
-    {
-        "AccountIds": List[str],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
-    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPortfoliosForProductInputRequestTypeDef = TypedDict(
     "_RequiredListPortfoliosForProductInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListPortfoliosForProductInputRequestTypeDef = TypedDict(
@@ -1702,64 +1489,30 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListPortfoliosForProductInputRequestTypeDef(
     _RequiredListPortfoliosForProductInputRequestTypeDef,
     _OptionalListPortfoliosForProductInputRequestTypeDef,
 ):
     pass
 
-
-ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPortfoliosInputRequestTypeDef = TypedDict(
     "ListPortfoliosInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
-    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1768,22 +1521,20 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-
 class ListPrincipalsForPortfolioInputRequestTypeDef(
     _RequiredListPrincipalsForPortfolioInputRequestTypeDef,
     _OptionalListPrincipalsForPortfolioInputRequestTypeDef,
 ):
     pass
 
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "PrincipalARN": str,
         "PrincipalType": PrincipalTypeType,
     },
     total=False,
@@ -1798,37 +1549,14 @@
         "ProvisionProductName": str,
         "PlanType": Literal["CLOUDFORMATION"],
         "ProvisioningArtifactId": str,
     },
     total=False,
 )
 
-_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "ServiceActionId": str,
-    },
-)
-_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
-    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     {
         "ServiceActionId": str,
     },
 )
 _OptionalListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
@@ -1837,76 +1565,49 @@
         "PageSize": int,
         "PageToken": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class ListProvisioningArtifactsForServiceActionInputRequestTypeDef(
     _RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     _OptionalListProvisioningArtifactsForServiceActionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListProvisioningArtifactsInputRequestTypeDef = TypedDict(
     "_RequiredListProvisioningArtifactsInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListProvisioningArtifactsInputRequestTypeDef = TypedDict(
     "_OptionalListProvisioningArtifactsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class ListProvisioningArtifactsInputRequestTypeDef(
     _RequiredListProvisioningArtifactsInputRequestTypeDef,
     _OptionalListProvisioningArtifactsInputRequestTypeDef,
 ):
     pass
 
-
 ListRecordHistorySearchFilterTypeDef = TypedDict(
     "ListRecordHistorySearchFilterTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "TagOptionId": str,
-    },
-)
-_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
-    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesForTagOptionInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesForTagOptionInputRequestTypeDef",
     {
         "TagOptionId": str,
     },
 )
 _OptionalListResourcesForTagOptionInputRequestTypeDef = TypedDict(
@@ -1915,58 +1616,32 @@
         "ResourceType": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-
 class ListResourcesForTagOptionInputRequestTypeDef(
     _RequiredListResourcesForTagOptionInputRequestTypeDef,
     _OptionalListResourcesForTagOptionInputRequestTypeDef,
 ):
     pass
 
-
 ResourceDetailTypeDef = TypedDict(
     "ResourceDetailTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Name": str,
         "Description": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "ProductId": str,
-        "ProvisioningArtifactId": str,
-    },
-)
-_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
-    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -1976,42 +1651,31 @@
         "PageSize": int,
         "PageToken": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class ListServiceActionsForProvisioningArtifactInputRequestTypeDef(
     _RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     _OptionalListServiceActionsForProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 ServiceActionSummaryTypeDef = TypedDict(
     "ServiceActionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
     },
     total=False,
 )
 
-ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceActionsInputRequestTypeDef = TypedDict(
     "ListServiceActionsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
@@ -2030,22 +1694,20 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListStackInstancesForProvisionedProductInputRequestTypeDef(
     _RequiredListStackInstancesForProvisionedProductInputRequestTypeDef,
     _OptionalListStackInstancesForProvisionedProductInputRequestTypeDef,
 ):
     pass
 
-
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "Account": str,
         "Region": str,
         "StackInstanceStatus": StackInstanceStatusType,
     },
@@ -2075,32 +1737,20 @@
     "_OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
-
 class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
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
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
         "AllowedPattern": str,
         "ConstraintDescription": str,
         "MaxLength": str,
@@ -2171,43 +1821,30 @@
     {
         "AcceptLanguage": str,
         "PortfolioShareType": PortfolioShareTypeType,
     },
     total=False,
 )
 
-
 class RejectPortfolioShareInputRequestTypeDef(
     _RequiredRejectPortfolioShareInputRequestTypeDef,
     _OptionalRejectPortfolioShareInputRequestTypeDef,
 ):
     pass
 
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
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
 SearchProductsAsAdminInputRequestTypeDef = TypedDict(
     "SearchProductsAsAdminInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PortfolioId": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "SortBy": ProductViewSortByType,
@@ -2215,28 +1852,14 @@
         "PageToken": str,
         "PageSize": int,
         "ProductSource": Literal["ACCOUNT"],
     },
     total=False,
 )
 
-SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PortfolioId": str,
-        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
-        "SortBy": ProductViewSortByType,
-        "SortOrder": SortOrderType,
-        "ProductSource": Literal["ACCOUNT"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProductsInputRequestTypeDef = TypedDict(
     "SearchProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "PageSize": int,
         "SortBy": ProductViewSortByType,
@@ -2270,22 +1893,20 @@
         "IgnoreErrors": bool,
         "AcceptLanguage": str,
         "RetainPhysicalResources": bool,
     },
     total=False,
 )
 
-
 class TerminateProvisionedProductInputRequestTypeDef(
     _RequiredTerminateProvisionedProductInputRequestTypeDef,
     _OptionalTerminateProvisionedProductInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateConstraintInputRequestTypeDef = TypedDict(
     "_RequiredUpdateConstraintInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateConstraintInputRequestTypeDef = TypedDict(
@@ -2294,30 +1915,19 @@
         "AcceptLanguage": str,
         "Description": str,
         "Parameters": str,
     },
     total=False,
 )
 
-
 class UpdateConstraintInputRequestTypeDef(
     _RequiredUpdateConstraintInputRequestTypeDef, _OptionalUpdateConstraintInputRequestTypeDef
 ):
     pass
 
-
-UpdatePortfolioShareOutputTypeDef = TypedDict(
-    "UpdatePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "Status": ShareStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateProvisioningPreferencesTypeDef = TypedDict(
     "UpdateProvisioningPreferencesTypeDef",
     {
         "StackSetAccounts": Sequence[str],
         "StackSetRegions": Sequence[str],
         "StackSetFailureToleranceCount": int,
         "StackSetFailureTolerancePercentage": int,
@@ -2340,33 +1950,20 @@
     "_OptionalUpdateProvisionedProductPropertiesInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class UpdateProvisionedProductPropertiesInputRequestTypeDef(
     _RequiredUpdateProvisionedProductPropertiesInputRequestTypeDef,
     _OptionalUpdateProvisionedProductPropertiesInputRequestTypeDef,
 ):
     pass
 
-
-UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
-    {
-        "ProvisionedProductId": str,
-        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
-        "RecordId": str,
-        "Status": RecordStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -2378,22 +1975,20 @@
         "Description": str,
         "Active": bool,
         "Guidance": ProvisioningArtifactGuidanceType,
     },
     total=False,
 )
 
-
 class UpdateProvisioningArtifactInputRequestTypeDef(
     _RequiredUpdateProvisioningArtifactInputRequestTypeDef,
     _OptionalUpdateProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceActionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateServiceActionInputRequestTypeDef = TypedDict(
@@ -2403,21 +1998,19 @@
         "Definition": Mapping[ServiceActionDefinitionKeyType, str],
         "Description": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class UpdateServiceActionInputRequestTypeDef(
     _RequiredUpdateServiceActionInputRequestTypeDef, _OptionalUpdateServiceActionInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTagOptionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTagOptionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateTagOptionInputRequestTypeDef = TypedDict(
@@ -2425,32 +2018,19 @@
     {
         "Value": str,
         "Active": bool,
     },
     total=False,
 )
 
-
 class UpdateTagOptionInputRequestTypeDef(
     _RequiredUpdateTagOptionInputRequestTypeDef, _OptionalUpdateTagOptionInputRequestTypeDef
 ):
     pass
 
-
-ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProvisionProductId": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisionedProductPlansInputRequestTypeDef = TypedDict(
     "ListProvisionedProductPlansInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionProductId": str,
         "PageSize": int,
         "PageToken": str,
@@ -2466,24 +2046,14 @@
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProvisionedProductsInputRequestTypeDef = TypedDict(
     "SearchProvisionedProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "Filters": Mapping[Literal["SearchQuery"], Sequence[str]],
         "SortBy": str,
@@ -2504,66 +2074,145 @@
     "_OptionalBatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef(
     _RequiredBatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     _OptionalBatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "ServiceActionAssociations": Sequence[ServiceActionAssociationTypeDef],
     },
 )
 _OptionalBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_OptionalBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef(
     _RequiredBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     _OptionalBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyProductOutputTypeDef = TypedDict(
+    "CopyProductOutputTypeDef",
+    {
+        "CopyProductToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortfolioShareOutputTypeDef = TypedDict(
+    "CreatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisionedProductPlanOutputTypeDef = TypedDict(
+    "CreateProvisionedProductPlanOutputTypeDef",
+    {
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionedProductName": str,
+        "ProvisioningArtifactId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePortfolioShareOutputTypeDef = TypedDict(
+    "DeletePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCopyProductStatusOutputTypeDef = TypedDict(
+    "DescribeCopyProductStatusOutputTypeDef",
+    {
+        "CopyProductStatus": CopyProductStatusType,
+        "TargetProductId": str,
+        "StatusDetail": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    {
+        "AccessStatus": AccessStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPortfolioAccessOutputTypeDef = TypedDict(
+    "ListPortfolioAccessOutputTypeDef",
+    {
+        "AccountIds": List[str],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePortfolioShareOutputTypeDef = TypedDict(
+    "UpdatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "Status": ShareStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
+    {
+        "ProvisionedProductId": str,
+        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
+        "RecordId": str,
+        "Status": RecordStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBudgetsForResourceOutputTypeDef = TypedDict(
     "ListBudgetsForResourceOutputTypeDef",
     {
         "Budgets": List[BudgetDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConnectionParametersTypeDef = TypedDict(
     "SourceConnectionParametersTypeDef",
     {
         "CodeStar": CodeStarParametersTypeDef,
@@ -2573,44 +2222,44 @@
 
 CreateConstraintOutputTypeDef = TypedDict(
     "CreateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConstraintOutputTypeDef = TypedDict(
     "DescribeConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConstraintsForPortfolioOutputTypeDef = TypedDict(
     "ListConstraintsForPortfolioOutputTypeDef",
     {
         "ConstraintDetails": List[ConstraintDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConstraintOutputTypeDef = TypedDict(
     "UpdateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioInputRequestTypeDef",
     {
         "DisplayName": str,
@@ -2624,21 +2273,19 @@
         "AcceptLanguage": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePortfolioInputRequestTypeDef(
     _RequiredCreatePortfolioInputRequestTypeDef, _OptionalCreatePortfolioInputRequestTypeDef
 ):
     pass
 
-
 LaunchPathSummaryTypeDef = TypedDict(
     "LaunchPathSummaryTypeDef",
     {
         "Id": str,
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "Tags": List[TagTypeDef],
         "Name": str,
@@ -2687,63 +2334,61 @@
         "ProviderName": str,
         "AddTags": Sequence[TagTypeDef],
         "RemoveTags": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdatePortfolioInputRequestTypeDef(
     _RequiredUpdatePortfolioInputRequestTypeDef, _OptionalUpdatePortfolioInputRequestTypeDef
 ):
     pass
 
-
 CreatePortfolioOutputTypeDef = TypedDict(
     "CreatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAcceptedPortfolioSharesOutputTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosForProductOutputTypeDef = TypedDict(
     "ListPortfoliosForProductOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosOutputTypeDef = TypedDict(
     "ListPortfoliosOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePortfolioOutputTypeDef = TypedDict(
     "UpdatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
@@ -2757,22 +2402,20 @@
         "OrganizationNode": OrganizationNodeTypeDef,
         "ShareTagOptions": bool,
         "SharePrincipals": bool,
     },
     total=False,
 )
 
-
 class CreatePortfolioShareInputRequestTypeDef(
     _RequiredCreatePortfolioShareInputRequestTypeDef,
     _OptionalCreatePortfolioShareInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredDeletePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalDeletePortfolioShareInputRequestTypeDef = TypedDict(
@@ -2781,28 +2424,26 @@
         "AcceptLanguage": str,
         "AccountId": str,
         "OrganizationNode": OrganizationNodeTypeDef,
     },
     total=False,
 )
 
-
 class DeletePortfolioShareInputRequestTypeDef(
     _RequiredDeletePortfolioShareInputRequestTypeDef,
     _OptionalDeletePortfolioShareInputRequestTypeDef,
 ):
     pass
 
-
 ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
     "ListOrganizationPortfolioAccessOutputTypeDef",
     {
         "OrganizationNodes": List[OrganizationNodeTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
@@ -2816,22 +2457,20 @@
         "OrganizationNode": OrganizationNodeTypeDef,
         "ShareTagOptions": bool,
         "SharePrincipals": bool,
     },
     total=False,
 )
 
-
 class UpdatePortfolioShareInputRequestTypeDef(
     _RequiredUpdatePortfolioShareInputRequestTypeDef,
     _OptionalUpdatePortfolioShareInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "Parameters": ProvisioningArtifactPropertiesTypeDef,
         "IdempotencyToken": str,
     },
@@ -2840,48 +2479,46 @@
     "_OptionalCreateProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
-
 class CreateProvisioningArtifactInputRequestTypeDef(
     _RequiredCreateProvisioningArtifactInputRequestTypeDef,
     _OptionalCreateProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
-
 CreateProvisioningArtifactOutputTypeDef = TypedDict(
     "CreateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsOutputTypeDef",
     {
         "ProvisioningArtifactDetails": List[ProvisioningArtifactDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisioningArtifactOutputTypeDef = TypedDict(
     "UpdateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanName": str,
@@ -2900,22 +2537,20 @@
         "PathId": str,
         "ProvisioningParameters": Sequence[UpdateProvisioningParameterTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateProvisionedProductPlanInputRequestTypeDef(
     _RequiredCreateProvisionedProductPlanInputRequestTypeDef,
     _OptionalCreateProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
-
 ProvisionedProductPlanDetailsTypeDef = TypedDict(
     "ProvisionedProductPlanDetailsTypeDef",
     {
         "CreatedTime": datetime,
         "PathId": str,
         "ProductId": str,
         "PlanName": str,
@@ -2934,80 +2569,80 @@
     total=False,
 )
 
 CreateTagOptionOutputTypeDef = TypedDict(
     "CreateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioOutputTypeDef = TypedDict(
     "DescribePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
         "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagOptionOutputTypeDef = TypedDict(
     "DescribeTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsOutputTypeDef = TypedDict(
     "ListTagOptionsOutputTypeDef",
     {
         "TagOptionDetails": List[TagOptionDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTagOptionOutputTypeDef = TypedDict(
     "UpdateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioSharesOutputTypeDef = TypedDict(
     "DescribePortfolioSharesOutputTypeDef",
     {
         "NextPageToken": str,
         "PortfolioShareDetails": List[PortfolioShareDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductOutputTypeDef = TypedDict(
     "DescribeProductOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "LaunchPaths": List[LaunchPathTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductViewOutputTypeDef = TypedDict(
     "DescribeProductViewOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisioningArtifactViewTypeDef = TypedDict(
     "ProvisioningArtifactViewTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -3017,33 +2652,33 @@
 )
 
 DescribeProvisionedProductOutputTypeDef = TypedDict(
     "DescribeProvisionedProductOutputTypeDef",
     {
         "ProvisionedProductDetail": ProvisionedProductDetailTypeDef,
         "CloudWatchDashboards": List[CloudWatchDashboardTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanProvisionedProductsOutputTypeDef = TypedDict(
     "ScanProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProvisionedProductOutputsOutputTypeDef = TypedDict(
     "GetProvisionedProductOutputsOutputTypeDef",
     {
         "Outputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -3057,63 +2692,295 @@
     {
         "FailureReason": str,
         "Outputs": Sequence[RecordOutputTypeDef],
     },
     total=False,
 )
 
-
 class NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
-
 DescribeServiceActionExecutionParametersOutputTypeDef = TypedDict(
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     {
         "ServiceActionParameters": List[ExecutionParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineWorkflowResourceIdentifierTypeDef = TypedDict(
     "EngineWorkflowResourceIdentifierTypeDef",
     {
         "UniqueTag": UniqueTagResourceIdentifierTypeDef,
     },
     total=False,
 )
 
+ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioShareType": PortfolioShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProductId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
+    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+):
+    pass
+
+_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
+    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "PortfolioId": str,
+        "OrganizationNodeType": OrganizationNodeTypeType,
+    },
+)
+_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
+    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+):
+    pass
+
+_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
+    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+):
+    pass
+
+ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
+    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+):
+    pass
+
+ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProvisionProductId": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "ServiceActionId": str,
+    },
+)
+_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
+    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "TagOptionId": str,
+    },
+)
+_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
+    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+):
+    pass
+
+_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "ProductId": str,
+        "ProvisioningArtifactId": str,
+    },
+)
+_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
+    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+):
+    pass
+
+ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioId": str,
+        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
+        "SortBy": ProductViewSortByType,
+        "SortOrder": SortOrderType,
+        "ProductSource": Literal["ACCOUNT"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPrincipalsForPortfolioOutputTypeDef = TypedDict(
     "ListPrincipalsForPortfolioOutputTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisionedProductPlansOutputTypeDef = TypedDict(
     "ListProvisionedProductPlansOutputTypeDef",
     {
         "ProvisionedProductPlans": List[ProvisionedProductPlanSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryInputListRecordHistoryPaginateTypeDef = TypedDict(
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "SearchFilter": ListRecordHistorySearchFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListRecordHistoryInputRequestTypeDef = TypedDict(
     "ListRecordHistoryInputRequestTypeDef",
     {
@@ -3127,33 +2994,33 @@
 )
 
 ListResourcesForTagOptionOutputTypeDef = TypedDict(
     "ListResourcesForTagOptionOutputTypeDef",
     {
         "ResourceDetails": List[ResourceDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsForProvisioningArtifactOutputTypeDef = TypedDict(
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsOutputTypeDef = TypedDict(
     "ListServiceActionsOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceActionDetailTypeDef = TypedDict(
     "ServiceActionDetailTypeDef",
     {
         "ServiceActionSummary": ServiceActionSummaryTypeDef,
@@ -3163,23 +3030,23 @@
 )
 
 ListStackInstancesForProvisionedProductOutputTypeDef = TypedDict(
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     {
         "StackInstances": List[StackInstanceTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsInputListTagOptionsPaginateTypeDef = TypedDict(
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     {
         "Filters": ListTagOptionsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTagOptionsInputRequestTypeDef = TypedDict(
     "ListTagOptionsInputRequestTypeDef",
     {
@@ -3205,15 +3072,15 @@
 
 SearchProductsOutputTypeDef = TypedDict(
     "SearchProductsOutputTypeDef",
     {
         "ProductViewSummaries": List[ProductViewSummaryTypeDef],
         "ProductViewAggregations": Dict[str, List[ProductViewAggregationValueTypeDef]],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProvisionProductInputRequestTypeDef = TypedDict(
     "_RequiredProvisionProductInputRequestTypeDef",
     {
         "ProvisionedProductName": str,
@@ -3234,21 +3101,19 @@
         "ProvisioningPreferences": ProvisioningPreferencesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "NotificationArns": Sequence[str],
     },
     total=False,
 )
 
-
 class ProvisionProductInputRequestTypeDef(
     _RequiredProvisionProductInputRequestTypeDef, _OptionalProvisionProductInputRequestTypeDef
 ):
     pass
 
-
 RecordDetailTypeDef = TypedDict(
     "RecordDetailTypeDef",
     {
         "RecordId": str,
         "ProvisionedProductName": str,
         "Status": RecordStatusType,
         "CreatedTime": datetime,
@@ -3306,22 +3171,20 @@
         "ProvisioningParameters": Sequence[UpdateProvisioningParameterTypeDef],
         "ProvisioningPreferences": UpdateProvisioningPreferencesTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateProvisionedProductInputRequestTypeDef(
     _RequiredUpdateProvisionedProductInputRequestTypeDef,
     _OptionalUpdateProvisionedProductInputRequestTypeDef,
 ):
     pass
 
-
 SourceConnectionDetailTypeDef = TypedDict(
     "SourceConnectionDetailTypeDef",
     {
         "Type": Literal["CODESTAR"],
         "ConnectionParameters": SourceConnectionParametersTypeDef,
         "LastSync": LastSyncTypeDef,
     },
@@ -3338,44 +3201,42 @@
     "_OptionalSourceConnectionTypeDef",
     {
         "Type": Literal["CODESTAR"],
     },
     total=False,
 )
 
-
 class SourceConnectionTypeDef(_RequiredSourceConnectionTypeDef, _OptionalSourceConnectionTypeDef):
     pass
 
-
 ListLaunchPathsOutputTypeDef = TypedDict(
     "ListLaunchPathsOutputTypeDef",
     {
         "LaunchPathSummaries": List[LaunchPathSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProvisionedProductsOutputTypeDef = TypedDict(
     "SearchProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductAttributeTypeDef],
         "TotalResultsCount": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsForServiceActionOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsForServiceActionOutputTypeDef",
     {
         "ProvisioningArtifactViews": List[ProvisioningArtifactViewTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -3390,135 +3251,133 @@
         "FailureReason": str,
         "ResourceIdentifier": EngineWorkflowResourceIdentifierTypeDef,
         "Outputs": Sequence[RecordOutputTypeDef],
     },
     total=False,
 )
 
-
 class NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
-
 CreateServiceActionOutputTypeDef = TypedDict(
     "CreateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceActionOutputTypeDef = TypedDict(
     "DescribeServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceActionOutputTypeDef = TypedDict(
     "UpdateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningArtifactOutputTypeDef = TypedDict(
     "DescribeProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningParametersOutputTypeDef = TypedDict(
     "DescribeProvisioningParametersOutputTypeDef",
     {
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "UsageInstructions": List[UsageInstructionTypeDef],
         "TagOptions": List[TagOptionSummaryTypeDef],
         "ProvisioningArtifactPreferences": ProvisioningArtifactPreferencesTypeDef,
         "ProvisioningArtifactOutputs": List[ProvisioningArtifactOutputTypeDef],
         "ProvisioningArtifactOutputKeys": List[ProvisioningArtifactOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecordOutputTypeDef = TypedDict(
     "DescribeRecordOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
         "RecordOutputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductPlanOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductPlanOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductServiceActionOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductServiceActionOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportAsProvisionedProductOutputTypeDef = TypedDict(
     "ImportAsProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryOutputTypeDef = TypedDict(
     "ListRecordHistoryOutputTypeDef",
     {
         "RecordDetails": List[RecordDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionProductOutputTypeDef = TypedDict(
     "ProvisionProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateProvisionedProductOutputTypeDef = TypedDict(
     "TerminateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisionedProductOutputTypeDef = TypedDict(
     "UpdateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3536,15 +3395,15 @@
     "DescribePortfolioShareStatusOutputTypeDef",
     {
         "PortfolioShareToken": str,
         "PortfolioId": str,
         "OrganizationNodeValue": str,
         "Status": ShareStatusType,
         "ShareDetails": ShareDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProductViewDetailTypeDef = TypedDict(
     "ProductViewDetailTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -3577,21 +3436,19 @@
         "Tags": Sequence[TagTypeDef],
         "ProvisioningArtifactParameters": ProvisioningArtifactPropertiesTypeDef,
         "SourceConnection": SourceConnectionTypeDef,
     },
     total=False,
 )
 
-
 class CreateProductInputRequestTypeDef(
     _RequiredCreateProductInputRequestTypeDef, _OptionalCreateProductInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateProductInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProductInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateProductInputRequestTypeDef = TypedDict(
@@ -3608,63 +3465,61 @@
         "AddTags": Sequence[TagTypeDef],
         "RemoveTags": Sequence[str],
         "SourceConnection": SourceConnectionTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProductInputRequestTypeDef(
     _RequiredUpdateProductInputRequestTypeDef, _OptionalUpdateProductInputRequestTypeDef
 ):
     pass
 
-
 DescribeProvisionedProductPlanOutputTypeDef = TypedDict(
     "DescribeProvisionedProductPlanOutputTypeDef",
     {
         "ProvisionedProductPlanDetails": ProvisionedProductPlanDetailsTypeDef,
         "ResourceChanges": List[ResourceChangeTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProductOutputTypeDef = TypedDict(
     "CreateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductAsAdminOutputTypeDef = TypedDict(
     "DescribeProductAsAdminOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactSummaries": List[ProvisioningArtifactSummaryTypeDef],
         "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProductsAsAdminOutputTypeDef = TypedDict(
     "SearchProductsAsAdminOutputTypeDef",
     {
         "ProductViewDetails": List[ProductViewDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProductOutputTypeDef = TypedDict(
     "UpdateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog/type_defs.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_servicecatalog.type_defs import AcceptPortfolioShareInputRequestTypeDef
 
-    data: AcceptPortfolioShareInputRequestTypeDef = {...}
+    data: AcceptPortfolioShareInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -53,54 +53,51 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptPortfolioShareInputRequestTypeDef",
     "AccessLevelFilterTypeDef",
     "AssociateBudgetWithResourceInputRequestTypeDef",
     "AssociatePrincipalWithPortfolioInputRequestTypeDef",
     "AssociateProductWithPortfolioInputRequestTypeDef",
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     "ServiceActionAssociationTypeDef",
     "FailedServiceActionAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "BudgetDetailTypeDef",
     "CloudWatchDashboardTypeDef",
     "CodeStarParametersTypeDef",
     "ConstraintDetailTypeDef",
     "ConstraintSummaryTypeDef",
     "CopyProductInputRequestTypeDef",
-    "CopyProductOutputTypeDef",
     "CreateConstraintInputRequestTypeDef",
     "TagTypeDef",
     "PortfolioDetailTypeDef",
     "OrganizationNodeTypeDef",
-    "CreatePortfolioShareOutputTypeDef",
     "ProvisioningArtifactPropertiesTypeDef",
     "ProvisioningArtifactDetailTypeDef",
     "UpdateProvisioningParameterTypeDef",
-    "CreateProvisionedProductPlanOutputTypeDef",
     "CreateServiceActionInputRequestTypeDef",
     "CreateTagOptionInputRequestTypeDef",
     "TagOptionDetailTypeDef",
     "DeleteConstraintInputRequestTypeDef",
     "DeletePortfolioInputRequestTypeDef",
-    "DeletePortfolioShareOutputTypeDef",
     "DeleteProductInputRequestTypeDef",
     "DeleteProvisionedProductPlanInputRequestTypeDef",
     "DeleteProvisioningArtifactInputRequestTypeDef",
     "DeleteServiceActionInputRequestTypeDef",
     "DeleteTagOptionInputRequestTypeDef",
     "DescribeConstraintInputRequestTypeDef",
     "DescribeCopyProductStatusInputRequestTypeDef",
-    "DescribeCopyProductStatusOutputTypeDef",
     "DescribePortfolioInputRequestTypeDef",
     "DescribePortfolioShareStatusInputRequestTypeDef",
     "DescribePortfolioSharesInputRequestTypeDef",
     "PortfolioShareDetailTypeDef",
     "DescribeProductAsAdminInputRequestTypeDef",
     "ProvisioningArtifactSummaryTypeDef",
     "DescribeProductInputRequestTypeDef",
@@ -127,85 +124,75 @@
     "DisassociatePrincipalFromPortfolioInputRequestTypeDef",
     "DisassociateProductFromPortfolioInputRequestTypeDef",
     "DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     "UniqueTagResourceIdentifierTypeDef",
     "ExecuteProvisionedProductPlanInputRequestTypeDef",
     "ExecuteProvisionedProductServiceActionInputRequestTypeDef",
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
     "GetProvisionedProductOutputsInputRequestTypeDef",
     "ImportAsProvisionedProductInputRequestTypeDef",
     "LastSyncTypeDef",
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     "ListBudgetsForResourceInputRequestTypeDef",
-    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
     "ListConstraintsForPortfolioInputRequestTypeDef",
-    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
     "ListLaunchPathsInputRequestTypeDef",
-    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
     "ListOrganizationPortfolioAccessInputRequestTypeDef",
     "ListPortfolioAccessInputRequestTypeDef",
-    "ListPortfolioAccessOutputTypeDef",
-    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
     "ListPortfoliosForProductInputRequestTypeDef",
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
     "ListPortfoliosInputRequestTypeDef",
-    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
     "ListPrincipalsForPortfolioInputRequestTypeDef",
     "PrincipalTypeDef",
     "ProvisionedProductPlanSummaryTypeDef",
-    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
     "ListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     "ListProvisioningArtifactsInputRequestTypeDef",
     "ListRecordHistorySearchFilterTypeDef",
-    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
     "ListResourcesForTagOptionInputRequestTypeDef",
     "ResourceDetailTypeDef",
-    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
     "ListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     "ServiceActionSummaryTypeDef",
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
     "ListServiceActionsInputRequestTypeDef",
     "ListStackInstancesForProvisionedProductInputRequestTypeDef",
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
     "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchProductsAsAdminInputRequestTypeDef",
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
     "SearchProductsInputRequestTypeDef",
     "ShareErrorTypeDef",
     "TerminateProvisionedProductInputRequestTypeDef",
     "UpdateConstraintInputRequestTypeDef",
-    "UpdatePortfolioShareOutputTypeDef",
     "UpdateProvisioningPreferencesTypeDef",
     "UpdateProvisionedProductPropertiesInputRequestTypeDef",
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "UpdateProvisioningArtifactInputRequestTypeDef",
     "UpdateServiceActionInputRequestTypeDef",
     "UpdateTagOptionInputRequestTypeDef",
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
     "ListProvisionedProductPlansInputRequestTypeDef",
     "ScanProvisionedProductsInputRequestTypeDef",
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
     "SearchProvisionedProductsInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
+    "CopyProductOutputTypeDef",
+    "CreatePortfolioShareOutputTypeDef",
+    "CreateProvisionedProductPlanOutputTypeDef",
+    "DeletePortfolioShareOutputTypeDef",
+    "DescribeCopyProductStatusOutputTypeDef",
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    "ListPortfolioAccessOutputTypeDef",
+    "UpdatePortfolioShareOutputTypeDef",
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "ListBudgetsForResourceOutputTypeDef",
     "SourceConnectionParametersTypeDef",
     "CreateConstraintOutputTypeDef",
     "DescribeConstraintOutputTypeDef",
     "ListConstraintsForPortfolioOutputTypeDef",
     "UpdateConstraintOutputTypeDef",
     "CreatePortfolioInputRequestTypeDef",
@@ -238,14 +225,28 @@
     "ProvisioningArtifactViewTypeDef",
     "DescribeProvisionedProductOutputTypeDef",
     "ScanProvisionedProductsOutputTypeDef",
     "GetProvisionedProductOutputsOutputTypeDef",
     "NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     "EngineWorkflowResourceIdentifierTypeDef",
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
     "ListPrincipalsForPortfolioOutputTypeDef",
     "ListProvisionedProductPlansOutputTypeDef",
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     "ListRecordHistoryInputRequestTypeDef",
     "ListResourcesForTagOptionOutputTypeDef",
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     "ListServiceActionsOutputTypeDef",
@@ -302,20 +303,22 @@
     {
         "AcceptLanguage": str,
         "PortfolioShareType": PortfolioShareTypeType,
     },
     total=False,
 )
 
+
 class AcceptPortfolioShareInputRequestTypeDef(
     _RequiredAcceptPortfolioShareInputRequestTypeDef,
     _OptionalAcceptPortfolioShareInputRequestTypeDef,
 ):
     pass
 
+
 AccessLevelFilterTypeDef = TypedDict(
     "AccessLevelFilterTypeDef",
     {
         "Key": AccessLevelFilterKeyType,
         "Value": str,
     },
     total=False,
@@ -341,20 +344,22 @@
     "_OptionalAssociatePrincipalWithPortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class AssociatePrincipalWithPortfolioInputRequestTypeDef(
     _RequiredAssociatePrincipalWithPortfolioInputRequestTypeDef,
     _OptionalAssociatePrincipalWithPortfolioInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredAssociateProductWithPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredAssociateProductWithPortfolioInputRequestTypeDef",
     {
         "ProductId": str,
         "PortfolioId": str,
     },
 )
@@ -363,20 +368,22 @@
     {
         "AcceptLanguage": str,
         "SourcePortfolioId": str,
     },
     total=False,
 )
 
+
 class AssociateProductWithPortfolioInputRequestTypeDef(
     _RequiredAssociateProductWithPortfolioInputRequestTypeDef,
     _OptionalAssociateProductWithPortfolioInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
         "ServiceActionId": str,
     },
@@ -385,20 +392,22 @@
     "_OptionalAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef(
     _RequiredAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     _OptionalAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 AssociateTagOptionWithResourceInputRequestTypeDef = TypedDict(
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagOptionId": str,
     },
 )
@@ -420,14 +429,25 @@
         "ProvisioningArtifactId": str,
         "ErrorCode": ServiceActionAssociationErrorCodeType,
         "ErrorMessage": str,
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
 BudgetDetailTypeDef = TypedDict(
     "BudgetDetailTypeDef",
     {
         "BudgetName": str,
     },
     total=False,
 )
@@ -487,26 +507,20 @@
         "TargetProductName": str,
         "SourceProvisioningArtifactIdentifiers": Sequence[Mapping[Literal["Id"], str]],
         "CopyOptions": Sequence[Literal["CopyTags"]],
     },
     total=False,
 )
 
+
 class CopyProductInputRequestTypeDef(
     _RequiredCopyProductInputRequestTypeDef, _OptionalCopyProductInputRequestTypeDef
 ):
     pass
 
-CopyProductOutputTypeDef = TypedDict(
-    "CopyProductOutputTypeDef",
-    {
-        "CopyProductToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateConstraintInputRequestTypeDef = TypedDict(
     "_RequiredCreateConstraintInputRequestTypeDef",
     {
         "PortfolioId": str,
         "ProductId": str,
         "Parameters": str,
@@ -519,19 +533,21 @@
     {
         "AcceptLanguage": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateConstraintInputRequestTypeDef(
     _RequiredCreateConstraintInputRequestTypeDef, _OptionalCreateConstraintInputRequestTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -554,22 +570,14 @@
     {
         "Type": OrganizationNodeTypeType,
         "Value": str,
     },
     total=False,
 )
 
-CreatePortfolioShareOutputTypeDef = TypedDict(
-    "CreatePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ProvisioningArtifactPropertiesTypeDef = TypedDict(
     "ProvisioningArtifactPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
         "Info": Mapping[str, str],
         "Type": ProvisioningArtifactTypeType,
@@ -599,26 +607,14 @@
         "Key": str,
         "Value": str,
         "UsePreviousValue": bool,
     },
     total=False,
 )
 
-CreateProvisionedProductPlanOutputTypeDef = TypedDict(
-    "CreateProvisionedProductPlanOutputTypeDef",
-    {
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionedProductName": str,
-        "ProvisioningArtifactId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceActionInputRequestTypeDef",
     {
         "Name": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
         "Definition": Mapping[ServiceActionDefinitionKeyType, str],
         "IdempotencyToken": str,
@@ -629,19 +625,21 @@
     {
         "Description": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class CreateServiceActionInputRequestTypeDef(
     _RequiredCreateServiceActionInputRequestTypeDef, _OptionalCreateServiceActionInputRequestTypeDef
 ):
     pass
 
+
 CreateTagOptionInputRequestTypeDef = TypedDict(
     "CreateTagOptionInputRequestTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -668,45 +666,41 @@
     "_OptionalDeleteConstraintInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DeleteConstraintInputRequestTypeDef(
     _RequiredDeleteConstraintInputRequestTypeDef, _OptionalDeleteConstraintInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeletePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDeletePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeletePortfolioInputRequestTypeDef = TypedDict(
     "_OptionalDeletePortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DeletePortfolioInputRequestTypeDef(
     _RequiredDeletePortfolioInputRequestTypeDef, _OptionalDeletePortfolioInputRequestTypeDef
 ):
     pass
 
-DeletePortfolioShareOutputTypeDef = TypedDict(
-    "DeletePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteProductInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProductInputRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -714,19 +708,21 @@
     "_OptionalDeleteProductInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DeleteProductInputRequestTypeDef(
     _RequiredDeleteProductInputRequestTypeDef, _OptionalDeleteProductInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanId": str,
     },
 )
 _OptionalDeleteProvisionedProductPlanInputRequestTypeDef = TypedDict(
@@ -734,20 +730,22 @@
     {
         "AcceptLanguage": str,
         "IgnoreErrors": bool,
     },
     total=False,
 )
 
+
 class DeleteProvisionedProductPlanInputRequestTypeDef(
     _RequiredDeleteProvisionedProductPlanInputRequestTypeDef,
     _OptionalDeleteProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -755,39 +753,43 @@
     "_OptionalDeleteProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DeleteProvisioningArtifactInputRequestTypeDef(
     _RequiredDeleteProvisioningArtifactInputRequestTypeDef,
     _OptionalDeleteProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredDeleteServiceActionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteServiceActionInputRequestTypeDef = TypedDict(
     "_OptionalDeleteServiceActionInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DeleteServiceActionInputRequestTypeDef(
     _RequiredDeleteServiceActionInputRequestTypeDef, _OptionalDeleteServiceActionInputRequestTypeDef
 ):
     pass
 
+
 DeleteTagOptionInputRequestTypeDef = TypedDict(
     "DeleteTagOptionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -801,48 +803,42 @@
     "_OptionalDescribeConstraintInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DescribeConstraintInputRequestTypeDef(
     _RequiredDescribeConstraintInputRequestTypeDef, _OptionalDescribeConstraintInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeCopyProductStatusInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCopyProductStatusInputRequestTypeDef",
     {
         "CopyProductToken": str,
     },
 )
 _OptionalDescribeCopyProductStatusInputRequestTypeDef = TypedDict(
     "_OptionalDescribeCopyProductStatusInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DescribeCopyProductStatusInputRequestTypeDef(
     _RequiredDescribeCopyProductStatusInputRequestTypeDef,
     _OptionalDescribeCopyProductStatusInputRequestTypeDef,
 ):
     pass
 
-DescribeCopyProductStatusOutputTypeDef = TypedDict(
-    "DescribeCopyProductStatusOutputTypeDef",
-    {
-        "CopyProductStatus": CopyProductStatusType,
-        "TargetProductId": str,
-        "StatusDetail": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDescribePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDescribePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -850,19 +846,21 @@
     "_OptionalDescribePortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DescribePortfolioInputRequestTypeDef(
     _RequiredDescribePortfolioInputRequestTypeDef, _OptionalDescribePortfolioInputRequestTypeDef
 ):
     pass
 
+
 DescribePortfolioShareStatusInputRequestTypeDef = TypedDict(
     "DescribePortfolioShareStatusInputRequestTypeDef",
     {
         "PortfolioShareToken": str,
     },
 )
 
@@ -878,20 +876,22 @@
     {
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class DescribePortfolioSharesInputRequestTypeDef(
     _RequiredDescribePortfolioSharesInputRequestTypeDef,
     _OptionalDescribePortfolioSharesInputRequestTypeDef,
 ):
     pass
 
+
 PortfolioShareDetailTypeDef = TypedDict(
     "PortfolioShareDetailTypeDef",
     {
         "PrincipalId": str,
         "Type": DescribePortfolioShareTypeType,
         "Accepted": bool,
         "ShareTagOptions": bool,
@@ -982,19 +982,21 @@
     "_OptionalDescribeProductViewInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DescribeProductViewInputRequestTypeDef(
     _RequiredDescribeProductViewInputRequestTypeDef, _OptionalDescribeProductViewInputRequestTypeDef
 ):
     pass
 
+
 DescribeProvisionedProductInputRequestTypeDef = TypedDict(
     "DescribeProvisionedProductInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "Id": str,
         "Name": str,
     },
@@ -1034,20 +1036,22 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
+
 class DescribeProvisionedProductPlanInputRequestTypeDef(
     _RequiredDescribeProvisionedProductPlanInputRequestTypeDef,
     _OptionalDescribeProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
+
 DescribeProvisioningArtifactInputRequestTypeDef = TypedDict(
     "DescribeProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisioningArtifactId": str,
         "ProductId": str,
         "ProvisioningArtifactName": str,
@@ -1120,19 +1124,21 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class DescribeRecordInputRequestTypeDef(
     _RequiredDescribeRecordInputRequestTypeDef, _OptionalDescribeRecordInputRequestTypeDef
 ):
     pass
 
+
 RecordOutputTypeDef = TypedDict(
     "RecordOutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
     },
@@ -1150,20 +1156,22 @@
     "_OptionalDescribeServiceActionExecutionParametersInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DescribeServiceActionExecutionParametersInputRequestTypeDef(
     _RequiredDescribeServiceActionExecutionParametersInputRequestTypeDef,
     _OptionalDescribeServiceActionExecutionParametersInputRequestTypeDef,
 ):
     pass
 
+
 ExecutionParameterTypeDef = TypedDict(
     "ExecutionParameterTypeDef",
     {
         "Name": str,
         "Type": str,
         "DefaultValues": List[str],
     },
@@ -1180,20 +1188,22 @@
     "_OptionalDescribeServiceActionInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DescribeServiceActionInputRequestTypeDef(
     _RequiredDescribeServiceActionInputRequestTypeDef,
     _OptionalDescribeServiceActionInputRequestTypeDef,
 ):
     pass
 
+
 DescribeTagOptionInputRequestTypeDef = TypedDict(
     "DescribeTagOptionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1217,20 +1227,22 @@
     {
         "AcceptLanguage": str,
         "PrincipalType": PrincipalTypeType,
     },
     total=False,
 )
 
+
 class DisassociatePrincipalFromPortfolioInputRequestTypeDef(
     _RequiredDisassociatePrincipalFromPortfolioInputRequestTypeDef,
     _OptionalDisassociatePrincipalFromPortfolioInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisassociateProductFromPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateProductFromPortfolioInputRequestTypeDef",
     {
         "ProductId": str,
         "PortfolioId": str,
     },
 )
@@ -1238,20 +1250,22 @@
     "_OptionalDisassociateProductFromPortfolioInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DisassociateProductFromPortfolioInputRequestTypeDef(
     _RequiredDisassociateProductFromPortfolioInputRequestTypeDef,
     _OptionalDisassociateProductFromPortfolioInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
         "ServiceActionId": str,
     },
@@ -1260,20 +1274,22 @@
     "_OptionalDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef(
     _RequiredDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     _OptionalDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 DisassociateTagOptionFromResourceInputRequestTypeDef = TypedDict(
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagOptionId": str,
     },
 )
@@ -1298,20 +1314,22 @@
     "_OptionalExecuteProvisionedProductPlanInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class ExecuteProvisionedProductPlanInputRequestTypeDef(
     _RequiredExecuteProvisionedProductPlanInputRequestTypeDef,
     _OptionalExecuteProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef",
     {
         "ProvisionedProductId": str,
         "ServiceActionId": str,
         "ExecuteToken": str,
     },
@@ -1321,27 +1339,21 @@
     {
         "AcceptLanguage": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class ExecuteProvisionedProductServiceActionInputRequestTypeDef(
     _RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef,
     _OptionalExecuteProvisionedProductServiceActionInputRequestTypeDef,
 ):
     pass
 
-GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
-    {
-        "AccessStatus": AccessStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetProvisionedProductOutputsInputRequestTypeDef = TypedDict(
     "GetProvisionedProductOutputsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionedProductId": str,
         "ProvisionedProductName": str,
@@ -1366,38 +1378,40 @@
     "_OptionalImportAsProvisionedProductInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class ImportAsProvisionedProductInputRequestTypeDef(
     _RequiredImportAsProvisionedProductInputRequestTypeDef,
     _OptionalImportAsProvisionedProductInputRequestTypeDef,
 ):
     pass
 
+
 LastSyncTypeDef = TypedDict(
     "LastSyncTypeDef",
     {
         "LastSyncTime": datetime,
         "LastSyncStatus": LastSyncStatusType,
         "LastSyncStatusMessage": str,
         "LastSuccessfulSyncTime": datetime,
         "LastSuccessfulSyncProvisioningArtifactId": str,
     },
     total=False,
 )
 
-ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AcceptLanguage": str,
-        "PortfolioShareType": PortfolioShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAcceptedPortfolioSharesInputRequestTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     {
@@ -1421,41 +1435,21 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
+
 class ListBudgetsForResourceInputRequestTypeDef(
     _RequiredListBudgetsForResourceInputRequestTypeDef,
     _OptionalListBudgetsForResourceInputRequestTypeDef,
 ):
     pass
 
-_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProductId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
-    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-):
-    pass
 
 _RequiredListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListConstraintsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
@@ -1466,40 +1460,21 @@
         "ProductId": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
+
 class ListConstraintsForPortfolioInputRequestTypeDef(
     _RequiredListConstraintsForPortfolioInputRequestTypeDef,
     _OptionalListConstraintsForPortfolioInputRequestTypeDef,
 ):
     pass
 
-_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
-    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-):
-    pass
 
 _RequiredListLaunchPathsInputRequestTypeDef = TypedDict(
     "_RequiredListLaunchPathsInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
@@ -1509,40 +1484,20 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
+
 class ListLaunchPathsInputRequestTypeDef(
     _RequiredListLaunchPathsInputRequestTypeDef, _OptionalListLaunchPathsInputRequestTypeDef
 ):
     pass
 
-_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "PortfolioId": str,
-        "OrganizationNodeType": OrganizationNodeTypeType,
-    },
-)
-_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
-    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-):
-    pass
 
 _RequiredListOrganizationPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListOrganizationPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
         "OrganizationNodeType": OrganizationNodeTypeType,
     },
@@ -1553,20 +1508,22 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListOrganizationPortfolioAccessInputRequestTypeDef(
     _RequiredListOrganizationPortfolioAccessInputRequestTypeDef,
     _OptionalListOrganizationPortfolioAccessInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPortfolioAccessInputRequestTypeDef = TypedDict(
@@ -1576,48 +1533,20 @@
         "OrganizationParentId": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListPortfolioAccessInputRequestTypeDef(
     _RequiredListPortfolioAccessInputRequestTypeDef, _OptionalListPortfolioAccessInputRequestTypeDef
 ):
     pass
 
-ListPortfolioAccessOutputTypeDef = TypedDict(
-    "ListPortfolioAccessOutputTypeDef",
-    {
-        "AccountIds": List[str],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
-    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-):
-    pass
 
 _RequiredListPortfoliosForProductInputRequestTypeDef = TypedDict(
     "_RequiredListPortfoliosForProductInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
@@ -1627,60 +1556,32 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListPortfoliosForProductInputRequestTypeDef(
     _RequiredListPortfoliosForProductInputRequestTypeDef,
     _OptionalListPortfoliosForProductInputRequestTypeDef,
 ):
     pass
 
-ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListPortfoliosInputRequestTypeDef = TypedDict(
     "ListPortfoliosInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
-    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1689,20 +1590,22 @@
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
+
 class ListPrincipalsForPortfolioInputRequestTypeDef(
     _RequiredListPrincipalsForPortfolioInputRequestTypeDef,
     _OptionalListPrincipalsForPortfolioInputRequestTypeDef,
 ):
     pass
 
+
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "PrincipalARN": str,
         "PrincipalType": PrincipalTypeType,
     },
     total=False,
@@ -1717,35 +1620,14 @@
         "ProvisionProductName": str,
         "PlanType": Literal["CLOUDFORMATION"],
         "ProvisioningArtifactId": str,
     },
     total=False,
 )
 
-_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "ServiceActionId": str,
-    },
-)
-_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
-    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-):
-    pass
-
 _RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     {
         "ServiceActionId": str,
     },
 )
 _OptionalListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
@@ -1754,70 +1636,53 @@
         "PageSize": int,
         "PageToken": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class ListProvisioningArtifactsForServiceActionInputRequestTypeDef(
     _RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     _OptionalListProvisioningArtifactsForServiceActionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListProvisioningArtifactsInputRequestTypeDef = TypedDict(
     "_RequiredListProvisioningArtifactsInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListProvisioningArtifactsInputRequestTypeDef = TypedDict(
     "_OptionalListProvisioningArtifactsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class ListProvisioningArtifactsInputRequestTypeDef(
     _RequiredListProvisioningArtifactsInputRequestTypeDef,
     _OptionalListProvisioningArtifactsInputRequestTypeDef,
 ):
     pass
 
+
 ListRecordHistorySearchFilterTypeDef = TypedDict(
     "ListRecordHistorySearchFilterTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "TagOptionId": str,
-    },
-)
-_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
-    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesForTagOptionInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesForTagOptionInputRequestTypeDef",
     {
         "TagOptionId": str,
     },
 )
 _OptionalListResourcesForTagOptionInputRequestTypeDef = TypedDict(
@@ -1826,54 +1691,34 @@
         "ResourceType": str,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
+
 class ListResourcesForTagOptionInputRequestTypeDef(
     _RequiredListResourcesForTagOptionInputRequestTypeDef,
     _OptionalListResourcesForTagOptionInputRequestTypeDef,
 ):
     pass
 
+
 ResourceDetailTypeDef = TypedDict(
     "ResourceDetailTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Name": str,
         "Description": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "ProductId": str,
-        "ProvisioningArtifactId": str,
-    },
-)
-_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
-    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-):
-    pass
-
 _RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -1883,40 +1728,33 @@
         "PageSize": int,
         "PageToken": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class ListServiceActionsForProvisioningArtifactInputRequestTypeDef(
     _RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     _OptionalListServiceActionsForProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 ServiceActionSummaryTypeDef = TypedDict(
     "ServiceActionSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
     },
     total=False,
 )
 
-ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceActionsInputRequestTypeDef = TypedDict(
     "ListServiceActionsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
@@ -1935,20 +1773,22 @@
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListStackInstancesForProvisionedProductInputRequestTypeDef(
     _RequiredListStackInstancesForProvisionedProductInputRequestTypeDef,
     _OptionalListStackInstancesForProvisionedProductInputRequestTypeDef,
 ):
     pass
 
+
 StackInstanceTypeDef = TypedDict(
     "StackInstanceTypeDef",
     {
         "Account": str,
         "Region": str,
         "StackInstanceStatus": StackInstanceStatusType,
     },
@@ -1978,29 +1818,21 @@
     "_OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     {
         "FailureReason": str,
     },
     total=False,
 )
 
+
 class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
 
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
         "AllowedPattern": str,
         "ConstraintDescription": str,
@@ -2072,41 +1904,32 @@
     {
         "AcceptLanguage": str,
         "PortfolioShareType": PortfolioShareTypeType,
     },
     total=False,
 )
 
+
 class RejectPortfolioShareInputRequestTypeDef(
     _RequiredRejectPortfolioShareInputRequestTypeDef,
     _OptionalRejectPortfolioShareInputRequestTypeDef,
 ):
     pass
 
+
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
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
 SearchProductsAsAdminInputRequestTypeDef = TypedDict(
     "SearchProductsAsAdminInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PortfolioId": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "SortBy": ProductViewSortByType,
@@ -2114,28 +1937,14 @@
         "PageToken": str,
         "PageSize": int,
         "ProductSource": Literal["ACCOUNT"],
     },
     total=False,
 )
 
-SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PortfolioId": str,
-        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
-        "SortBy": ProductViewSortByType,
-        "SortOrder": SortOrderType,
-        "ProductSource": Literal["ACCOUNT"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProductsInputRequestTypeDef = TypedDict(
     "SearchProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "PageSize": int,
         "SortBy": ProductViewSortByType,
@@ -2169,20 +1978,22 @@
         "IgnoreErrors": bool,
         "AcceptLanguage": str,
         "RetainPhysicalResources": bool,
     },
     total=False,
 )
 
+
 class TerminateProvisionedProductInputRequestTypeDef(
     _RequiredTerminateProvisionedProductInputRequestTypeDef,
     _OptionalTerminateProvisionedProductInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateConstraintInputRequestTypeDef = TypedDict(
     "_RequiredUpdateConstraintInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateConstraintInputRequestTypeDef = TypedDict(
@@ -2191,27 +2002,20 @@
         "AcceptLanguage": str,
         "Description": str,
         "Parameters": str,
     },
     total=False,
 )
 
+
 class UpdateConstraintInputRequestTypeDef(
     _RequiredUpdateConstraintInputRequestTypeDef, _OptionalUpdateConstraintInputRequestTypeDef
 ):
     pass
 
-UpdatePortfolioShareOutputTypeDef = TypedDict(
-    "UpdatePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "Status": ShareStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateProvisioningPreferencesTypeDef = TypedDict(
     "UpdateProvisioningPreferencesTypeDef",
     {
         "StackSetAccounts": Sequence[str],
         "StackSetRegions": Sequence[str],
         "StackSetFailureToleranceCount": int,
@@ -2235,30 +2039,21 @@
     "_OptionalUpdateProvisionedProductPropertiesInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class UpdateProvisionedProductPropertiesInputRequestTypeDef(
     _RequiredUpdateProvisionedProductPropertiesInputRequestTypeDef,
     _OptionalUpdateProvisionedProductPropertiesInputRequestTypeDef,
 ):
     pass
 
-UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
-    {
-        "ProvisionedProductId": str,
-        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
-        "RecordId": str,
-        "Status": RecordStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
@@ -2271,20 +2066,22 @@
         "Description": str,
         "Active": bool,
         "Guidance": ProvisioningArtifactGuidanceType,
     },
     total=False,
 )
 
+
 class UpdateProvisioningArtifactInputRequestTypeDef(
     _RequiredUpdateProvisioningArtifactInputRequestTypeDef,
     _OptionalUpdateProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceActionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateServiceActionInputRequestTypeDef = TypedDict(
@@ -2294,19 +2091,21 @@
         "Definition": Mapping[ServiceActionDefinitionKeyType, str],
         "Description": str,
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class UpdateServiceActionInputRequestTypeDef(
     _RequiredUpdateServiceActionInputRequestTypeDef, _OptionalUpdateServiceActionInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTagOptionInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTagOptionInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateTagOptionInputRequestTypeDef = TypedDict(
@@ -2314,29 +2113,20 @@
     {
         "Value": str,
         "Active": bool,
     },
     total=False,
 )
 
+
 class UpdateTagOptionInputRequestTypeDef(
     _RequiredUpdateTagOptionInputRequestTypeDef, _OptionalUpdateTagOptionInputRequestTypeDef
 ):
     pass
 
-ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProvisionProductId": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListProvisionedProductPlansInputRequestTypeDef = TypedDict(
     "ListProvisionedProductPlansInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionProductId": str,
         "PageSize": int,
@@ -2353,24 +2143,14 @@
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProvisionedProductsInputRequestTypeDef = TypedDict(
     "SearchProvisionedProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "Filters": Mapping[Literal["SearchQuery"], Sequence[str]],
         "SortBy": str,
@@ -2391,62 +2171,149 @@
     "_OptionalBatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef(
     _RequiredBatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     _OptionalBatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "ServiceActionAssociations": Sequence[ServiceActionAssociationTypeDef],
     },
 )
 _OptionalBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_OptionalBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef(
     _RequiredBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     _OptionalBatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyProductOutputTypeDef = TypedDict(
+    "CopyProductOutputTypeDef",
+    {
+        "CopyProductToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortfolioShareOutputTypeDef = TypedDict(
+    "CreatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisionedProductPlanOutputTypeDef = TypedDict(
+    "CreateProvisionedProductPlanOutputTypeDef",
+    {
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionedProductName": str,
+        "ProvisioningArtifactId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePortfolioShareOutputTypeDef = TypedDict(
+    "DeletePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCopyProductStatusOutputTypeDef = TypedDict(
+    "DescribeCopyProductStatusOutputTypeDef",
+    {
+        "CopyProductStatus": CopyProductStatusType,
+        "TargetProductId": str,
+        "StatusDetail": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    {
+        "AccessStatus": AccessStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPortfolioAccessOutputTypeDef = TypedDict(
+    "ListPortfolioAccessOutputTypeDef",
+    {
+        "AccountIds": List[str],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePortfolioShareOutputTypeDef = TypedDict(
+    "UpdatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "Status": ShareStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
+    {
+        "ProvisionedProductId": str,
+        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
+        "RecordId": str,
+        "Status": RecordStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBudgetsForResourceOutputTypeDef = TypedDict(
     "ListBudgetsForResourceOutputTypeDef",
     {
         "Budgets": List[BudgetDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceConnectionParametersTypeDef = TypedDict(
     "SourceConnectionParametersTypeDef",
     {
         "CodeStar": CodeStarParametersTypeDef,
@@ -2456,44 +2323,44 @@
 
 CreateConstraintOutputTypeDef = TypedDict(
     "CreateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConstraintOutputTypeDef = TypedDict(
     "DescribeConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConstraintsForPortfolioOutputTypeDef = TypedDict(
     "ListConstraintsForPortfolioOutputTypeDef",
     {
         "ConstraintDetails": List[ConstraintDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConstraintOutputTypeDef = TypedDict(
     "UpdateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioInputRequestTypeDef",
     {
         "DisplayName": str,
@@ -2507,19 +2374,21 @@
         "AcceptLanguage": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePortfolioInputRequestTypeDef(
     _RequiredCreatePortfolioInputRequestTypeDef, _OptionalCreatePortfolioInputRequestTypeDef
 ):
     pass
 
+
 LaunchPathSummaryTypeDef = TypedDict(
     "LaunchPathSummaryTypeDef",
     {
         "Id": str,
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "Tags": List[TagTypeDef],
         "Name": str,
@@ -2568,61 +2437,63 @@
         "ProviderName": str,
         "AddTags": Sequence[TagTypeDef],
         "RemoveTags": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdatePortfolioInputRequestTypeDef(
     _RequiredUpdatePortfolioInputRequestTypeDef, _OptionalUpdatePortfolioInputRequestTypeDef
 ):
     pass
 
+
 CreatePortfolioOutputTypeDef = TypedDict(
     "CreatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAcceptedPortfolioSharesOutputTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosForProductOutputTypeDef = TypedDict(
     "ListPortfoliosForProductOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosOutputTypeDef = TypedDict(
     "ListPortfoliosOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePortfolioOutputTypeDef = TypedDict(
     "UpdatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
@@ -2636,20 +2507,22 @@
         "OrganizationNode": OrganizationNodeTypeDef,
         "ShareTagOptions": bool,
         "SharePrincipals": bool,
     },
     total=False,
 )
 
+
 class CreatePortfolioShareInputRequestTypeDef(
     _RequiredCreatePortfolioShareInputRequestTypeDef,
     _OptionalCreatePortfolioShareInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredDeletePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalDeletePortfolioShareInputRequestTypeDef = TypedDict(
@@ -2658,26 +2531,28 @@
         "AcceptLanguage": str,
         "AccountId": str,
         "OrganizationNode": OrganizationNodeTypeDef,
     },
     total=False,
 )
 
+
 class DeletePortfolioShareInputRequestTypeDef(
     _RequiredDeletePortfolioShareInputRequestTypeDef,
     _OptionalDeletePortfolioShareInputRequestTypeDef,
 ):
     pass
 
+
 ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
     "ListOrganizationPortfolioAccessOutputTypeDef",
     {
         "OrganizationNodes": List[OrganizationNodeTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
@@ -2691,20 +2566,22 @@
         "OrganizationNode": OrganizationNodeTypeDef,
         "ShareTagOptions": bool,
         "SharePrincipals": bool,
     },
     total=False,
 )
 
+
 class UpdatePortfolioShareInputRequestTypeDef(
     _RequiredUpdatePortfolioShareInputRequestTypeDef,
     _OptionalUpdatePortfolioShareInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "Parameters": ProvisioningArtifactPropertiesTypeDef,
         "IdempotencyToken": str,
     },
@@ -2713,46 +2590,48 @@
     "_OptionalCreateProvisioningArtifactInputRequestTypeDef",
     {
         "AcceptLanguage": str,
     },
     total=False,
 )
 
+
 class CreateProvisioningArtifactInputRequestTypeDef(
     _RequiredCreateProvisioningArtifactInputRequestTypeDef,
     _OptionalCreateProvisioningArtifactInputRequestTypeDef,
 ):
     pass
 
+
 CreateProvisioningArtifactOutputTypeDef = TypedDict(
     "CreateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsOutputTypeDef",
     {
         "ProvisioningArtifactDetails": List[ProvisioningArtifactDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisioningArtifactOutputTypeDef = TypedDict(
     "UpdateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanName": str,
@@ -2771,20 +2650,22 @@
         "PathId": str,
         "ProvisioningParameters": Sequence[UpdateProvisioningParameterTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateProvisionedProductPlanInputRequestTypeDef(
     _RequiredCreateProvisionedProductPlanInputRequestTypeDef,
     _OptionalCreateProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
+
 ProvisionedProductPlanDetailsTypeDef = TypedDict(
     "ProvisionedProductPlanDetailsTypeDef",
     {
         "CreatedTime": datetime,
         "PathId": str,
         "ProductId": str,
         "PlanName": str,
@@ -2803,80 +2684,80 @@
     total=False,
 )
 
 CreateTagOptionOutputTypeDef = TypedDict(
     "CreateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioOutputTypeDef = TypedDict(
     "DescribePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
         "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagOptionOutputTypeDef = TypedDict(
     "DescribeTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsOutputTypeDef = TypedDict(
     "ListTagOptionsOutputTypeDef",
     {
         "TagOptionDetails": List[TagOptionDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTagOptionOutputTypeDef = TypedDict(
     "UpdateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioSharesOutputTypeDef = TypedDict(
     "DescribePortfolioSharesOutputTypeDef",
     {
         "NextPageToken": str,
         "PortfolioShareDetails": List[PortfolioShareDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductOutputTypeDef = TypedDict(
     "DescribeProductOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "LaunchPaths": List[LaunchPathTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductViewOutputTypeDef = TypedDict(
     "DescribeProductViewOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisioningArtifactViewTypeDef = TypedDict(
     "ProvisioningArtifactViewTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -2886,33 +2767,33 @@
 )
 
 DescribeProvisionedProductOutputTypeDef = TypedDict(
     "DescribeProvisionedProductOutputTypeDef",
     {
         "ProvisionedProductDetail": ProvisionedProductDetailTypeDef,
         "CloudWatchDashboards": List[CloudWatchDashboardTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanProvisionedProductsOutputTypeDef = TypedDict(
     "ScanProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProvisionedProductOutputsOutputTypeDef = TypedDict(
     "GetProvisionedProductOutputsOutputTypeDef",
     {
         "Outputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -2926,61 +2807,313 @@
     {
         "FailureReason": str,
         "Outputs": Sequence[RecordOutputTypeDef],
     },
     total=False,
 )
 
+
 class NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
+
 DescribeServiceActionExecutionParametersOutputTypeDef = TypedDict(
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     {
         "ServiceActionParameters": List[ExecutionParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineWorkflowResourceIdentifierTypeDef = TypedDict(
     "EngineWorkflowResourceIdentifierTypeDef",
     {
         "UniqueTag": UniqueTagResourceIdentifierTypeDef,
     },
     total=False,
 )
 
+ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioShareType": PortfolioShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProductId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
+    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
+    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "PortfolioId": str,
+        "OrganizationNodeType": OrganizationNodeTypeType,
+    },
+)
+_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
+    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
+    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+):
+    pass
+
+
+ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
+    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+):
+    pass
+
+
+ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProvisionProductId": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "ServiceActionId": str,
+    },
+)
+_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
+    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "TagOptionId": str,
+    },
+)
+_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
+    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "ProductId": str,
+        "ProvisioningArtifactId": str,
+    },
+)
+_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
+    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+):
+    pass
+
+
+ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioId": str,
+        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
+        "SortBy": ProductViewSortByType,
+        "SortOrder": SortOrderType,
+        "ProductSource": Literal["ACCOUNT"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPrincipalsForPortfolioOutputTypeDef = TypedDict(
     "ListPrincipalsForPortfolioOutputTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisionedProductPlansOutputTypeDef = TypedDict(
     "ListProvisionedProductPlansOutputTypeDef",
     {
         "ProvisionedProductPlans": List[ProvisionedProductPlanSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryInputListRecordHistoryPaginateTypeDef = TypedDict(
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "SearchFilter": ListRecordHistorySearchFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListRecordHistoryInputRequestTypeDef = TypedDict(
     "ListRecordHistoryInputRequestTypeDef",
     {
@@ -2994,33 +3127,33 @@
 )
 
 ListResourcesForTagOptionOutputTypeDef = TypedDict(
     "ListResourcesForTagOptionOutputTypeDef",
     {
         "ResourceDetails": List[ResourceDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsForProvisioningArtifactOutputTypeDef = TypedDict(
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsOutputTypeDef = TypedDict(
     "ListServiceActionsOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceActionDetailTypeDef = TypedDict(
     "ServiceActionDetailTypeDef",
     {
         "ServiceActionSummary": ServiceActionSummaryTypeDef,
@@ -3030,23 +3163,23 @@
 )
 
 ListStackInstancesForProvisionedProductOutputTypeDef = TypedDict(
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     {
         "StackInstances": List[StackInstanceTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsInputListTagOptionsPaginateTypeDef = TypedDict(
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     {
         "Filters": ListTagOptionsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTagOptionsInputRequestTypeDef = TypedDict(
     "ListTagOptionsInputRequestTypeDef",
     {
@@ -3072,15 +3205,15 @@
 
 SearchProductsOutputTypeDef = TypedDict(
     "SearchProductsOutputTypeDef",
     {
         "ProductViewSummaries": List[ProductViewSummaryTypeDef],
         "ProductViewAggregations": Dict[str, List[ProductViewAggregationValueTypeDef]],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProvisionProductInputRequestTypeDef = TypedDict(
     "_RequiredProvisionProductInputRequestTypeDef",
     {
         "ProvisionedProductName": str,
@@ -3101,19 +3234,21 @@
         "ProvisioningPreferences": ProvisioningPreferencesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "NotificationArns": Sequence[str],
     },
     total=False,
 )
 
+
 class ProvisionProductInputRequestTypeDef(
     _RequiredProvisionProductInputRequestTypeDef, _OptionalProvisionProductInputRequestTypeDef
 ):
     pass
 
+
 RecordDetailTypeDef = TypedDict(
     "RecordDetailTypeDef",
     {
         "RecordId": str,
         "ProvisionedProductName": str,
         "Status": RecordStatusType,
         "CreatedTime": datetime,
@@ -3171,20 +3306,22 @@
         "ProvisioningParameters": Sequence[UpdateProvisioningParameterTypeDef],
         "ProvisioningPreferences": UpdateProvisioningPreferencesTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateProvisionedProductInputRequestTypeDef(
     _RequiredUpdateProvisionedProductInputRequestTypeDef,
     _OptionalUpdateProvisionedProductInputRequestTypeDef,
 ):
     pass
 
+
 SourceConnectionDetailTypeDef = TypedDict(
     "SourceConnectionDetailTypeDef",
     {
         "Type": Literal["CODESTAR"],
         "ConnectionParameters": SourceConnectionParametersTypeDef,
         "LastSync": LastSyncTypeDef,
     },
@@ -3201,42 +3338,44 @@
     "_OptionalSourceConnectionTypeDef",
     {
         "Type": Literal["CODESTAR"],
     },
     total=False,
 )
 
+
 class SourceConnectionTypeDef(_RequiredSourceConnectionTypeDef, _OptionalSourceConnectionTypeDef):
     pass
 
+
 ListLaunchPathsOutputTypeDef = TypedDict(
     "ListLaunchPathsOutputTypeDef",
     {
         "LaunchPathSummaries": List[LaunchPathSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProvisionedProductsOutputTypeDef = TypedDict(
     "SearchProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductAttributeTypeDef],
         "TotalResultsCount": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsForServiceActionOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsForServiceActionOutputTypeDef",
     {
         "ProvisioningArtifactViews": List[ProvisioningArtifactViewTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -3251,133 +3390,135 @@
         "FailureReason": str,
         "ResourceIdentifier": EngineWorkflowResourceIdentifierTypeDef,
         "Outputs": Sequence[RecordOutputTypeDef],
     },
     total=False,
 )
 
+
 class NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
+
 CreateServiceActionOutputTypeDef = TypedDict(
     "CreateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceActionOutputTypeDef = TypedDict(
     "DescribeServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceActionOutputTypeDef = TypedDict(
     "UpdateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningArtifactOutputTypeDef = TypedDict(
     "DescribeProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningParametersOutputTypeDef = TypedDict(
     "DescribeProvisioningParametersOutputTypeDef",
     {
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "UsageInstructions": List[UsageInstructionTypeDef],
         "TagOptions": List[TagOptionSummaryTypeDef],
         "ProvisioningArtifactPreferences": ProvisioningArtifactPreferencesTypeDef,
         "ProvisioningArtifactOutputs": List[ProvisioningArtifactOutputTypeDef],
         "ProvisioningArtifactOutputKeys": List[ProvisioningArtifactOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecordOutputTypeDef = TypedDict(
     "DescribeRecordOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
         "RecordOutputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductPlanOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductPlanOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductServiceActionOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductServiceActionOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportAsProvisionedProductOutputTypeDef = TypedDict(
     "ImportAsProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryOutputTypeDef = TypedDict(
     "ListRecordHistoryOutputTypeDef",
     {
         "RecordDetails": List[RecordDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionProductOutputTypeDef = TypedDict(
     "ProvisionProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateProvisionedProductOutputTypeDef = TypedDict(
     "TerminateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisionedProductOutputTypeDef = TypedDict(
     "UpdateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3395,15 +3536,15 @@
     "DescribePortfolioShareStatusOutputTypeDef",
     {
         "PortfolioShareToken": str,
         "PortfolioId": str,
         "OrganizationNodeValue": str,
         "Status": ShareStatusType,
         "ShareDetails": ShareDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProductViewDetailTypeDef = TypedDict(
     "ProductViewDetailTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -3436,19 +3577,21 @@
         "Tags": Sequence[TagTypeDef],
         "ProvisioningArtifactParameters": ProvisioningArtifactPropertiesTypeDef,
         "SourceConnection": SourceConnectionTypeDef,
     },
     total=False,
 )
 
+
 class CreateProductInputRequestTypeDef(
     _RequiredCreateProductInputRequestTypeDef, _OptionalCreateProductInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateProductInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProductInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateProductInputRequestTypeDef = TypedDict(
@@ -3465,61 +3608,63 @@
         "AddTags": Sequence[TagTypeDef],
         "RemoveTags": Sequence[str],
         "SourceConnection": SourceConnectionTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProductInputRequestTypeDef(
     _RequiredUpdateProductInputRequestTypeDef, _OptionalUpdateProductInputRequestTypeDef
 ):
     pass
 
+
 DescribeProvisionedProductPlanOutputTypeDef = TypedDict(
     "DescribeProvisionedProductPlanOutputTypeDef",
     {
         "ProvisionedProductPlanDetails": ProvisionedProductPlanDetailsTypeDef,
         "ResourceChanges": List[ResourceChangeTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProductOutputTypeDef = TypedDict(
     "CreateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductAsAdminOutputTypeDef = TypedDict(
     "DescribeProductAsAdminOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactSummaries": List[ProvisioningArtifactSummaryTypeDef],
         "Tags": List[TagTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProductsAsAdminOutputTypeDef = TypedDict(
     "SearchProductsAsAdminOutputTypeDef",
     {
         "ProductViewDetails": List[ProductViewDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProductOutputTypeDef = TypedDict(
     "UpdateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/PKG-INFO` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServiceCatalog 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServiceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore servicecatalog type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicecatalog"></a>
 
 # types-aiobotocore-servicecatalog
 
 [![PyPI - types-aiobotocore-servicecatalog](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicecatalog?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicecatalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog)](https://pepy.tech/project/types-aiobotocore-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [types-aiobotocore-servicecatalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog/).
 
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
@@ -417,62 +416,58 @@
 )
 
 
 def check_value(value: AccessLevelFilterKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicecatalog.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_servicecatalog.type_defs import (
     AcceptPortfolioShareInputRequestTypeDef,
     AccessLevelFilterTypeDef,
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
     AssociateProductWithPortfolioInputRequestTypeDef,
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
+    ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
-    CopyProductOutputTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
     OrganizationNodeTypeDef,
-    CreatePortfolioShareOutputTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
-    CreateProvisionedProductPlanOutputTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
     DeleteConstraintInputRequestTypeDef,
     DeletePortfolioInputRequestTypeDef,
-    DeletePortfolioShareOutputTypeDef,
     DeleteProductInputRequestTypeDef,
     DeleteProvisionedProductPlanInputRequestTypeDef,
     DeleteProvisioningArtifactInputRequestTypeDef,
     DeleteServiceActionInputRequestTypeDef,
     DeleteTagOptionInputRequestTypeDef,
     DescribeConstraintInputRequestTypeDef,
     DescribeCopyProductStatusInputRequestTypeDef,
-    DescribeCopyProductStatusOutputTypeDef,
     DescribePortfolioInputRequestTypeDef,
     DescribePortfolioShareStatusInputRequestTypeDef,
     DescribePortfolioSharesInputRequestTypeDef,
     PortfolioShareDetailTypeDef,
     DescribeProductAsAdminInputRequestTypeDef,
     ProvisioningArtifactSummaryTypeDef,
     DescribeProductInputRequestTypeDef,
@@ -499,85 +494,75 @@
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
     UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
-    GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
-    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
-    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
-    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListLaunchPathsInputRequestTypeDef,
-    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
-    ListPortfolioAccessOutputTypeDef,
-    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
-    ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPortfoliosInputRequestTypeDef,
-    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
-    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     ListProvisioningArtifactsInputRequestTypeDef,
     ListRecordHistorySearchFilterTypeDef,
-    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListResourcesForTagOptionInputRequestTypeDef,
     ResourceDetailTypeDef,
-    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
-    ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
-    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
     TerminateProvisionedProductInputRequestTypeDef,
     UpdateConstraintInputRequestTypeDef,
-    UpdatePortfolioShareOutputTypeDef,
     UpdateProvisioningPreferencesTypeDef,
     UpdateProvisionedProductPropertiesInputRequestTypeDef,
-    UpdateProvisionedProductPropertiesOutputTypeDef,
     UpdateProvisioningArtifactInputRequestTypeDef,
     UpdateServiceActionInputRequestTypeDef,
     UpdateTagOptionInputRequestTypeDef,
-    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisionedProductPlansInputRequestTypeDef,
     ScanProvisionedProductsInputRequestTypeDef,
-    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProvisionedProductsInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef,
+    CopyProductOutputTypeDef,
+    CreatePortfolioShareOutputTypeDef,
+    CreateProvisionedProductPlanOutputTypeDef,
+    DeletePortfolioShareOutputTypeDef,
+    DescribeCopyProductStatusOutputTypeDef,
+    GetAWSOrganizationsAccessStatusOutputTypeDef,
+    ListPortfolioAccessOutputTypeDef,
+    UpdatePortfolioShareOutputTypeDef,
+    UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
@@ -610,14 +595,28 @@
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     EngineWorkflowResourceIdentifierTypeDef,
+    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    ListPortfoliosInputListPortfoliosPaginateTypeDef,
+    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
+    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    ListServiceActionsInputListServiceActionsPaginateTypeDef,
+    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
+    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
@@ -660,15 +659,15 @@
     CreateProductOutputTypeDef,
     DescribeProductAsAdminOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     UpdateProductOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptPortfolioShareInputRequestTypeDef:
+def get_value() -> AcceptPortfolioShareInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt` & `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*


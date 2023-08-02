# Comparing `tmp/types-aiobotocore-es-2.5.2.tar.gz` & `tmp/types-aiobotocore-es-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-es-2.5.2.tar", last modified: Sat Jul  8 01:43:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-es-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
```

## Comparing `types-aiobotocore-es-2.5.2.tar` & `types-aiobotocore-es-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.534130 types-aiobotocore-es-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-08 01:43:37.534130 types-aiobotocore-es-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:37.534130 types-aiobotocore-es-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.534130 types-aiobotocore-es-2.5.2/types_aiobotocore_es/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43173 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-08 01:30:43.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63699 2023-07-08 01:30:44.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63652 2023-07-08 01:30:43.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:42.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.534130 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-08 01:43:37.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-08 01:43:37.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:37.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:43:37.000000 types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.965588 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43183 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43119 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64435 2023-08-02 14:38:35.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64388 2023-08-02 14:38:33.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-es-2.5.2/LICENSE` & `types-aiobotocore-es-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2/PKG-INFO` & `types-aiobotocore-es-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-es
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore es type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore es type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-es"></a>
 
 # types-aiobotocore-es
 
 [![PyPI - types-aiobotocore-es](https://img.shields.io/pypi/v/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-es?color=blue)](https://pypistats.org/packages/types-aiobotocore-es)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticsearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [types-aiobotocore-es docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/).
 
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
@@ -356,33 +355,35 @@
 )
 
 
 def check_value(value: AutoTuneDesiredStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_es.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_es.type_defs import (
     AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
+    TimestampTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
     CognitoOptionsTypeDef,
@@ -408,70 +409,65 @@
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeElasticsearchDomainConfigRequestRequestTypeDef,
     DescribeElasticsearchDomainRequestRequestTypeDef,
     DescribeElasticsearchDomainsRequestRequestTypeDef,
     DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef,
     FilterTypeDef,
     DescribePackagesFilterTypeDef,
-    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef,
-    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
     DescribeReservedElasticsearchInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     DryRunResultsTypeDef,
     ZoneAwarenessConfigTypeDef,
     VPCDerivedInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleElasticsearchVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
-    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundCrossClusterSearchConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
-    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
     ListElasticsearchInstanceTypesRequestRequestTypeDef,
-    ListElasticsearchInstanceTypesResponseTypeDef,
-    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListElasticsearchVersionsRequestRequestTypeDef,
-    ListElasticsearchVersionsResponseTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpgradeElasticsearchDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListElasticsearchInstanceTypesResponseTypeDef,
+    ListElasticsearchVersionsResponseTypeDef,
+    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     ElasticsearchVersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     StartElasticsearchServiceSoftwareUpdateResponseTypeDef,
     UpgradeElasticsearchDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleElasticsearchVersionsResponseTypeDef,
@@ -490,14 +486,19 @@
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
+    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
+    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
+    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     ElasticsearchClusterConfigTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
@@ -506,14 +507,15 @@
     ReservedElasticsearchInstanceOfferingTypeDef,
     ReservedElasticsearchInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     DeleteOutboundCrossClusterSearchConnectionResponseTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
@@ -535,14 +537,15 @@
     DescribeReservedElasticsearchInstancesResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CreateElasticsearchDomainRequestRequestTypeDef,
     UpdateElasticsearchDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     ElasticsearchDomainStatusTypeDef,
     DescribeElasticsearchInstanceTypeLimitsResponseTypeDef,
     ElasticsearchDomainConfigTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
@@ -550,15 +553,15 @@
     DescribeElasticsearchDomainResponseTypeDef,
     DescribeElasticsearchDomainsResponseTypeDef,
     DescribeElasticsearchDomainConfigResponseTypeDef,
     UpdateElasticsearchDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef:
+def get_value() -> AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-es-2.5.2/README.md` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-es
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore es type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-es"></a>
 
 # types-aiobotocore-es
 
 [![PyPI - types-aiobotocore-es](https://img.shields.io/pypi/v/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-es?color=blue)](https://pypistats.org/packages/types-aiobotocore-es)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticsearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [types-aiobotocore-es docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -323,33 +355,35 @@
 )
 
 
 def check_value(value: AutoTuneDesiredStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_es.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_es.type_defs import (
     AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
+    TimestampTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
     CognitoOptionsTypeDef,
@@ -375,70 +409,65 @@
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeElasticsearchDomainConfigRequestRequestTypeDef,
     DescribeElasticsearchDomainRequestRequestTypeDef,
     DescribeElasticsearchDomainsRequestRequestTypeDef,
     DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef,
     FilterTypeDef,
     DescribePackagesFilterTypeDef,
-    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef,
-    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
     DescribeReservedElasticsearchInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     DryRunResultsTypeDef,
     ZoneAwarenessConfigTypeDef,
     VPCDerivedInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleElasticsearchVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
-    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundCrossClusterSearchConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
-    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
     ListElasticsearchInstanceTypesRequestRequestTypeDef,
-    ListElasticsearchInstanceTypesResponseTypeDef,
-    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListElasticsearchVersionsRequestRequestTypeDef,
-    ListElasticsearchVersionsResponseTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpgradeElasticsearchDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListElasticsearchInstanceTypesResponseTypeDef,
+    ListElasticsearchVersionsResponseTypeDef,
+    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     ElasticsearchVersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     StartElasticsearchServiceSoftwareUpdateResponseTypeDef,
     UpgradeElasticsearchDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleElasticsearchVersionsResponseTypeDef,
@@ -457,14 +486,19 @@
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
+    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
+    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
+    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     ElasticsearchClusterConfigTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
@@ -473,14 +507,15 @@
     ReservedElasticsearchInstanceOfferingTypeDef,
     ReservedElasticsearchInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     DeleteOutboundCrossClusterSearchConnectionResponseTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
@@ -502,14 +537,15 @@
     DescribeReservedElasticsearchInstancesResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CreateElasticsearchDomainRequestRequestTypeDef,
     UpdateElasticsearchDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     ElasticsearchDomainStatusTypeDef,
     DescribeElasticsearchInstanceTypeLimitsResponseTypeDef,
     ElasticsearchDomainConfigTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
@@ -517,15 +553,15 @@
     DescribeElasticsearchDomainResponseTypeDef,
     DescribeElasticsearchDomainsResponseTypeDef,
     DescribeElasticsearchDomainConfigResponseTypeDef,
     UpdateElasticsearchDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef:
+def get_value() -> AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-es-2.5.2/setup.py` & `types-aiobotocore-es-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-es",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_es"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with"
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
-    keywords="aiobotocore es type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore es type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_es": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/__init__.py` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/__init__.pyi` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/__main__.py` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticsearchService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService\nOther"
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

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/client.py` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from .type_defs import (
     AcceptInboundCrossClusterSearchConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     CognitoOptionsTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
     CreateOutboundCrossClusterSearchConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteElasticsearchDomainResponseTypeDef,
@@ -707,15 +707,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...
     ) -> UpdateElasticsearchDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Elasticsearch domain,
         setting as setting the instance type and the number of instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_elasticsearch_domain_config)
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/client.pyi` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from .type_defs import (
     AcceptInboundCrossClusterSearchConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     CognitoOptionsTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
     CreateOutboundCrossClusterSearchConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteElasticsearchDomainResponseTypeDef,
@@ -653,15 +653,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...
     ) -> UpdateElasticsearchDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Elasticsearch domain,
         setting as setting the instance type and the number of instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_elasticsearch_domain_config)
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/literals.py` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/literals.pyi` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/paginator.py` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
         """
 
 
@@ -85,30 +85,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
         """
 
 
 class GetUpgradeHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#getupgradehistorypaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetUpgradeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#getupgradehistorypaginator)
         """
 
 
@@ -119,28 +119,28 @@
     """
 
     def paginate(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListElasticsearchInstanceTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchinstancetypespaginator)
         """
 
 
 class ListElasticsearchVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListElasticsearchVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchversionspaginator)
         """
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/paginator.pyi` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceOfferingId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstanceofferingspaginator)
         """
 
 class DescribeReservedElasticsearchInstancesPaginator(AioPaginator):
@@ -81,29 +81,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         ReservedElasticsearchInstanceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#describereservedelasticsearchinstancespaginator)
         """
 
 class GetUpgradeHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#getupgradehistorypaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetUpgradeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#getupgradehistorypaginator)
         """
 
 class ListElasticsearchInstanceTypesPaginator(AioPaginator):
@@ -113,27 +113,27 @@
     """
 
     def paginate(
         self,
         *,
         ElasticsearchVersion: str,
         DomainName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListElasticsearchInstanceTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchinstancetypespaginator)
         """
 
 class ListElasticsearchVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchversionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListElasticsearchVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/paginators/#listelasticsearchversionspaginator)
         """
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/type_defs.py` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_es.type_defs import AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef
 
-    data: AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = {...}
+    data: AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -51,23 +51,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
     "DurationTypeDef",
+    "TimestampTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
     "CognitoOptionsTypeDef",
@@ -93,70 +95,65 @@
     "DescribeDomainChangeProgressRequestRequestTypeDef",
     "DescribeElasticsearchDomainConfigRequestRequestTypeDef",
     "DescribeElasticsearchDomainRequestRequestTypeDef",
     "DescribeElasticsearchDomainsRequestRequestTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef",
     "FilterTypeDef",
     "DescribePackagesFilterTypeDef",
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "DryRunResultsTypeDef",
     "ZoneAwarenessConfigTypeDef",
     "VPCDerivedInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
-    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
-    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
     "ListElasticsearchInstanceTypesRequestRequestTypeDef",
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListElasticsearchVersionsRequestRequestTypeDef",
-    "ListElasticsearchVersionsResponseTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpgradeElasticsearchDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    "ListElasticsearchVersionsResponseTypeDef",
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "ElasticsearchVersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "UpgradeElasticsearchDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
@@ -175,14 +172,19 @@
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
+    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
     "ElasticsearchClusterConfigTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
@@ -191,14 +193,15 @@
     "ReservedElasticsearchInstanceOfferingTypeDef",
     "ReservedElasticsearchInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
@@ -220,14 +223,15 @@
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "CreateElasticsearchDomainRequestRequestTypeDef",
     "UpdateElasticsearchDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "ElasticsearchDomainStatusTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     "ElasticsearchDomainConfigTypeDef",
     "CreateElasticsearchDomainResponseTypeDef",
@@ -241,14 +245,25 @@
 AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     {
         "CrossClusterSearchConnectionId": str,
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -335,14 +350,15 @@
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 AutoTuneOptionsOutputTypeDef = TypedDict(
     "AutoTuneOptionsOutputTypeDef",
     {
         "State": AutoTuneStateType,
         "ErrorMessage": str,
     },
     total=False,
@@ -696,42 +712,34 @@
     {
         "Name": DescribePackagesFilterNameType,
         "Value": Sequence[str],
     },
     total=False,
 )
 
-DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ReservedElasticsearchInstanceOfferingId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedElasticsearchInstancesRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -805,21 +813,14 @@
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCompatibleElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -853,36 +854,14 @@
         "PackageVersion": str,
         "CommitMessage": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
-_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
-    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetUpgradeHistoryRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
@@ -904,24 +883,14 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InboundCrossClusterSearchConnectionStatusTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     {
         "StatusCode": InboundCrossClusterSearchConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -963,37 +932,14 @@
 class ListDomainsForPackageRequestRequestTypeDef(
     _RequiredListDomainsForPackageRequestRequestTypeDef,
     _OptionalListDomainsForPackageRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "ElasticsearchVersion": str,
-    },
-)
-_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "DomainName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
-    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListElasticsearchInstanceTypesRequestRequestTypeDef",
     {
         "ElasticsearchVersion": str,
     },
 )
 _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
@@ -1010,49 +956,23 @@
 class ListElasticsearchInstanceTypesRequestRequestTypeDef(
     _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef,
     _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef,
 ):
     pass
 
 
-ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    {
-        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "ListElasticsearchVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListElasticsearchVersionsResponseTypeDef = TypedDict(
-    "ListElasticsearchVersionsResponseTypeDef",
-    {
-        "ElasticsearchVersions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListPackagesForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListPackagesForDomainRequestRequestTypeDef = TypedDict(
@@ -1127,24 +1047,14 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
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
 _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "ReservationName": str,
     },
 )
@@ -1160,23 +1070,14 @@
 class PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
 
-PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1193,25 +1094,14 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
@@ -1270,14 +1160,58 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    {
+        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListElasticsearchVersionsResponseTypeDef = TypedDict(
+    "ListElasticsearchVersionsResponseTypeDef",
+    {
+        "ElasticsearchVersions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1306,77 +1240,87 @@
     },
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
+    {
+        "StartAt": datetime,
+        "Duration": DurationTypeDef,
+        "CronExpressionForRecurrence": str,
+    },
+    total=False,
+)
+
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
-        "StartAt": Union[datetime, str],
+        "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
 CancelElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpgradeElasticsearchDomainResponseTypeDef = TypedDict(
     "UpgradeElasticsearchDomainResponseTypeDef",
     {
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1398,15 +1342,15 @@
     },
 )
 
 GetCompatibleElasticsearchVersionsResponseTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
     {
         "CompatibleElasticsearchVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
         "Options": DomainEndpointOptionsTypeDef,
@@ -1498,15 +1442,15 @@
     "CreateOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
         "DestinationDomainInfo": DomainInformationTypeDef,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundCrossClusterSearchConnectionStatusTypeDef,
         "CrossClusterSearchConnectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OutboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "OutboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1564,33 +1508,33 @@
     pass
 
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1616,19 +1560,90 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+    {
+        "ReservedElasticsearchInstanceOfferingId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
+    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "ElasticsearchVersion": str,
+    },
+)
+_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "DomainName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
+    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+):
+    pass
+
+
+ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1701,15 +1716,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1815,122 +1830,132 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsExtraOutputTypeDef = TypedDict(
+    "AutoTuneOptionsExtraOutputTypeDef",
+    {
+        "DesiredState": AutoTuneDesiredStateType,
+        "RollbackOnDisable": RollbackOnDisableType,
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
+    },
+    total=False,
+)
+
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteOutboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": OutboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[OutboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ElasticsearchClusterConfigStatusTypeDef = TypedDict(
     "ElasticsearchClusterConfigStatusTypeDef",
     {
         "Options": ElasticsearchClusterConfigTypeDef,
@@ -1938,85 +1963,85 @@
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[InboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "RejectInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstanceOfferings": List[
             ReservedElasticsearchInstanceOfferingTypeDef
         ],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedElasticsearchInstancesResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstances": List[ReservedElasticsearchInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2051,36 +2076,37 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsTypeDef,
+        "Options": AutoTuneOptionsExtraOutputTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 _RequiredCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateElasticsearchDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
@@ -2200,15 +2226,15 @@
     pass
 
 
 DescribeElasticsearchInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ElasticsearchDomainConfigTypeDef = TypedDict(
     "ElasticsearchDomainConfigTypeDef",
     {
         "ElasticsearchVersion": ElasticsearchVersionStatusTypeDef,
@@ -2230,51 +2256,51 @@
     total=False,
 )
 
 CreateElasticsearchDomainResponseTypeDef = TypedDict(
     "CreateElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteElasticsearchDomainResponseTypeDef = TypedDict(
     "DeleteElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticsearchDomainResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticsearchDomainsResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainsResponseTypeDef",
     {
         "DomainStatusList": List[ElasticsearchDomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "UpdateElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es/type_defs.pyi` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_es.type_defs import AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef
 
-    data: AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = {...}
+    data: AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -50,23 +50,25 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
     "DurationTypeDef",
+    "TimestampTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
     "CognitoOptionsTypeDef",
@@ -92,70 +94,65 @@
     "DescribeDomainChangeProgressRequestRequestTypeDef",
     "DescribeElasticsearchDomainConfigRequestRequestTypeDef",
     "DescribeElasticsearchDomainRequestRequestTypeDef",
     "DescribeElasticsearchDomainsRequestRequestTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef",
     "FilterTypeDef",
     "DescribePackagesFilterTypeDef",
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "DryRunResultsTypeDef",
     "ZoneAwarenessConfigTypeDef",
     "VPCDerivedInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
-    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
-    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
     "ListElasticsearchInstanceTypesRequestRequestTypeDef",
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListElasticsearchVersionsRequestRequestTypeDef",
-    "ListElasticsearchVersionsResponseTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpgradeElasticsearchDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    "ListElasticsearchVersionsResponseTypeDef",
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "ElasticsearchVersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "UpgradeElasticsearchDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
@@ -174,14 +171,19 @@
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
+    "GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    "ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
     "ElasticsearchClusterConfigTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
@@ -190,14 +192,15 @@
     "ReservedElasticsearchInstanceOfferingTypeDef",
     "ReservedElasticsearchInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
@@ -219,14 +222,15 @@
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "CreateElasticsearchDomainRequestRequestTypeDef",
     "UpdateElasticsearchDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "ElasticsearchDomainStatusTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     "ElasticsearchDomainConfigTypeDef",
     "CreateElasticsearchDomainResponseTypeDef",
@@ -240,14 +244,25 @@
 AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef",
     {
         "CrossClusterSearchConnectionId": str,
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
 _RequiredOptionStatusTypeDef = TypedDict(
     "_RequiredOptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
         "State": OptionStateType,
     },
@@ -332,14 +347,15 @@
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 AutoTuneOptionsOutputTypeDef = TypedDict(
     "AutoTuneOptionsOutputTypeDef",
     {
         "State": AutoTuneStateType,
         "ErrorMessage": str,
     },
     total=False,
@@ -683,42 +699,34 @@
     {
         "Name": DescribePackagesFilterNameType,
         "Value": Sequence[str],
     },
     total=False,
 )
 
-DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ReservedElasticsearchInstanceOfferingId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
-    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedElasticsearchInstancesRequestRequestTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -792,21 +800,14 @@
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCompatibleElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -838,34 +839,14 @@
         "PackageVersion": str,
         "CommitMessage": str,
         "CreatedAt": datetime,
     },
     total=False,
 )
 
-_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
-    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetUpgradeHistoryRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetUpgradeHistoryRequestRequestTypeDef = TypedDict(
@@ -885,24 +866,14 @@
 GetUpgradeStatusRequestRequestTypeDef = TypedDict(
     "GetUpgradeStatusRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetUpgradeStatusResponseTypeDef = TypedDict(
-    "GetUpgradeStatusResponseTypeDef",
-    {
-        "UpgradeStep": UpgradeStepType,
-        "StepStatus": UpgradeStatusType,
-        "UpgradeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InboundCrossClusterSearchConnectionStatusTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionStatusTypeDef",
     {
         "StatusCode": InboundCrossClusterSearchConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -942,35 +913,14 @@
 
 class ListDomainsForPackageRequestRequestTypeDef(
     _RequiredListDomainsForPackageRequestRequestTypeDef,
     _OptionalListDomainsForPackageRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "ElasticsearchVersion": str,
-    },
-)
-_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
-    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
-    {
-        "DomainName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
-    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListElasticsearchInstanceTypesRequestRequestTypeDef",
     {
         "ElasticsearchVersion": str,
     },
 )
 _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef = TypedDict(
@@ -985,49 +935,23 @@
 
 class ListElasticsearchInstanceTypesRequestRequestTypeDef(
     _RequiredListElasticsearchInstanceTypesRequestRequestTypeDef,
     _OptionalListElasticsearchInstanceTypesRequestRequestTypeDef,
 ):
     pass
 
-ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
-    "ListElasticsearchInstanceTypesResponseTypeDef",
-    {
-        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
-    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListElasticsearchVersionsRequestRequestTypeDef = TypedDict(
     "ListElasticsearchVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListElasticsearchVersionsResponseTypeDef = TypedDict(
-    "ListElasticsearchVersionsResponseTypeDef",
-    {
-        "ElasticsearchVersions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListPackagesForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredListPackagesForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListPackagesForDomainRequestRequestTypeDef = TypedDict(
@@ -1096,24 +1020,14 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
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
 _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef",
     {
         "ReservedElasticsearchInstanceOfferingId": str,
         "ReservationName": str,
     },
 )
@@ -1127,23 +1041,14 @@
 
 class PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
-PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
-    {
-        "ReservedElasticsearchInstanceId": str,
-        "ReservationName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "RecurringChargeAmount": float,
         "RecurringChargeFrequency": str,
     },
     total=False,
@@ -1160,25 +1065,14 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagKeys": Sequence[str],
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
 RevokeVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
@@ -1235,14 +1129,58 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUpgradeStatusResponseTypeDef = TypedDict(
+    "GetUpgradeStatusResponseTypeDef",
+    {
+        "UpgradeStep": UpgradeStepType,
+        "StepStatus": UpgradeStatusType,
+        "UpgradeName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListElasticsearchInstanceTypesResponseTypeDef = TypedDict(
+    "ListElasticsearchInstanceTypesResponseTypeDef",
+    {
+        "ElasticsearchInstanceTypes": List[ESPartitionInstanceTypeType],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListElasticsearchVersionsResponseTypeDef = TypedDict(
+    "ListElasticsearchVersionsResponseTypeDef",
+    {
+        "ElasticsearchVersions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "ReservationName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AccessPoliciesStatusTypeDef = TypedDict(
     "AccessPoliciesStatusTypeDef",
     {
         "Options": str,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -1271,77 +1209,87 @@
     },
 )
 
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointAccessResponseTypeDef = TypedDict(
     "ListVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipalList": List[AuthorizedPrincipalTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
+    {
+        "StartAt": datetime,
+        "Duration": DurationTypeDef,
+        "CronExpressionForRecurrence": str,
+    },
+    total=False,
+)
+
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
-        "StartAt": Union[datetime, str],
+        "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
 CancelElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartElasticsearchServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpgradeElasticsearchDomainResponseTypeDef = TypedDict(
     "UpgradeElasticsearchDomainResponseTypeDef",
     {
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1363,15 +1311,15 @@
     },
 )
 
 GetCompatibleElasticsearchVersionsResponseTypeDef = TypedDict(
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
     {
         "CompatibleElasticsearchVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
         "Options": DomainEndpointOptionsTypeDef,
@@ -1461,15 +1409,15 @@
     "CreateOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
         "DestinationDomainInfo": DomainInformationTypeDef,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundCrossClusterSearchConnectionStatusTypeDef,
         "CrossClusterSearchConnectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OutboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "OutboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1523,33 +1471,33 @@
 ):
     pass
 
 DeleteVpcEndpointResponseTypeDef = TypedDict(
     "DeleteVpcEndpointResponseTypeDef",
     {
         "VpcEndpointSummary": VpcEndpointSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsForDomainResponseTypeDef = TypedDict(
     "ListVpcEndpointsForDomainResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVpcEndpointsResponseTypeDef = TypedDict(
     "ListVpcEndpointsResponseTypeDef",
     {
         "VpcEndpointSummaryList": List[VpcEndpointSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1575,19 +1523,86 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef",
+    {
+        "ReservedElasticsearchInstanceOfferingId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = TypedDict(
+    "DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef",
+    {
+        "ReservedElasticsearchInstanceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef(
+    _RequiredGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    _OptionalGetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "ElasticsearchVersion": str,
+    },
+)
+_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = TypedDict(
+    "_OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef",
+    {
+        "DomainName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef(
+    _RequiredListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    _OptionalListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+):
+    pass
+
+ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = TypedDict(
+    "ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": str,
@@ -1660,15 +1675,15 @@
 
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InboundCrossClusterSearchConnectionTypeDef = TypedDict(
     "InboundCrossClusterSearchConnectionTypeDef",
     {
         "SourceDomainInfo": DomainInformationTypeDef,
@@ -1774,122 +1789,132 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsExtraOutputTypeDef = TypedDict(
+    "AutoTuneOptionsExtraOutputTypeDef",
+    {
+        "DesiredState": AutoTuneDesiredStateType,
+        "RollbackOnDisable": RollbackOnDisableType,
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
+    },
+    total=False,
+)
+
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteOutboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": OutboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[OutboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DissociatePackageResponseTypeDef = TypedDict(
     "DissociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePackageResponseTypeDef = TypedDict(
     "DeletePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ElasticsearchClusterConfigStatusTypeDef = TypedDict(
     "ElasticsearchClusterConfigStatusTypeDef",
     {
         "Options": ElasticsearchClusterConfigTypeDef,
@@ -1897,85 +1922,85 @@
     },
 )
 
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVpcEndpointsResponseTypeDef = TypedDict(
     "DescribeVpcEndpointsResponseTypeDef",
     {
         "VpcEndpoints": List[VpcEndpointTypeDef],
         "VpcEndpointErrors": List[VpcEndpointErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcEndpointResponseTypeDef = TypedDict(
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "AcceptInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "DeleteInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundCrossClusterSearchConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundCrossClusterSearchConnectionsResponseTypeDef",
     {
         "CrossClusterSearchConnections": List[InboundCrossClusterSearchConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectInboundCrossClusterSearchConnectionResponseTypeDef = TypedDict(
     "RejectInboundCrossClusterSearchConnectionResponseTypeDef",
     {
         "CrossClusterSearchConnection": InboundCrossClusterSearchConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstanceOfferings": List[
             ReservedElasticsearchInstanceOfferingTypeDef
         ],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedElasticsearchInstancesResponseTypeDef = TypedDict(
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedElasticsearchInstances": List[ReservedElasticsearchInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2010,36 +2035,37 @@
 )
 
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsTypeDef,
+        "Options": AutoTuneOptionsExtraOutputTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 _RequiredCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateElasticsearchDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
@@ -2153,15 +2179,15 @@
 ):
     pass
 
 DescribeElasticsearchInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ElasticsearchDomainConfigTypeDef = TypedDict(
     "ElasticsearchDomainConfigTypeDef",
     {
         "ElasticsearchVersion": ElasticsearchVersionStatusTypeDef,
@@ -2183,51 +2209,51 @@
     total=False,
 )
 
 CreateElasticsearchDomainResponseTypeDef = TypedDict(
     "CreateElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteElasticsearchDomainResponseTypeDef = TypedDict(
     "DeleteElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticsearchDomainResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainResponseTypeDef",
     {
         "DomainStatus": ElasticsearchDomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticsearchDomainsResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainsResponseTypeDef",
     {
         "DomainStatusList": List[ElasticsearchDomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "DescribeElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateElasticsearchDomainConfigResponseTypeDef = TypedDict(
     "UpdateElasticsearchDomainConfigResponseTypeDef",
     {
         "DomainConfig": ElasticsearchDomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/PKG-INFO` & `types-aiobotocore-es-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-es
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore es type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-es"></a>
 
 # types-aiobotocore-es
 
 [![PyPI - types-aiobotocore-es](https://img.shields.io/pypi/v/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-es.svg?color=blue)](https://pypi.org/project/types-aiobotocore-es)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-es?color=blue)](https://pypistats.org/packages/types-aiobotocore-es)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-es)](https://pepy.tech/project/types-aiobotocore-es)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticsearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
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
 [types-aiobotocore-es docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -356,33 +323,35 @@
 )
 
 
 def check_value(value: AutoTuneDesiredStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_es.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_es.type_defs import (
     AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
     DurationTypeDef,
+    TimestampTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     CancelElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
     CognitoOptionsTypeDef,
@@ -408,70 +377,65 @@
     DescribeDomainChangeProgressRequestRequestTypeDef,
     DescribeElasticsearchDomainConfigRequestRequestTypeDef,
     DescribeElasticsearchDomainRequestRequestTypeDef,
     DescribeElasticsearchDomainsRequestRequestTypeDef,
     DescribeElasticsearchInstanceTypeLimitsRequestRequestTypeDef,
     FilterTypeDef,
     DescribePackagesFilterTypeDef,
-    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeReservedElasticsearchInstanceOfferingsRequestRequestTypeDef,
-    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
     DescribeReservedElasticsearchInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     DryRunResultsTypeDef,
     ZoneAwarenessConfigTypeDef,
     VPCDerivedInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleElasticsearchVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
-    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundCrossClusterSearchConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
-    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
     ListElasticsearchInstanceTypesRequestRequestTypeDef,
-    ListElasticsearchInstanceTypesResponseTypeDef,
-    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListElasticsearchVersionsRequestRequestTypeDef,
-    ListElasticsearchVersionsResponseTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseReservedElasticsearchInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundCrossClusterSearchConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartElasticsearchServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpgradeElasticsearchDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListElasticsearchInstanceTypesResponseTypeDef,
+    ListElasticsearchVersionsResponseTypeDef,
+    PurchaseReservedElasticsearchInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     ElasticsearchVersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     StartElasticsearchServiceSoftwareUpdateResponseTypeDef,
     UpgradeElasticsearchDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleElasticsearchVersionsResponseTypeDef,
@@ -490,14 +454,19 @@
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeInboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
+    DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef,
+    DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef,
+    GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef,
+    ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef,
+    ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
     ElasticsearchClusterConfigTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
@@ -506,14 +475,15 @@
     ReservedElasticsearchInstanceOfferingTypeDef,
     ReservedElasticsearchInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     DeleteOutboundCrossClusterSearchConnectionResponseTypeDef,
     DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
@@ -535,14 +505,15 @@
     DescribeReservedElasticsearchInstancesResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CreateElasticsearchDomainRequestRequestTypeDef,
     UpdateElasticsearchDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     ElasticsearchDomainStatusTypeDef,
     DescribeElasticsearchInstanceTypeLimitsResponseTypeDef,
     ElasticsearchDomainConfigTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
@@ -550,15 +521,15 @@
     DescribeElasticsearchDomainResponseTypeDef,
     DescribeElasticsearchDomainsResponseTypeDef,
     DescribeElasticsearchDomainConfigResponseTypeDef,
     UpdateElasticsearchDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef:
+def get_value() -> AcceptInboundCrossClusterSearchConnectionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-es-2.5.2/types_aiobotocore_es.egg-info/SOURCES.txt` & `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*


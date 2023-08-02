# Comparing `tmp/types-aiobotocore-opensearch-2.5.2.tar.gz` & `tmp/types-aiobotocore-opensearch-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opensearch-2.5.2.tar", last modified: Sat Jul  8 01:44:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-opensearch-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:44 2023, max compression
```

## Comparing `types-aiobotocore-opensearch-2.5.2.tar` & `types-aiobotocore-opensearch-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.098628 types-aiobotocore-opensearch-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-07-08 01:44:04.098628 types-aiobotocore-opensearch-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:04.098628 types-aiobotocore-opensearch-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:35:59.000000 types-aiobotocore-opensearch-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.098628 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43479 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43416 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68145 2023-07-08 01:36:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68088 2023-07-08 01:36:01.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:00.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.098628 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-07-08 01:44:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-08 01:44:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:44:03.000000 types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43489 2023-08-02 14:44:19.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43426 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-08-02 14:44:19.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-02 14:44:19.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68915 2023-08-02 14:44:20.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68858 2023-08-02 14:44:20.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:18.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.933506 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:44.000000 types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opensearch-2.5.2/LICENSE` & `types-aiobotocore-opensearch-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearch-2.5.2/PKG-INFO` & `types-aiobotocore-opensearch-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.OpenSearchService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.OpenSearchService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore opensearch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore opensearch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-opensearch"></a>
 
 # types-aiobotocore-opensearch
 
 [![PyPI - types-aiobotocore-opensearch](https://img.shields.io/pypi/v/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opensearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-opensearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearch)](https://pepy.tech/project/types-aiobotocore-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpenSearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [types-aiobotocore-opensearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/).
 
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
@@ -322,34 +321,36 @@
 )
 
 
 def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_opensearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
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
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
@@ -392,59 +393,59 @@
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListVersionsResponseTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     ClusterConfigTypeDef,
@@ -485,14 +486,15 @@
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
     CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
@@ -517,14 +519,15 @@
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
@@ -536,15 +539,15 @@
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_value() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-opensearch-2.5.2/README.md` & `types-aiobotocore-opensearch-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-opensearch"></a>
 
 # types-aiobotocore-opensearch
 
 [![PyPI - types-aiobotocore-opensearch](https://img.shields.io/pypi/v/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opensearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-opensearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearch)](https://pepy.tech/project/types-aiobotocore-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpenSearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [types-aiobotocore-opensearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/).
 
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
@@ -289,34 +289,36 @@
 )
 
 
 def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_opensearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
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
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
@@ -359,59 +361,59 @@
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListVersionsResponseTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     ClusterConfigTypeDef,
@@ -452,14 +454,15 @@
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
     CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
@@ -484,14 +487,15 @@
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
@@ -503,15 +507,15 @@
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_value() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-opensearch-2.5.2/setup.py` & `types-aiobotocore-opensearch-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opensearch",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpenSearchService 2.5.2 service generated with"
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
-    keywords="aiobotocore opensearch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore opensearch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_opensearch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/"
```

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/__main__.py` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpenSearchService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.OpenSearchService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/client.py` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
@@ -747,15 +747,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/client.pyi` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
@@ -690,15 +690,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/literals.py` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/literals.pyi` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/type_defs.py` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_opensearch.type_defs import AWSDomainInformationTypeDef
 
-    data: AWSDomainInformationTypeDef = {...}
+    data: AWSDomainInformationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -66,23 +66,25 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
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
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
@@ -125,59 +127,59 @@
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListVersionsResponseTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
     "DomainInformationContainerTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
+    "ListVersionsResponseTypeDef",
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "ClusterConfigTypeDef",
@@ -218,14 +220,15 @@
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
@@ -250,14 +253,15 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
@@ -297,14 +301,25 @@
 AcceptInboundConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
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
@@ -391,14 +406,15 @@
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
         "UseOffPeakWindow": bool,
     },
@@ -912,21 +928,14 @@
     {
         "Code": str,
         "Message": str,
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
 GetCompatibleVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -989,24 +998,14 @@
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
 InboundConnectionStatusTypeDef = TypedDict(
     "InboundConnectionStatusTypeDef",
     {
         "StatusCode": InboundConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -1177,23 +1176,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
-    {
-        "Versions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
@@ -1269,23 +1259,14 @@
 class PurchaseReservedInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
 
-PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
-    {
-        "ReservedInstanceId": str,
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
@@ -1302,25 +1283,14 @@
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
@@ -1428,14 +1398,49 @@
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
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
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "Versions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
+    {
+        "ReservedInstanceId": str,
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
@@ -1464,47 +1469,57 @@
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
 
 EnvironmentInfoTypeDef = TypedDict(
@@ -1515,36 +1530,36 @@
     total=False,
 )
 
 CancelServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpgradeDomainResponseTypeDef = TypedDict(
     "UpgradeDomainResponseTypeDef",
     {
         "UpgradeId": str,
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "AdvancedOptions": Dict[str, str],
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1585,15 +1600,15 @@
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionPropertiesTypeDef = TypedDict(
     "ConnectionPropertiesTypeDef",
     {
         "Endpoint": str,
@@ -1736,41 +1751,41 @@
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
 
 DescribeDomainNodesResponseTypeDef = TypedDict(
     "DescribeDomainNodesResponseTypeDef",
     {
         "DomainNodesStatusList": List[DomainNodesStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1800,15 +1815,15 @@
     total=False,
 )
 
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
@@ -1887,15 +1902,15 @@
 
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
 
 InstanceLimitsTypeDef = TypedDict(
     "InstanceLimitsTypeDef",
     {
         "InstanceCountLimits": InstanceCountLimitsTypeDef,
@@ -1904,32 +1919,32 @@
 )
 
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
@@ -2037,14 +2052,25 @@
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
+        "UseOffPeakWindow": bool,
+    },
+    total=False,
+)
+
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
@@ -2052,15 +2078,15 @@
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
@@ -2074,23 +2100,23 @@
         "MasterEligibleNodeCount": str,
         "WarmNodeCount": str,
         "MasterNode": MasterNodeStatusType,
         "ClusterHealth": DomainHealthType,
         "TotalShards": str,
         "TotalUnAssignedShards": str,
         "EnvironmentInformation": List[EnvironmentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
         "Options": ClusterConfigTypeDef,
@@ -2129,15 +2155,15 @@
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundConnectionStatusTypeDef,
         "ConnectionId": str,
         "ConnectionMode": ConnectionModeType,
         "ConnectionProperties": ConnectionPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OutboundConnectionTypeDef = TypedDict(
     "OutboundConnectionTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
@@ -2151,99 +2177,99 @@
     total=False,
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
 
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
@@ -2253,24 +2279,24 @@
 )
 
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2305,83 +2331,84 @@
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
 
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInboundConnectionResponseTypeDef = TypedDict(
     "DeleteInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
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
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOutboundConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundConnectionsResponseTypeDef",
     {
         "Connections": List[OutboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
         "Options": OffPeakWindowOptionsTypeDef,
@@ -2517,15 +2544,15 @@
     pass
 
 
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainConfigTypeDef = TypedDict(
     "DomainConfigTypeDef",
     {
         "EngineVersion": VersionStatusTypeDef,
@@ -2549,62 +2576,62 @@
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDryRunProgressResponseTypeDef = TypedDict(
     "DescribeDryRunProgressResponseTypeDef",
     {
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
         "DryRunConfig": DomainStatusTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainConfigResponseTypeDef = TypedDict(
     "DescribeDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainConfigResponseTypeDef = TypedDict(
     "UpdateDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch/type_defs.pyi` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_opensearch.type_defs import AWSDomainInformationTypeDef
 
-    data: AWSDomainInformationTypeDef = {...}
+    data: AWSDomainInformationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -65,23 +65,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
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
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
@@ -124,59 +126,59 @@
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
-    "GetUpgradeStatusResponseTypeDef",
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListVersionsResponseTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
     "DomainInformationContainerTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetUpgradeStatusResponseTypeDef",
+    "ListVersionsResponseTypeDef",
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "ClusterConfigTypeDef",
@@ -217,14 +219,15 @@
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
@@ -249,14 +252,15 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
@@ -294,14 +298,25 @@
 AcceptInboundConnectionRequestRequestTypeDef = TypedDict(
     "AcceptInboundConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
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
@@ -386,14 +401,15 @@
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
         "UseOffPeakWindow": bool,
     },
@@ -897,21 +913,14 @@
     {
         "Code": str,
         "Message": str,
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
 GetCompatibleVersionsRequestRequestTypeDef = TypedDict(
     "GetCompatibleVersionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
     total=False,
 )
@@ -970,24 +979,14 @@
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
 InboundConnectionStatusTypeDef = TypedDict(
     "InboundConnectionStatusTypeDef",
     {
         "StatusCode": InboundConnectionStatusCodeType,
         "Message": str,
     },
     total=False,
@@ -1148,23 +1147,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
-    {
-        "Versions": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
     "_RequiredListVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListVpcEndpointAccessRequestRequestTypeDef = TypedDict(
@@ -1234,23 +1224,14 @@
 
 class PurchaseReservedInstanceOfferingRequestRequestTypeDef(
     _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef,
     _OptionalPurchaseReservedInstanceOfferingRequestRequestTypeDef,
 ):
     pass
 
-PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
-    "PurchaseReservedInstanceOfferingResponseTypeDef",
-    {
-        "ReservedInstanceId": str,
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
@@ -1267,25 +1248,14 @@
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
@@ -1387,14 +1357,49 @@
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
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
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "Versions": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
+    "PurchaseReservedInstanceOfferingResponseTypeDef",
+    {
+        "ReservedInstanceId": str,
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
@@ -1423,47 +1428,57 @@
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
 
 EnvironmentInfoTypeDef = TypedDict(
@@ -1474,36 +1489,36 @@
     total=False,
 )
 
 CancelServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "CancelServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartServiceSoftwareUpdateResponseTypeDef = TypedDict(
     "StartServiceSoftwareUpdateResponseTypeDef",
     {
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpgradeDomainResponseTypeDef = TypedDict(
     "UpgradeDomainResponseTypeDef",
     {
         "UpgradeId": str,
         "DomainName": str,
         "TargetVersion": str,
         "PerformCheckOnly": bool,
         "AdvancedOptions": Dict[str, str],
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeProgressStatusDetailsTypeDef = TypedDict(
     "ChangeProgressStatusDetailsTypeDef",
     {
         "ChangeId": str,
@@ -1544,15 +1559,15 @@
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionPropertiesTypeDef = TypedDict(
     "ConnectionPropertiesTypeDef",
     {
         "Endpoint": str,
@@ -1689,41 +1704,41 @@
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
 
 DescribeDomainNodesResponseTypeDef = TypedDict(
     "DescribeDomainNodesResponseTypeDef",
     {
         "DomainNodesStatusList": List[DomainNodesStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsRequestRequestTypeDef = TypedDict(
     "DescribeInboundConnectionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
@@ -1753,15 +1768,15 @@
     total=False,
 )
 
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
@@ -1838,15 +1853,15 @@
 
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
 
 InstanceLimitsTypeDef = TypedDict(
     "InstanceLimitsTypeDef",
     {
         "InstanceCountLimits": InstanceCountLimitsTypeDef,
@@ -1855,32 +1870,32 @@
 )
 
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
@@ -1988,14 +2003,25 @@
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
+        "UseOffPeakWindow": bool,
+    },
+    total=False,
+)
+
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
@@ -2003,15 +2029,15 @@
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
         "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
@@ -2025,23 +2051,23 @@
         "MasterEligibleNodeCount": str,
         "WarmNodeCount": str,
         "MasterNode": MasterNodeStatusType,
         "ClusterHealth": DomainHealthType,
         "TotalShards": str,
         "TotalUnAssignedShards": str,
         "EnvironmentInformation": List[EnvironmentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatus": ChangeProgressStatusDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
         "Options": ClusterConfigTypeDef,
@@ -2078,15 +2104,15 @@
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionAlias": str,
         "ConnectionStatus": OutboundConnectionStatusTypeDef,
         "ConnectionId": str,
         "ConnectionMode": ConnectionModeType,
         "ConnectionProperties": ConnectionPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OutboundConnectionTypeDef = TypedDict(
     "OutboundConnectionTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
@@ -2100,99 +2126,99 @@
     total=False,
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
 
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
@@ -2202,24 +2228,24 @@
 )
 
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
@@ -2254,83 +2280,84 @@
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
 
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInboundConnectionResponseTypeDef = TypedDict(
     "DeleteInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
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
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOutboundConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundConnectionsResponseTypeDef",
     {
         "Connections": List[OutboundConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
         "Options": OffPeakWindowOptionsTypeDef,
@@ -2460,15 +2487,15 @@
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainConfigTypeDef = TypedDict(
     "DomainConfigTypeDef",
     {
         "EngineVersion": VersionStatusTypeDef,
@@ -2492,62 +2519,62 @@
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResponseTypeDef = TypedDict(
     "DeleteDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "DomainStatus": DomainStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainsResponseTypeDef = TypedDict(
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDryRunProgressResponseTypeDef = TypedDict(
     "DescribeDryRunProgressResponseTypeDef",
     {
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
         "DryRunConfig": DomainStatusTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainConfigResponseTypeDef = TypedDict(
     "DescribeDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainConfigResponseTypeDef = TypedDict(
     "UpdateDomainConfigResponseTypeDef",
     {
         "DomainConfig": DomainConfigTypeDef,
         "DryRunResults": DryRunResultsTypeDef,
         "DryRunProgressStatus": DryRunProgressStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/PKG-INFO` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.OpenSearchService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.OpenSearchService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore opensearch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore opensearch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-opensearch"></a>
 
 # types-aiobotocore-opensearch
 
 [![PyPI - types-aiobotocore-opensearch](https://img.shields.io/pypi/v/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opensearch?color=blue)](https://pypistats.org/packages/types-aiobotocore-opensearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearch)](https://pepy.tech/project/types-aiobotocore-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpenSearchService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [types-aiobotocore-opensearch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearch/).
 
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
@@ -322,34 +321,36 @@
 )
 
 
 def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_opensearch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_opensearch.type_defs import (
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
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
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
@@ -392,59 +393,59 @@
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
-    GetUpgradeStatusResponseTypeDef,
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
-    PurchaseReservedInstanceOfferingResponseTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetUpgradeStatusResponseTypeDef,
+    ListVersionsResponseTypeDef,
+    PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
+    AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
     ClusterConfigTypeDef,
@@ -485,14 +486,15 @@
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
+    AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
     CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
@@ -517,14 +519,15 @@
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
@@ -536,15 +539,15 @@
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationTypeDef:
+def get_value() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-opensearch-2.5.2/types_aiobotocore_opensearch.egg-info/SOURCES.txt` & `types-aiobotocore-opensearch-2.5.2.post1/types_aiobotocore_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


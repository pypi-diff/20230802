# Comparing `tmp/types-aiobotocore-snowball-2.5.2.tar.gz` & `tmp/types-aiobotocore-snowball-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-snowball-2.5.2.tar", last modified: Sat Jul  8 01:44:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-snowball-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:03 2023, max compression
```

## Comparing `types-aiobotocore-snowball-2.5.2.tar` & `types-aiobotocore-snowball-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:21.446923 types-aiobotocore-snowball-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-07-08 01:44:21.446923 types-aiobotocore-snowball-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:21.446923 types-aiobotocore-snowball-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:21.446923 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-07-08 01:41:15.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27628 2023-07-08 01:41:15.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-07-08 01:41:15.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:14.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:21.446923 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-07-08 01:44:21.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:44:21.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:21.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:21.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:21.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:21.000000 types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.137451 types-aiobotocore-snowball-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-08-02 14:53:03.133451 types-aiobotocore-snowball-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:03.137451 types-aiobotocore-snowball-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.133451 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28873 2023-08-02 14:49:55.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.133451 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-snowball-2.5.2/LICENSE` & `types-aiobotocore-snowball-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2/PKG-INFO` & `types-aiobotocore-snowball-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snowball
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore snowball type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore snowball type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-snowball"></a>
 
 # types-aiobotocore-snowball
 
 [![PyPI - types-aiobotocore-snowball](https://img.shields.io/pypi/v/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-snowball?color=blue)](https://pypistats.org/packages/types-aiobotocore-snowball)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Snowball 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [types-aiobotocore-snowball docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/).
 
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
@@ -343,111 +342,117 @@
 )
 
 
 def check_value(value: ClusterStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_snowball.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_snowball.type_defs import (
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    CreateAddressResultTypeDef,
+    ResponseMetadataTypeDef,
+    NotificationTypeDef,
     JobListEntryTypeDef,
-    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
-    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
-    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
+    CreateAddressResultTypeDef,
+    CreateJobResultTypeDef,
+    CreateLongTermPricingResultTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
+    GetJobManifestResultTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
+    NotificationUnionTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
     DependentServiceTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
+    LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
+    JobResourceOutputTypeDef,
     JobResourceTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
+    JobResourceUnionTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
     CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-snowball-2.5.2/README.md` & `types-aiobotocore-snowball-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-snowball"></a>
 
 # types-aiobotocore-snowball
 
 [![PyPI - types-aiobotocore-snowball](https://img.shields.io/pypi/v/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-snowball?color=blue)](https://pypistats.org/packages/types-aiobotocore-snowball)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Snowball 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [types-aiobotocore-snowball docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/).
 
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
@@ -310,111 +310,117 @@
 )
 
 
 def check_value(value: ClusterStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_snowball.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_snowball.type_defs import (
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    CreateAddressResultTypeDef,
+    ResponseMetadataTypeDef,
+    NotificationTypeDef,
     JobListEntryTypeDef,
-    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
-    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
-    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
+    CreateAddressResultTypeDef,
+    CreateJobResultTypeDef,
+    CreateLongTermPricingResultTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
+    GetJobManifestResultTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
+    NotificationUnionTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
     DependentServiceTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
+    LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
+    JobResourceOutputTypeDef,
     JobResourceTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
+    JobResourceUnionTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
     CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-snowball-2.5.2/setup.py` & `types-aiobotocore-snowball-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-snowball",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore snowball type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore snowball type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_snowball": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/"
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/__init__.py` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/__init__.pyi` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/__main__.py` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Snowball 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Snowball 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
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

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/client.py` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,22 +52,22 @@
     DescribeJobResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     DeviceConfigurationTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
-    JobResourceTypeDef,
+    JobResourceUnionTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     ListServiceVersionsResultTypeDef,
-    NotificationTypeDef,
+    NotificationUnionTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -160,20 +160,20 @@
     async def create_cluster(
         self,
         *,
         JobType: JobTypeType,
         AddressId: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
-        Notification: NotificationTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...
@@ -185,23 +185,23 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_cluster)
         """
 
     async def create_job(
         self,
         *,
         JobType: JobTypeType = ...,
-        Resources: JobResourceTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         AddressId: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         LongTermPricingId: str = ...
@@ -405,19 +405,19 @@
 
     async def update_cluster(
         self,
         *,
         ClusterId: str,
         RoleARN: str = ...,
         Description: str = ...,
-        Resources: JobResourceTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you can
         update some of the information associated with a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
@@ -425,16 +425,16 @@
         """
 
     async def update_job(
         self,
         *,
         JobId: str,
         RoleARN: str = ...,
-        Notification: NotificationTypeDef = ...,
-        Resources: JobResourceTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/client.pyi` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,22 +52,22 @@
     DescribeJobResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     DeviceConfigurationTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
-    JobResourceTypeDef,
+    JobResourceUnionTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
     ListServiceVersionsResultTypeDef,
-    NotificationTypeDef,
+    NotificationUnionTypeDef,
     OnDeviceServiceConfigurationTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -150,20 +150,20 @@
     async def create_cluster(
         self,
         *,
         JobType: JobTypeType,
         AddressId: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
-        Notification: NotificationTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...
@@ -174,23 +174,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_cluster)
         """
     async def create_job(
         self,
         *,
         JobType: JobTypeType = ...,
-        Resources: JobResourceTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         AddressId: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         LongTermPricingId: str = ...
@@ -375,35 +375,35 @@
         """
     async def update_cluster(
         self,
         *,
         ClusterId: str,
         RoleARN: str = ...,
         Description: str = ...,
-        Resources: JobResourceTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you can
         update some of the information associated with a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#update_cluster)
         """
     async def update_job(
         self,
         *,
         JobId: str,
         RoleARN: str = ...,
-        Notification: NotificationTypeDef = ...,
-        Resources: JobResourceTypeDef = ...,
+        Notification: NotificationUnionTypeDef = ...,
+        Resources: JobResourceUnionTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/literals.py` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/literals.pyi` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/paginator.py` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,88 +68,88 @@
 class DescribeAddressesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#describeaddressespaginator)
         """
 
 
 class ListClusterJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterjobspaginator)
         """
 
 
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterspaginator)
         """
 
 
 class ListCompatibleImagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 
 class ListJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listjobspaginator)
         """
 
 
 class ListLongTermPricingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/paginator.pyi` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -65,83 +65,83 @@
 class DescribeAddressesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#describeaddressespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAddressesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#describeaddressespaginator)
         """
 
 class ListClusterJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterjobspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClusterJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterjobspaginator)
         """
 
 class ListClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listclusterspaginator)
         """
 
 class ListCompatibleImagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listcompatibleimagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCompatibleImagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listcompatibleimagespaginator)
         """
 
 class ListJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listjobspaginator)
         """
 
 class ListLongTermPricingPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listlongtermpricingpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLongTermPricingResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListLongTermPricing.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/paginators/#listlongtermpricingpaginator)
         """
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/type_defs.py` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_snowball.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ClusterStateType,
     DeviceServiceNameType,
     JobStateType,
     JobTypeType,
     LongTermPricingTypeType,
@@ -42,88 +42,94 @@
 
 
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
-    "NotificationTypeDef",
+    "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
-    "CreateAddressResultTypeDef",
+    "ResponseMetadataTypeDef",
+    "NotificationTypeDef",
     "JobListEntryTypeDef",
-    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
-    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
-    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
     "KeyRangeTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
+    "CreateAddressResultTypeDef",
+    "CreateJobResultTypeDef",
+    "CreateLongTermPricingResultTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
+    "GetJobManifestResultTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
+    "NotificationUnionTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
+    "S3ResourceOutputTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
+    "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
+    "JobResourceUnionTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
@@ -170,63 +176,68 @@
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
+NotificationOutputTypeDef = TypedDict(
+    "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
-        "JobStatesToNotify": Sequence[JobStateType],
+        "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
     },
     total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
     total=False,
 )
 
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AddressId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
+    {
+        "SnsTopicARN": str,
+        "JobStatesToNotify": Sequence[JobStateType],
+        "NotifyAll": bool,
+    },
+    total=False,
+)
+
 JobListEntryTypeDef = TypedDict(
     "JobListEntryTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
@@ -242,22 +253,14 @@
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
 
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -272,22 +275,14 @@
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
 
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
@@ -306,18 +301,20 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
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
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -344,24 +341,14 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
@@ -397,61 +384,28 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
-    {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
-    {
-        "UpdatesURI": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
@@ -471,36 +425,14 @@
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -515,73 +447,41 @@
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
 
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -629,35 +529,14 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
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
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -714,85 +593,232 @@
 CreateAddressRequestRequestTypeDef = TypedDict(
     "CreateAddressRequestRequestTypeDef",
     {
         "Address": AddressTypeDef,
     },
 )
 
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
+    {
+        "AddressId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
         "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
         "Addresses": List[AddressTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
+    {
+        "UpdatesURI": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NotificationUnionTypeDef = Union[NotificationTypeDef, NotificationOutputTypeDef]
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClusterJobsResultTypeDef = TypedDict(
     "ListClusterJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+LambdaResourceOutputTypeDef = TypedDict(
+    "LambdaResourceOutputTypeDef",
+    {
+        "LambdaArn": str,
+        "EventTriggers": List[EventTriggerDefinitionTypeDef],
+    },
+    total=False,
+)
+
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
@@ -807,29 +833,39 @@
 )
 
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
+S3ResourceOutputTypeDef = TypedDict(
+    "S3ResourceOutputTypeDef",
+    {
+        "BucketArn": str,
+        "KeyRange": KeyRangeTypeDef,
+        "TargetOnDeviceServices": List[TargetOnDeviceServiceTypeDef],
+    },
+    total=False,
+)
+
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
         "TargetOnDeviceServices": Sequence[TargetOnDeviceServiceTypeDef],
     },
@@ -881,16 +917,26 @@
 ListServiceVersionsResultTypeDef = TypedDict(
     "ListServiceVersionsResultTypeDef",
     {
         "ServiceVersions": List[ServiceVersionTypeDef],
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobResourceOutputTypeDef = TypedDict(
+    "JobResourceOutputTypeDef",
+    {
+        "S3Resources": List[S3ResourceOutputTypeDef],
+        "LambdaResources": List[LambdaResourceOutputTypeDef],
+        "Ec2AmiResources": List[Ec2AmiResourceTypeDef],
     },
+    total=False,
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
@@ -914,18 +960,18 @@
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "ClusterState": ClusterStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceTypeDef,
+        "Resources": JobResourceOutputTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -961,14 +1007,15 @@
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
 
+JobResourceUnionTypeDef = Union[JobResourceTypeDef, JobResourceOutputTypeDef]
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
@@ -1050,22 +1097,22 @@
     "JobMetadataTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceTypeDef,
+        "Resources": JobResourceOutputTypeDef,
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "AddressId": str,
         "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
         "DataTransferProgress": DataTransferTypeDef,
         "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
@@ -1075,19 +1122,19 @@
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball/type_defs.pyi` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_snowball.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ClusterStateType,
     DeviceServiceNameType,
     JobStateType,
     JobTypeType,
     LongTermPricingTypeType,
@@ -41,88 +41,94 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
-    "NotificationTypeDef",
+    "NotificationOutputTypeDef",
     "CompatibleImageTypeDef",
-    "CreateAddressResultTypeDef",
+    "ResponseMetadataTypeDef",
+    "NotificationTypeDef",
     "JobListEntryTypeDef",
-    "CreateJobResultTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
-    "CreateLongTermPricingResultTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
-    "CreateReturnShippingLabelResultTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAddressesRequestRequestTypeDef",
     "DescribeClusterRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeReturnShippingLabelRequestRequestTypeDef",
-    "DescribeReturnShippingLabelResultTypeDef",
     "EKSOnDeviceServiceConfigurationTypeDef",
     "Ec2AmiResourceTypeDef",
     "EventTriggerDefinitionTypeDef",
     "GetJobManifestRequestRequestTypeDef",
-    "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeRequestRequestTypeDef",
-    "GetJobUnlockCodeResultTypeDef",
-    "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesRequestRequestTypeDef",
-    "GetSoftwareUpdatesResultTypeDef",
     "INDTaxDocumentsTypeDef",
     "JobLogsTypeDef",
     "KeyRangeTypeDef",
-    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
-    "ListClustersRequestListClustersPaginateTypeDef",
     "ListClustersRequestRequestTypeDef",
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
+    "CreateAddressResultTypeDef",
+    "CreateJobResultTypeDef",
+    "CreateLongTermPricingResultTypeDef",
+    "CreateReturnShippingLabelResultTypeDef",
     "DescribeAddressResultTypeDef",
     "DescribeAddressesResultTypeDef",
+    "DescribeReturnShippingLabelResultTypeDef",
+    "GetJobManifestResultTypeDef",
+    "GetJobUnlockCodeResultTypeDef",
+    "GetSnowballUsageResultTypeDef",
+    "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
+    "NotificationUnionTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
+    "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    "ListClustersRequestListClustersPaginateTypeDef",
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
+    "S3ResourceOutputTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
+    "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
+    "JobResourceUnionTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
@@ -169,63 +175,68 @@
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
+NotificationOutputTypeDef = TypedDict(
+    "NotificationOutputTypeDef",
     {
         "SnsTopicARN": str,
-        "JobStatesToNotify": Sequence[JobStateType],
+        "JobStatesToNotify": List[JobStateType],
         "NotifyAll": bool,
     },
     total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
         "AmiId": str,
         "Name": str,
     },
     total=False,
 )
 
-CreateAddressResultTypeDef = TypedDict(
-    "CreateAddressResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AddressId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
+    {
+        "SnsTopicARN": str,
+        "JobStatesToNotify": Sequence[JobStateType],
+        "NotifyAll": bool,
+    },
+    total=False,
+)
+
 JobListEntryTypeDef = TypedDict(
     "JobListEntryTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
@@ -239,22 +250,14 @@
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
 ):
     pass
 
-CreateLongTermPricingResultTypeDef = TypedDict(
-    "CreateLongTermPricingResultTypeDef",
-    {
-        "LongTermPricingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalCreateReturnShippingLabelRequestRequestTypeDef = TypedDict(
@@ -267,22 +270,14 @@
 
 class CreateReturnShippingLabelRequestRequestTypeDef(
     _RequiredCreateReturnShippingLabelRequestRequestTypeDef,
     _OptionalCreateReturnShippingLabelRequestRequestTypeDef,
 ):
     pass
 
-CreateReturnShippingLabelResultTypeDef = TypedDict(
-    "CreateReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataTransferTypeDef = TypedDict(
     "DataTransferTypeDef",
     {
         "BytesTransferred": int,
         "ObjectsTransferred": int,
         "TotalBytes": int,
         "TotalObjects": int,
@@ -301,18 +296,20 @@
 DescribeAddressRequestRequestTypeDef = TypedDict(
     "DescribeAddressRequestRequestTypeDef",
     {
         "AddressId": str,
     },
 )
 
-DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
-    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
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
 
 DescribeAddressesRequestRequestTypeDef = TypedDict(
     "DescribeAddressesRequestRequestTypeDef",
     {
@@ -339,24 +336,14 @@
 DescribeReturnShippingLabelRequestRequestTypeDef = TypedDict(
     "DescribeReturnShippingLabelRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DescribeReturnShippingLabelResultTypeDef = TypedDict(
-    "DescribeReturnShippingLabelResultTypeDef",
-    {
-        "Status": ShippingLabelStatusType,
-        "ExpirationDate": datetime,
-        "ReturnShippingLabelURI": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EKSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "EKSOnDeviceServiceConfigurationTypeDef",
     {
         "KubernetesVersion": str,
         "EKSAnywhereVersion": str,
     },
     total=False,
@@ -390,61 +377,28 @@
 GetJobManifestRequestRequestTypeDef = TypedDict(
     "GetJobManifestRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-GetJobManifestResultTypeDef = TypedDict(
-    "GetJobManifestResultTypeDef",
-    {
-        "ManifestURI": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobUnlockCodeRequestRequestTypeDef = TypedDict(
     "GetJobUnlockCodeRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-GetJobUnlockCodeResultTypeDef = TypedDict(
-    "GetJobUnlockCodeResultTypeDef",
-    {
-        "UnlockCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSnowballUsageResultTypeDef = TypedDict(
-    "GetSnowballUsageResultTypeDef",
-    {
-        "SnowballLimit": int,
-        "SnowballsInUse": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSoftwareUpdatesRequestRequestTypeDef = TypedDict(
     "GetSoftwareUpdatesRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-GetSoftwareUpdatesResultTypeDef = TypedDict(
-    "GetSoftwareUpdatesResultTypeDef",
-    {
-        "UpdatesURI": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 INDTaxDocumentsTypeDef = TypedDict(
     "INDTaxDocumentsTypeDef",
     {
         "GSTIN": str,
     },
     total=False,
 )
@@ -464,34 +418,14 @@
     {
         "BeginMarker": str,
         "EndMarker": str,
     },
     total=False,
 )
 
-_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
-    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
-    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
-    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListClusterJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListClusterJobsRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListClusterJobsRequestRequestTypeDef = TypedDict(
@@ -504,73 +438,41 @@
 )
 
 class ListClusterJobsRequestRequestTypeDef(
     _RequiredListClusterJobsRequestRequestTypeDef, _OptionalListClusterJobsRequestRequestTypeDef
 ):
     pass
 
-ListClustersRequestListClustersPaginateTypeDef = TypedDict(
-    "ListClustersRequestListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
-    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCompatibleImagesRequestRequestTypeDef = TypedDict(
     "ListCompatibleImagesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
-    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLongTermPricingRequestRequestTypeDef = TypedDict(
     "ListLongTermPricingRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -618,35 +520,14 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
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
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -701,85 +582,230 @@
 CreateAddressRequestRequestTypeDef = TypedDict(
     "CreateAddressRequestRequestTypeDef",
     {
         "Address": AddressTypeDef,
     },
 )
 
+CreateAddressResultTypeDef = TypedDict(
+    "CreateAddressResultTypeDef",
+    {
+        "AddressId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLongTermPricingResultTypeDef = TypedDict(
+    "CreateLongTermPricingResultTypeDef",
+    {
+        "LongTermPricingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReturnShippingLabelResultTypeDef = TypedDict(
+    "CreateReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAddressResultTypeDef = TypedDict(
     "DescribeAddressResultTypeDef",
     {
         "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAddressesResultTypeDef = TypedDict(
     "DescribeAddressesResultTypeDef",
     {
         "Addresses": List[AddressTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReturnShippingLabelResultTypeDef = TypedDict(
+    "DescribeReturnShippingLabelResultTypeDef",
+    {
+        "Status": ShippingLabelStatusType,
+        "ExpirationDate": datetime,
+        "ReturnShippingLabelURI": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobManifestResultTypeDef = TypedDict(
+    "GetJobManifestResultTypeDef",
+    {
+        "ManifestURI": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobUnlockCodeResultTypeDef = TypedDict(
+    "GetJobUnlockCodeResultTypeDef",
+    {
+        "UnlockCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSnowballUsageResultTypeDef = TypedDict(
+    "GetSnowballUsageResultTypeDef",
+    {
+        "SnowballLimit": int,
+        "SnowballsInUse": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSoftwareUpdatesResultTypeDef = TypedDict(
+    "GetSoftwareUpdatesResultTypeDef",
+    {
+        "UpdatesURI": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClustersResultTypeDef = TypedDict(
     "ListClustersResultTypeDef",
     {
         "ClusterListEntries": List[ClusterListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCompatibleImagesResultTypeDef = TypedDict(
     "ListCompatibleImagesResultTypeDef",
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NotificationUnionTypeDef = Union[NotificationTypeDef, NotificationOutputTypeDef]
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListClusterJobsResultTypeDef = TypedDict(
     "ListClusterJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "JobListEntries": List[JobListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DependentServiceTypeDef = TypedDict(
     "DependentServiceTypeDef",
     {
         "ServiceName": ServiceNameType,
         "ServiceVersion": ServiceVersionTypeDef,
     },
     total=False,
 )
 
+DescribeAddressesRequestDescribeAddressesPaginateTypeDef = TypedDict(
+    "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef = TypedDict(
+    "_OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClusterJobsRequestListClusterJobsPaginateTypeDef(
+    _RequiredListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    _OptionalListClusterJobsRequestListClusterJobsPaginateTypeDef,
+):
+    pass
+
+ListClustersRequestListClustersPaginateTypeDef = TypedDict(
+    "ListClustersRequestListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = TypedDict(
+    "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLongTermPricingRequestListLongTermPricingPaginateTypeDef = TypedDict(
+    "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+LambdaResourceOutputTypeDef = TypedDict(
+    "LambdaResourceOutputTypeDef",
+    {
+        "LambdaArn": str,
+        "EventTriggers": List[EventTriggerDefinitionTypeDef],
+    },
+    total=False,
+)
+
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
@@ -794,29 +820,39 @@
 )
 
 ListLongTermPricingResultTypeDef = TypedDict(
     "ListLongTermPricingResultTypeDef",
     {
         "LongTermPricingEntries": List[LongTermPricingListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OnDeviceServiceConfigurationTypeDef = TypedDict(
     "OnDeviceServiceConfigurationTypeDef",
     {
         "NFSOnDeviceService": NFSOnDeviceServiceConfigurationTypeDef,
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
+S3ResourceOutputTypeDef = TypedDict(
+    "S3ResourceOutputTypeDef",
+    {
+        "BucketArn": str,
+        "KeyRange": KeyRangeTypeDef,
+        "TargetOnDeviceServices": List[TargetOnDeviceServiceTypeDef],
+    },
+    total=False,
+)
+
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
         "BucketArn": str,
         "KeyRange": KeyRangeTypeDef,
         "TargetOnDeviceServices": Sequence[TargetOnDeviceServiceTypeDef],
     },
@@ -866,16 +902,26 @@
 ListServiceVersionsResultTypeDef = TypedDict(
     "ListServiceVersionsResultTypeDef",
     {
         "ServiceVersions": List[ServiceVersionTypeDef],
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobResourceOutputTypeDef = TypedDict(
+    "JobResourceOutputTypeDef",
+    {
+        "S3Resources": List[S3ResourceOutputTypeDef],
+        "LambdaResources": List[LambdaResourceOutputTypeDef],
+        "Ec2AmiResources": List[Ec2AmiResourceTypeDef],
     },
+    total=False,
 )
 
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
@@ -899,18 +945,18 @@
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "ClusterState": ClusterStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceTypeDef,
+        "Resources": JobResourceOutputTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -944,14 +990,15 @@
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
+JobResourceUnionTypeDef = Union[JobResourceTypeDef, JobResourceOutputTypeDef]
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
@@ -1029,22 +1076,22 @@
     "JobMetadataTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceTypeDef,
+        "Resources": JobResourceOutputTypeDef,
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "AddressId": str,
         "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "Notification": NotificationTypeDef,
+        "Notification": NotificationOutputTypeDef,
         "DataTransferProgress": DataTransferTypeDef,
         "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
@@ -1054,19 +1101,19 @@
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
         "ClusterMetadata": ClusterMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "JobMetadata": JobMetadataTypeDef,
         "SubJobMetadata": List[JobMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/PKG-INFO` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-snowball
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore snowball type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore snowball type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-snowball"></a>
 
 # types-aiobotocore-snowball
 
 [![PyPI - types-aiobotocore-snowball](https://img.shields.io/pypi/v/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-snowball.svg?color=blue)](https://pypi.org/project/types-aiobotocore-snowball)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-snowball?color=blue)](https://pypistats.org/packages/types-aiobotocore-snowball)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-snowball)](https://pepy.tech/project/types-aiobotocore-snowball)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Snowball 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
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
 [types-aiobotocore-snowball docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/).
 
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
@@ -343,111 +342,117 @@
 )
 
 
 def check_value(value: ClusterStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_snowball.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_snowball.type_defs import (
     AddressTypeDef,
     CancelClusterRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
     ClusterListEntryTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
     CompatibleImageTypeDef,
-    CreateAddressResultTypeDef,
+    ResponseMetadataTypeDef,
+    NotificationTypeDef,
     JobListEntryTypeDef,
-    CreateJobResultTypeDef,
     CreateLongTermPricingRequestRequestTypeDef,
-    CreateLongTermPricingResultTypeDef,
     CreateReturnShippingLabelRequestRequestTypeDef,
-    CreateReturnShippingLabelResultTypeDef,
     DataTransferTypeDef,
     ServiceVersionTypeDef,
     DescribeAddressRequestRequestTypeDef,
-    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAddressesRequestRequestTypeDef,
     DescribeClusterRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeReturnShippingLabelRequestRequestTypeDef,
-    DescribeReturnShippingLabelResultTypeDef,
     EKSOnDeviceServiceConfigurationTypeDef,
     Ec2AmiResourceTypeDef,
     EventTriggerDefinitionTypeDef,
     GetJobManifestRequestRequestTypeDef,
-    GetJobManifestResultTypeDef,
     GetJobUnlockCodeRequestRequestTypeDef,
-    GetJobUnlockCodeResultTypeDef,
-    GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesRequestRequestTypeDef,
-    GetSoftwareUpdatesResultTypeDef,
     INDTaxDocumentsTypeDef,
     JobLogsTypeDef,
     KeyRangeTypeDef,
-    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
     ListClusterJobsRequestRequestTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
     ListClustersRequestRequestTypeDef,
-    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
     ListCompatibleImagesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
     ListLongTermPricingRequestRequestTypeDef,
     LongTermPricingListEntryTypeDef,
     NFSOnDeviceServiceConfigurationTypeDef,
     S3OnDeviceServiceConfigurationTypeDef,
     TGWOnDeviceServiceConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TargetOnDeviceServiceTypeDef,
     ShipmentTypeDef,
     WirelessConnectionTypeDef,
     UpdateJobShipmentStateRequestRequestTypeDef,
     UpdateLongTermPricingRequestRequestTypeDef,
     CreateAddressRequestRequestTypeDef,
+    CreateAddressResultTypeDef,
+    CreateJobResultTypeDef,
+    CreateLongTermPricingResultTypeDef,
+    CreateReturnShippingLabelResultTypeDef,
     DescribeAddressResultTypeDef,
     DescribeAddressesResultTypeDef,
+    DescribeReturnShippingLabelResultTypeDef,
+    GetJobManifestResultTypeDef,
+    GetJobUnlockCodeResultTypeDef,
+    GetSnowballUsageResultTypeDef,
+    GetSoftwareUpdatesResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
+    NotificationUnionTypeDef,
     CreateClusterResultTypeDef,
     ListClusterJobsResultTypeDef,
     ListJobsResultTypeDef,
     DependentServiceTypeDef,
+    DescribeAddressesRequestDescribeAddressesPaginateTypeDef,
+    ListClusterJobsRequestListClusterJobsPaginateTypeDef,
+    ListClustersRequestListClustersPaginateTypeDef,
+    ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListLongTermPricingRequestListLongTermPricingPaginateTypeDef,
+    LambdaResourceOutputTypeDef,
     LambdaResourceTypeDef,
     TaxDocumentsTypeDef,
     ListLongTermPricingResultTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    S3ResourceOutputTypeDef,
     S3ResourceTypeDef,
     ShippingDetailsTypeDef,
     SnowconeDeviceConfigurationTypeDef,
     ListServiceVersionsRequestRequestTypeDef,
     ListServiceVersionsResultTypeDef,
+    JobResourceOutputTypeDef,
     JobResourceTypeDef,
     DeviceConfigurationTypeDef,
     ClusterMetadataTypeDef,
     CreateClusterRequestRequestTypeDef,
+    JobResourceUnionTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateJobRequestRequestTypeDef,
     CreateJobRequestRequestTypeDef,
     JobMetadataTypeDef,
     DescribeClusterResultTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-snowball-2.5.2/types_aiobotocore_snowball.egg-info/SOURCES.txt` & `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*


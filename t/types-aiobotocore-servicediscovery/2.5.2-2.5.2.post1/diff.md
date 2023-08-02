# Comparing `tmp/types-aiobotocore-servicediscovery-2.5.2.tar.gz` & `tmp/types-aiobotocore-servicediscovery-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicediscovery-2.5.2.tar", last modified: Sat Jul  8 01:44:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicediscovery-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:00 2023, max compression
```

## Comparing `types-aiobotocore-servicediscovery-2.5.2.tar` & `types-aiobotocore-servicediscovery-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.370899 types-aiobotocore-servicediscovery-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17499 2023-07-08 01:44:19.370899 types-aiobotocore-servicediscovery-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:19.370899 types-aiobotocore-servicediscovery-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.362898 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24510 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28492 2023-07-08 01:41:00.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28456 2023-07-08 01:41:00.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:59.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.370899 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17499 2023-07-08 01:44:19.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:44:19.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:19.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:44:19.000000 types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.733458 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24559 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-08-02 14:49:40.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28990 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:36.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.737458 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:53:00.000000 types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/LICENSE` & `types-aiobotocore-servicediscovery-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2/PKG-INFO` & `types-aiobotocore-servicediscovery-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicediscovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore servicediscovery type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicediscovery?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicediscovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceDiscovery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
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
@@ -332,94 +331,96 @@
 )
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicediscovery.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_servicediscovery.type_defs import (
     TagTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
-    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
     SOATypeDef,
-    EmptyResponseMetadataTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     SOAChangeTypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    RegisterInstanceResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DeregisterInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterInstanceResponseTypeDef,
+    UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
+    DnsConfigOutputTypeDef,
     DnsConfigTypeDef,
     DnsPropertiesTypeDef,
     PrivateDnsPropertiesMutableTypeDef,
     PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
     ServiceChangeTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    DnsConfigUnionTypeDef,
     NamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
@@ -434,15 +435,15 @@
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/README.md` & `types-aiobotocore-servicediscovery-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicediscovery?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicediscovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceDiscovery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
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
@@ -299,94 +299,96 @@
 )
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicediscovery.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_servicediscovery.type_defs import (
     TagTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
-    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
     SOATypeDef,
-    EmptyResponseMetadataTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     SOAChangeTypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    RegisterInstanceResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DeregisterInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterInstanceResponseTypeDef,
+    UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
+    DnsConfigOutputTypeDef,
     DnsConfigTypeDef,
     DnsPropertiesTypeDef,
     PrivateDnsPropertiesMutableTypeDef,
     PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
     ServiceChangeTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    DnsConfigUnionTypeDef,
     NamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
@@ -401,15 +403,15 @@
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/setup.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicediscovery",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with"
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
-    keywords="aiobotocore servicediscovery type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore servicediscovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_servicediscovery": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/"
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/__init__.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/__init__.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/__main__.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceDiscovery 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ServiceDiscovery 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/client.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     CreateServiceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
-    DnsConfigTypeDef,
+    DnsConfigUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstanceResponseTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceResponseTypeDef,
     GetOperationResponseTypeDef,
     GetServiceResponseTypeDef,
     HealthCheckConfigTypeDef,
@@ -186,15 +186,15 @@
     async def create_service(
         self,
         *,
         Name: str,
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        DnsConfig: DnsConfigTypeDef = ...,
+        DnsConfig: DnsConfigUnionTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: Literal["HTTP"] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/client.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     CreateServiceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
-    DnsConfigTypeDef,
+    DnsConfigUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstanceResponseTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceResponseTypeDef,
     GetOperationResponseTypeDef,
     GetServiceResponseTypeDef,
     HealthCheckConfigTypeDef,
@@ -176,15 +176,15 @@
     async def create_service(
         self,
         *,
         Name: str,
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        DnsConfig: DnsConfigTypeDef = ...,
+        DnsConfig: DnsConfigUnionTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: Literal["HTTP"] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/literals.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/literals.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/paginator.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 class ListInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, ServiceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listinstancespaginator)
         """
 
 
@@ -81,15 +81,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 
@@ -99,15 +99,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
         """
 
 
@@ -117,13 +117,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/paginator.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 class ListInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, ServiceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listinstancespaginator)
         """
 
 class ListNamespacesPaginator(AioPaginator):
@@ -77,15 +77,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[NamespaceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListNamespaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listnamespacespaginator)
         """
 
 class ListOperationsPaginator(AioPaginator):
@@ -94,15 +94,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OperationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listoperationspaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
@@ -111,13 +111,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ServiceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/type_defs.py` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CustomHealthStatusType,
     FilterConditionType,
     HealthCheckTypeType,
     HealthStatusFilterType,
     HealthStatusType,
@@ -40,84 +40,86 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "CreateHttpNamespaceResponseTypeDef",
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    "CreatePublicDnsNamespaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
-    "DeregisterInstanceResponseTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
     "SOATypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
-    "GetInstancesHealthStatusResponseTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "SOAChangeTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
-    "RegisterInstanceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateHttpNamespaceResponseTypeDef",
     "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+    "CreateHttpNamespaceRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateHttpNamespaceResponseTypeDef",
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    "CreatePublicDnsNamespaceResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DeregisterInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetInstancesHealthStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterInstanceResponseTypeDef",
+    "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
-    "CreateHttpNamespaceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
+    "DnsConfigOutputTypeDef",
     "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
     "PrivateDnsPropertiesMutableTypeDef",
     "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
     "ServiceChangeTypeDef",
-    "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
+    "CreateServiceRequestRequestTypeDef",
+    "DnsConfigUnionTypeDef",
     "NamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
@@ -139,35 +141,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateHttpNamespaceResponseTypeDef = TypedDict(
-    "CreateHttpNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePublicDnsNamespaceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -200,22 +189,14 @@
 DeleteNamespaceRequestRequestTypeDef = TypedDict(
     "DeleteNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -223,22 +204,14 @@
     "DeregisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
 
-DeregisterInstanceResponseTypeDef = TypedDict(
-    "DeregisterInstanceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDiscoverInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDiscoverInstancesRequestRequestTypeDef",
     {
         "NamespaceName": str,
         "ServiceName": str,
     },
 )
@@ -283,21 +256,14 @@
 SOATypeDef = TypedDict(
     "SOATypeDef",
     {
         "TTL": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
@@ -342,23 +308,14 @@
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
 
-GetInstancesHealthStatusResponseTypeDef = TypedDict(
-    "GetInstancesHealthStatusResponseTypeDef",
-    {
-        "Status": Dict[str, HealthStatusType],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -411,36 +368,24 @@
     {
         "Id": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "ServiceId": str,
-    },
-)
-_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
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
-class ListInstancesRequestListInstancesPaginateTypeDef(
-    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
-    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstancesRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalListInstancesRequestRequestTypeDef = TypedDict(
@@ -531,24 +476,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
@@ -571,137 +506,202 @@
 
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
 
-RegisterInstanceResponseTypeDef = TypedDict(
-    "RegisterInstanceResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceId": str,
+        "InstanceId": str,
+        "Status": CustomHealthStatusType,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateHttpNamespaceRequestRequestTypeDef(
+    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
+    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
+):
+    pass
+
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-UpdateHttpNamespaceResponseTypeDef = TypedDict(
-    "UpdateHttpNamespaceResponseTypeDef",
+CreateHttpNamespaceResponseTypeDef = TypedDict(
+    "CreateHttpNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePrivateDnsNamespaceResponseTypeDef",
     {
-        "ServiceId": str,
-        "InstanceId": str,
-        "Status": CustomHealthStatusType,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePrivateDnsNamespaceResponseTypeDef",
+CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePublicDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePublicDnsNamespaceResponseTypeDef",
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+DeregisterInstanceResponseTypeDef = TypedDict(
+    "DeregisterInstanceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+
+GetInstancesHealthStatusResponseTypeDef = TypedDict(
+    "GetInstancesHealthStatusResponseTypeDef",
     {
-        "CreatorRequestId": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "Status": Dict[str, HealthStatusType],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateHttpNamespaceRequestRequestTypeDef(
-    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
-    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
-):
-    pass
-
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+RegisterInstanceResponseTypeDef = TypedDict(
+    "RegisterInstanceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateHttpNamespaceResponseTypeDef = TypedDict(
+    "UpdateHttpNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePrivateDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePublicDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DiscoverInstancesResponseTypeDef = TypedDict(
     "DiscoverInstancesResponseTypeDef",
     {
         "Instances": List[HttpInstanceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 
+_RequiredDnsConfigOutputTypeDef = TypedDict(
+    "_RequiredDnsConfigOutputTypeDef",
+    {
+        "DnsRecords": List[DnsRecordTypeDef],
+    },
+)
+_OptionalDnsConfigOutputTypeDef = TypedDict(
+    "_OptionalDnsConfigOutputTypeDef",
+    {
+        "NamespaceId": str,
+        "RoutingPolicy": RoutingPolicyType,
+    },
+    total=False,
+)
+
+
+class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
+    pass
+
+
 _RequiredDnsConfigTypeDef = TypedDict(
     "_RequiredDnsConfigTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 _OptionalDnsConfigTypeDef = TypedDict(
@@ -741,23 +741,23 @@
     },
 )
 
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationResponseTypeDef = TypedDict(
     "GetOperationResponseTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateHttpNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -781,23 +781,45 @@
 
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "ServiceId": str,
     },
 )
+_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstancesRequestListInstancesPaginateTypeDef(
+    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
+    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
+):
+    pass
+
 
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
@@ -808,15 +830,15 @@
     total=False,
 )
 
 ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsRequestListOperationsPaginateTypeDef",
     {
         "Filters": Sequence[OperationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
@@ -828,23 +850,23 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "Filters": Sequence[ServiceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
@@ -875,52 +897,24 @@
         "Description": str,
         "DnsConfig": DnsConfigChangeTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
-    {
-        "NamespaceId": str,
-        "CreatorRequestId": str,
-        "Description": str,
-        "DnsConfig": DnsConfigTypeDef,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "Type": Literal["HTTP"],
-    },
-    total=False,
-)
-
-
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
-
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": ServiceTypeType,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
     },
     total=False,
 )
 
@@ -929,24 +923,53 @@
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "NamespaceId": str,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
         "Type": ServiceTypeType,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
+    {
+        "NamespaceId": str,
+        "CreatorRequestId": str,
+        "Description": str,
+        "DnsConfig": DnsConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "Type": Literal["HTTP"],
+    },
+    total=False,
+)
+
+
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
+    pass
+
+
+DnsConfigUnionTypeDef = Union[DnsConfigTypeDef, DnsConfigOutputTypeDef]
 NamespacePropertiesTypeDef = TypedDict(
     "NamespacePropertiesTypeDef",
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
@@ -989,31 +1012,31 @@
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "Services": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NamespaceSummaryTypeDef = TypedDict(
     "NamespaceSummaryTypeDef",
     {
         "Id": str,
@@ -1114,23 +1137,23 @@
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "Namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery/type_defs.pyi` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_servicediscovery.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CustomHealthStatusType,
     FilterConditionType,
     HealthCheckTypeType,
     HealthStatusFilterType,
     HealthStatusType,
@@ -39,84 +39,86 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "CreateHttpNamespaceResponseTypeDef",
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    "CreatePublicDnsNamespaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "HealthCheckConfigTypeDef",
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
-    "DeregisterInstanceResponseTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
     "SOATypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
-    "GetInstancesHealthStatusResponseTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "SOAChangeTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
-    "RegisterInstanceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateHttpNamespaceResponseTypeDef",
     "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+    "CreateHttpNamespaceRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "CreateHttpNamespaceResponseTypeDef",
+    "CreatePrivateDnsNamespaceResponseTypeDef",
+    "CreatePublicDnsNamespaceResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DeregisterInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetInstancesHealthStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterInstanceResponseTypeDef",
+    "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
-    "CreateHttpNamespaceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
+    "DnsConfigOutputTypeDef",
     "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
     "PrivateDnsPropertiesMutableTypeDef",
     "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
     "ServiceChangeTypeDef",
-    "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
+    "CreateServiceRequestRequestTypeDef",
+    "DnsConfigUnionTypeDef",
     "NamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
@@ -138,35 +140,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateHttpNamespaceResponseTypeDef = TypedDict(
-    "CreateHttpNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePrivateDnsNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "CreatePublicDnsNamespaceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
@@ -197,22 +186,14 @@
 DeleteNamespaceRequestRequestTypeDef = TypedDict(
     "DeleteNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -220,22 +201,14 @@
     "DeregisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
 
-DeregisterInstanceResponseTypeDef = TypedDict(
-    "DeregisterInstanceResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDiscoverInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredDiscoverInstancesRequestRequestTypeDef",
     {
         "NamespaceName": str,
         "ServiceName": str,
     },
 )
@@ -278,21 +251,14 @@
 SOATypeDef = TypedDict(
     "SOATypeDef",
     {
         "TTL": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
     },
 )
@@ -333,23 +299,14 @@
 
 class GetInstancesHealthStatusRequestRequestTypeDef(
     _RequiredGetInstancesHealthStatusRequestRequestTypeDef,
     _OptionalGetInstancesHealthStatusRequestRequestTypeDef,
 ):
     pass
 
-GetInstancesHealthStatusResponseTypeDef = TypedDict(
-    "GetInstancesHealthStatusResponseTypeDef",
-    {
-        "Status": Dict[str, HealthStatusType],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetNamespaceRequestRequestTypeDef = TypedDict(
     "GetNamespaceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -402,34 +359,24 @@
     {
         "Id": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "ServiceId": str,
-    },
-)
-_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
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
 
-class ListInstancesRequestListInstancesPaginateTypeDef(
-    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
-    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
-):
-    pass
-
 _RequiredListInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredListInstancesRequestRequestTypeDef",
     {
         "ServiceId": str,
     },
 )
 _OptionalListInstancesRequestRequestTypeDef = TypedDict(
@@ -512,24 +459,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
@@ -550,135 +487,198 @@
 )
 
 class RegisterInstanceRequestRequestTypeDef(
     _RequiredRegisterInstanceRequestRequestTypeDef, _OptionalRegisterInstanceRequestRequestTypeDef
 ):
     pass
 
-RegisterInstanceResponseTypeDef = TypedDict(
-    "RegisterInstanceResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
+    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ServiceId": str,
+        "InstanceId": str,
+        "Status": CustomHealthStatusType,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateHttpNamespaceRequestRequestTypeDef(
+    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
+    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
+):
+    pass
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-UpdateHttpNamespaceResponseTypeDef = TypedDict(
-    "UpdateHttpNamespaceResponseTypeDef",
+CreateHttpNamespaceResponseTypeDef = TypedDict(
+    "CreateHttpNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateInstanceCustomHealthStatusRequestRequestTypeDef = TypedDict(
-    "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
+CreatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePrivateDnsNamespaceResponseTypeDef",
     {
-        "ServiceId": str,
-        "InstanceId": str,
-        "Status": CustomHealthStatusType,
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePrivateDnsNamespaceResponseTypeDef",
+CreatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "CreatePublicDnsNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
-    "UpdatePublicDnsNamespaceResponseTypeDef",
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+DeregisterInstanceResponseTypeDef = TypedDict(
+    "DeregisterInstanceResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHttpNamespaceRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateHttpNamespaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHttpNamespaceRequestRequestTypeDef",
+
+GetInstancesHealthStatusResponseTypeDef = TypedDict(
+    "GetInstancesHealthStatusResponseTypeDef",
     {
-        "CreatorRequestId": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "Status": Dict[str, HealthStatusType],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateHttpNamespaceRequestRequestTypeDef(
-    _RequiredCreateHttpNamespaceRequestRequestTypeDef,
-    _OptionalCreateHttpNamespaceRequestRequestTypeDef,
-):
-    pass
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+RegisterInstanceResponseTypeDef = TypedDict(
+    "RegisterInstanceResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateHttpNamespaceResponseTypeDef = TypedDict(
+    "UpdateHttpNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePrivateDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePrivateDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePublicDnsNamespaceResponseTypeDef = TypedDict(
+    "UpdatePublicDnsNamespaceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DiscoverInstancesResponseTypeDef = TypedDict(
     "DiscoverInstancesResponseTypeDef",
     {
         "Instances": List[HttpInstanceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 
+_RequiredDnsConfigOutputTypeDef = TypedDict(
+    "_RequiredDnsConfigOutputTypeDef",
+    {
+        "DnsRecords": List[DnsRecordTypeDef],
+    },
+)
+_OptionalDnsConfigOutputTypeDef = TypedDict(
+    "_OptionalDnsConfigOutputTypeDef",
+    {
+        "NamespaceId": str,
+        "RoutingPolicy": RoutingPolicyType,
+    },
+    total=False,
+)
+
+class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
+    pass
+
 _RequiredDnsConfigTypeDef = TypedDict(
     "_RequiredDnsConfigTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 _OptionalDnsConfigTypeDef = TypedDict(
@@ -716,23 +716,23 @@
     },
 )
 
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationResponseTypeDef = TypedDict(
     "GetOperationResponseTypeDef",
     {
         "Operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateHttpNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHttpNamespaceRequestRequestTypeDef",
     {
         "Id": str,
@@ -754,23 +754,43 @@
     pass
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "ServiceId": str,
+    },
+)
+_OptionalListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstancesRequestListInstancesPaginateTypeDef(
+    _RequiredListInstancesRequestListInstancesPaginateTypeDef,
+    _OptionalListInstancesRequestListInstancesPaginateTypeDef,
+):
+    pass
+
 ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "Filters": Sequence[NamespaceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
@@ -781,15 +801,15 @@
     total=False,
 )
 
 ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
     "ListOperationsRequestListOperationsPaginateTypeDef",
     {
         "Filters": Sequence[OperationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
@@ -801,23 +821,23 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "Filters": Sequence[ServiceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
@@ -848,50 +868,24 @@
         "Description": str,
         "DnsConfig": DnsConfigChangeTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
-    {
-        "NamespaceId": str,
-        "CreatorRequestId": str,
-        "Description": str,
-        "DnsConfig": DnsConfigTypeDef,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "Type": Literal["HTTP"],
-    },
-    total=False,
-)
-
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "Type": ServiceTypeType,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
     },
     total=False,
 )
 
@@ -900,24 +894,51 @@
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "NamespaceId": str,
         "Description": str,
         "InstanceCount": int,
-        "DnsConfig": DnsConfigTypeDef,
+        "DnsConfig": DnsConfigOutputTypeDef,
         "Type": ServiceTypeType,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
+    {
+        "NamespaceId": str,
+        "CreatorRequestId": str,
+        "Description": str,
+        "DnsConfig": DnsConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "Type": Literal["HTTP"],
+    },
+    total=False,
+)
+
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
+    pass
+
+DnsConfigUnionTypeDef = Union[DnsConfigTypeDef, DnsConfigOutputTypeDef]
 NamespacePropertiesTypeDef = TypedDict(
     "NamespacePropertiesTypeDef",
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
@@ -960,31 +981,31 @@
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "Services": List[ServiceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NamespaceSummaryTypeDef = TypedDict(
     "NamespaceSummaryTypeDef",
     {
         "Id": str,
@@ -1081,23 +1102,23 @@
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "Namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Id": str,
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/PKG-INFO` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicediscovery
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServiceDiscovery 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicediscovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore servicediscovery type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicediscovery"></a>
 
 # types-aiobotocore-servicediscovery
 
 [![PyPI - types-aiobotocore-servicediscovery](https://img.shields.io/pypi/v/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicediscovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicediscovery?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicediscovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicediscovery)](https://pepy.tech/project/types-aiobotocore-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceDiscovery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [types-aiobotocore-servicediscovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicediscovery/).
 
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
@@ -332,94 +331,96 @@
 )
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicediscovery.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_servicediscovery.type_defs import (
     TagTypeDef,
-    CreateHttpNamespaceResponseTypeDef,
-    CreatePrivateDnsNamespaceResponseTypeDef,
-    CreatePublicDnsNamespaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
-    DeregisterInstanceResponseTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
     SOATypeDef,
-    EmptyResponseMetadataTypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
-    GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     SOAChangeTypeDef,
     RegisterInstanceRequestRequestTypeDef,
-    RegisterInstanceResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateHttpNamespaceResponseTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
+    CreateHttpNamespaceRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
+    CreateHttpNamespaceResponseTypeDef,
+    CreatePrivateDnsNamespaceResponseTypeDef,
+    CreatePublicDnsNamespaceResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DeregisterInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetInstancesHealthStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterInstanceResponseTypeDef,
+    UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
-    CreateHttpNamespaceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
+    DnsConfigOutputTypeDef,
     DnsConfigTypeDef,
     DnsPropertiesTypeDef,
     PrivateDnsPropertiesMutableTypeDef,
     PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
     ServiceChangeTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
+    DnsConfigUnionTypeDef,
     NamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
@@ -434,15 +435,15 @@
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicediscovery-2.5.2/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt` & `types-aiobotocore-servicediscovery-2.5.2.post1/types_aiobotocore_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*


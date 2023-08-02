# Comparing `tmp/types-aiobotocore-service-quotas-2.5.2.tar.gz` & `tmp/types-aiobotocore-service-quotas-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-service-quotas-2.5.2.tar", last modified: Sat Jul  8 01:44:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-service-quotas-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
```

## Comparing `types-aiobotocore-service-quotas-2.5.2.tar` & `types-aiobotocore-service-quotas-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.514889 types-aiobotocore-service-quotas-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:50.000000 types-aiobotocore-service-quotas-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-07-08 01:44:18.514889 types-aiobotocore-service-quotas-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-07-08 01:40:50.000000 types-aiobotocore-service-quotas-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:18.514889 types-aiobotocore-service-quotas-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:40:50.000000 types-aiobotocore-service-quotas-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.506888 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-08 01:40:50.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-08 01:40:50.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-07-08 01:40:51.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:50.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.514889 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-07-08 01:44:18.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:18.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:18.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:18.000000 types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.901461 types-aiobotocore-service-quotas-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-08-02 14:52:59.897461 types-aiobotocore-service-quotas-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.901461 types-aiobotocore-service-quotas-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.897461 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-08-02 14:49:31.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-08-02 14:49:31.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:30.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.897461 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:59.000000 types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/LICENSE` & `types-aiobotocore-service-quotas-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/PKG-INFO` & `types-aiobotocore-service-quotas-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore service-quotas type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore service-quotas type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-service-quotas?color=blue)](https://pypistats.org/packages/types-aiobotocore-service-quotas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceQuotas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
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
@@ -336,73 +335,73 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_service_quotas.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MetricInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
+def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/README.md` & `types-aiobotocore-service-quotas-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-service-quotas?color=blue)](https://pypistats.org/packages/types-aiobotocore-service-quotas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceQuotas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
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
@@ -303,73 +303,73 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_service_quotas.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MetricInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
+def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/setup.py` & `types-aiobotocore-service-quotas-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-service-quotas",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with"
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
-    keywords="aiobotocore service-quotas type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore service-quotas type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_service_quotas": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/"
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/__init__.py` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/__init__.pyi` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/__main__.py` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ServiceQuotas 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ServiceQuotas 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas\nOther"
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

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/client.py` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/client.pyi` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/literals.py` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/literals.pyi` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/paginator.py` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 class ListAWSDefaultServiceQuotasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAWSDefaultServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
         """
 
 
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
 
@@ -108,15 +108,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
 
@@ -127,43 +127,43 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
 
 class ListServiceQuotasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaspaginator)
         """
 
 
 class ListServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/paginator.pyi` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 class ListAWSDefaultServiceQuotasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAWSDefaultServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
         """
 
 class ListRequestedServiceQuotaChangeHistoryPaginator(AioPaginator):
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
 class ListRequestedServiceQuotaChangeHistoryByQuotaPaginator(AioPaginator):
@@ -103,15 +103,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
 class ListServiceQuotaIncreaseRequestsInTemplatePaginator(AioPaginator):
@@ -121,41 +121,41 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
 class ListServiceQuotasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicequotaspaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/paginators/#listservicespaginator)
         """
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/type_defs.py` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_service_quotas.type_defs import DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef
 
-    data: DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = {...}
+    data: DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -28,49 +28,49 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "RequestedServiceQuotaChangeTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ServiceQuotaIncreaseRequestInTemplateTypeDef",
     "GetServiceQuotaRequestRequestTypeDef",
-    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAWSDefaultServiceQuotasRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
-    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MetricInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
+    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ServiceQuotaTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
@@ -99,19 +99,22 @@
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetRequestedServiceQuotaChangeRequestRequestTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     {
         "RequestId": str,
@@ -167,36 +170,24 @@
     "GetServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
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
-class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
-    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -212,38 +203,14 @@
 class ListAWSDefaultServiceQuotasRequestRequestTypeDef(
     _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef,
     _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "QuotaCode": str,
-    },
-)
-_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
-    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = TypedDict(
     "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
@@ -261,78 +228,36 @@
 class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(
     _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
 ):
     pass
 
 
-ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "Status": RequestStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AwsRegion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AwsRegion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
-    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -347,22 +272,14 @@
 
 class ListServiceQuotasRequestRequestTypeDef(
     _RequiredListServiceQuotasRequestRequestTypeDef, _OptionalListServiceQuotasRequestRequestTypeDef
 ):
     pass
 
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -399,24 +316,14 @@
         "MetricName": str,
         "MetricDimensions": Dict[str, str],
         "MetricStatisticRecommendation": str,
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
 PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     {
         "QuotaCode": str,
         "ServiceCode": str,
         "AwsRegion": str,
         "DesiredValue": float,
@@ -437,108 +344,201 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    {
+        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRequestedServiceQuotaChangeResponseTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestServiceQuotaIncreaseResponseTypeDef = TypedDict(
     "RequestServiceQuotaIncreaseResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef = TypedDict(
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplateList": List[
             ServiceQuotaIncreaseRequestInTemplateTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
+    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "QuotaCode": str,
+    },
+)
+_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
+    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+):
+    pass
+
+
+ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AwsRegion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
+    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+):
+    pass
+
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "Services": List[ServiceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
         "ResourceARN": str,
@@ -565,36 +565,36 @@
     total=False,
 )
 
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaResponseTypeDef = TypedDict(
     "GetServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAWSDefaultServiceQuotasResponseTypeDef = TypedDict(
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotasResponseTypeDef = TypedDict(
     "ListServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas/type_defs.pyi` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_service_quotas.type_defs import DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef
 
-    data: DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = {...}
+    data: DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -27,49 +27,49 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "RequestedServiceQuotaChangeTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ServiceQuotaIncreaseRequestInTemplateTypeDef",
     "GetServiceQuotaRequestRequestTypeDef",
-    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAWSDefaultServiceQuotasRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
-    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "MetricInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
+    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ServiceQuotaTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
@@ -98,19 +98,22 @@
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetRequestedServiceQuotaChangeRequestRequestTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     {
         "RequestId": str,
@@ -166,34 +169,24 @@
     "GetServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
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
 
-class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
-    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-):
-    pass
-
 _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -207,36 +200,14 @@
 
 class ListAWSDefaultServiceQuotasRequestRequestTypeDef(
     _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef,
     _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "QuotaCode": str,
-    },
-)
-_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
-    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-):
-    pass
-
 _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = TypedDict(
     "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
@@ -252,76 +223,36 @@
 
 class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(
     _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
 ):
     pass
 
-ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "Status": RequestStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AwsRegion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AwsRegion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
-    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-):
-    pass
-
 _RequiredListServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -334,22 +265,14 @@
 )
 
 class ListServiceQuotasRequestRequestTypeDef(
     _RequiredListServiceQuotasRequestRequestTypeDef, _OptionalListServiceQuotasRequestRequestTypeDef
 ):
     pass
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -386,24 +309,14 @@
         "MetricName": str,
         "MetricDimensions": Dict[str, str],
         "MetricStatisticRecommendation": str,
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
 PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     {
         "QuotaCode": str,
         "ServiceCode": str,
         "AwsRegion": str,
         "DesiredValue": float,
@@ -424,108 +337,195 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    {
+        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRequestedServiceQuotaChangeResponseTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestServiceQuotaIncreaseResponseTypeDef = TypedDict(
     "RequestServiceQuotaIncreaseResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef = TypedDict(
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplateList": List[
             ServiceQuotaIncreaseRequestInTemplateTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
+    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+):
+    pass
+
+_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "QuotaCode": str,
+    },
+)
+_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
+    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+):
+    pass
+
+ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AwsRegion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
+    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+):
+    pass
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "Services": List[ServiceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
         "ResourceARN": str,
@@ -552,36 +552,36 @@
     total=False,
 )
 
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaResponseTypeDef = TypedDict(
     "GetServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAWSDefaultServiceQuotasResponseTypeDef = TypedDict(
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotasResponseTypeDef = TypedDict(
     "ListServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/PKG-INFO` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-service-quotas
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ServiceQuotas 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore service-quotas type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore service-quotas type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-service-quotas"></a>
 
 # types-aiobotocore-service-quotas
 
 [![PyPI - types-aiobotocore-service-quotas](https://img.shields.io/pypi/v/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-service-quotas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-service-quotas?color=blue)](https://pypistats.org/packages/types-aiobotocore-service-quotas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-service-quotas)](https://pepy.tech/project/types-aiobotocore-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ServiceQuotas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [types-aiobotocore-service-quotas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_service_quotas/).
 
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
@@ -336,73 +335,73 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_service_quotas.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     MetricInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
+def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-service-quotas-2.5.2/types_aiobotocore_service_quotas.egg-info/SOURCES.txt` & `types-aiobotocore-service-quotas-2.5.2.post1/types_aiobotocore_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*


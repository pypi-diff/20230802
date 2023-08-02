# Comparing `tmp/types-aiobotocore-worklink-2.5.2.tar.gz` & `tmp/types-aiobotocore-worklink-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-worklink-2.5.2.tar", last modified: Sat Jul  8 01:44:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-worklink-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
```

## Comparing `types-aiobotocore-worklink-2.5.2.tar` & `types-aiobotocore-worklink-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.667055 types-aiobotocore-worklink-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-07-08 01:44:28.667055 types-aiobotocore-worklink-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:28.667055 types-aiobotocore-worklink-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.667055 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23792 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-08 01:42:41.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-08 01:42:41.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-07-08 01:42:41.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-07-08 01:42:41.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:40.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.667055 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-07-08 01:44:28.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:44:28.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:28.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:28.000000 types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.885425 types-aiobotocore-worklink-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-08-02 14:53:10.865425 types-aiobotocore-worklink-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.885425 types-aiobotocore-worklink-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.865425 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23792 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-02 14:51:19.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-08-02 14:51:19.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21206 2023-08-02 14:51:19.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.865425 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-worklink-2.5.2/LICENSE` & `types-aiobotocore-worklink-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2/PKG-INFO` & `types-aiobotocore-worklink-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-worklink
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore worklink type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore worklink type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-worklink"></a>
 
 # types-aiobotocore-worklink
 
 [![PyPI - types-aiobotocore-worklink](https://img.shields.io/pypi/v/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-worklink?color=blue)](https://pypistats.org/packages/types-aiobotocore-worklink)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkLink 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [types-aiobotocore-worklink docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/).
 
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
@@ -283,83 +282,83 @@
 )
 
 
 def check_value(value: AuthorizationProviderTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_worklink.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
-    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
-    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
+    DescribeDeviceResponseTypeDef,
+    DescribeDomainResponseTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDomainRequestRequestTypeDef:
+def get_value() -> AssociateDomainRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-worklink-2.5.2/README.md` & `types-aiobotocore-worklink-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-worklink"></a>
 
 # types-aiobotocore-worklink
 
 [![PyPI - types-aiobotocore-worklink](https://img.shields.io/pypi/v/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-worklink?color=blue)](https://pypistats.org/packages/types-aiobotocore-worklink)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkLink 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [types-aiobotocore-worklink docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/).
 
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
@@ -250,83 +250,83 @@
 )
 
 
 def check_value(value: AuthorizationProviderTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_worklink.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
-    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
-    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
+    DescribeDeviceResponseTypeDef,
+    DescribeDomainResponseTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDomainRequestRequestTypeDef:
+def get_value() -> AssociateDomainRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-worklink-2.5.2/setup.py` & `types-aiobotocore-worklink-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-worklink",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_worklink"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore worklink type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore worklink type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_worklink": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/"
```

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/__main__.py` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkLink 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WorkLink 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink\nOther"
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

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/client.py` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/client.pyi` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/literals.py` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/literals.pyi` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/type_defs.py` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_worklink.type_defs import AssociateDomainRequestRequestTypeDef
 
-    data: AssociateDomainRequestRequestTypeDef = {...}
+    data: AssociateDomainRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import DeviceStatusType, DomainStatusType, FleetStatusType
@@ -26,63 +26,63 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
-    "DescribeAuditStreamConfigurationResponseTypeDef",
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
-    "DescribeDeviceResponseTypeDef",
     "DescribeDomainRequestRequestTypeDef",
-    "DescribeDomainResponseTypeDef",
     "DescribeFleetMetadataRequestRequestTypeDef",
-    "DescribeFleetMetadataResponseTypeDef",
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
     "DeviceSummaryTypeDef",
     "DisassociateDomainRequestRequestTypeDef",
     "DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "FleetSummaryTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     "WebsiteAuthorizationProviderSummaryTypeDef",
     "ListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     "WebsiteCaSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDomainAccessRequestRequestTypeDef",
     "RevokeDomainAccessRequestRequestTypeDef",
     "SignOutUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuditStreamConfigurationRequestRequestTypeDef",
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     "UpdateDevicePolicyConfigurationRequestRequestTypeDef",
     "UpdateDomainMetadataRequestRequestTypeDef",
     "UpdateFleetMetadataRequestRequestTypeDef",
     "UpdateIdentityProviderConfigurationRequestRequestTypeDef",
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    "DescribeDeviceResponseTypeDef",
+    "DescribeDomainResponseTypeDef",
+    "DescribeFleetMetadataResponseTypeDef",
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
 )
 
@@ -128,19 +128,22 @@
 class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(
     _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     _OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AuthorizationProviderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
@@ -159,22 +162,14 @@
 class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(
     _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     _OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "WebsiteCaId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalCreateFleetRequestRequestTypeDef = TypedDict(
@@ -190,177 +185,80 @@
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "FleetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
 DescribeAuditStreamConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    {
-        "AuditStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDevicePolicyConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    {
-        "DeviceCaCertificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DeviceId": str,
     },
 )
 
-DescribeDeviceResponseTypeDef = TypedDict(
-    "DescribeDeviceResponseTypeDef",
-    {
-        "Status": DeviceStatusType,
-        "Model": str,
-        "Manufacturer": str,
-        "OperatingSystem": str,
-        "OperatingSystemVersion": str,
-        "PatchLevel": str,
-        "FirstAccessedTime": datetime,
-        "LastAccessedTime": datetime,
-        "Username": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
 
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DisplayName": str,
-        "CreatedTime": datetime,
-        "DomainStatus": DomainStatusType,
-        "AcmCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeFleetMetadataResponseTypeDef = TypedDict(
-    "DescribeFleetMetadataResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "FleetName": str,
-        "DisplayName": str,
-        "OptimizeForEndUserLocation": bool,
-        "CompanyCode": str,
-        "FleetStatus": FleetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    {
-        "IdentityProviderType": Literal["SAML"],
-        "ServiceProviderSamlMetadata": str,
-        "IdentityProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
         "WebsiteCaId": str,
     },
 )
 
-DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "Certificate": str,
-        "CreatedTime": datetime,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceId": str,
         "DeviceStatus": DeviceStatusType,
     },
     total=False,
@@ -482,22 +380,14 @@
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
 _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
@@ -570,25 +460,14 @@
         "WebsiteCaId": str,
         "CreatedTime": datetime,
         "DisplayName": str,
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
 RestoreDomainAccessRequestRequestTypeDef = TypedDict(
     "RestoreDomainAccessRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -744,51 +623,172 @@
 class UpdateIdentityProviderConfigurationRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    {
+        "AuthorizationProviderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "WebsiteCaId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "FleetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    {
+        "AuditStreamArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    {
+        "DeviceCaCertificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDeviceResponseTypeDef = TypedDict(
+    "DescribeDeviceResponseTypeDef",
+    {
+        "Status": DeviceStatusType,
+        "Model": str,
+        "Manufacturer": str,
+        "OperatingSystem": str,
+        "OperatingSystemVersion": str,
+        "PatchLevel": str,
+        "FirstAccessedTime": datetime,
+        "LastAccessedTime": datetime,
+        "Username": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DisplayName": str,
+        "CreatedTime": datetime,
+        "DomainStatus": DomainStatusType,
+        "AcmCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetadataResponseTypeDef = TypedDict(
+    "DescribeFleetMetadataResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "FleetName": str,
+        "DisplayName": str,
+        "OptimizeForEndUserLocation": bool,
+        "CompanyCode": str,
+        "FleetStatus": FleetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    {
+        "IdentityProviderType": Literal["SAML"],
+        "ServiceProviderSamlMetadata": str,
+        "IdentityProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "Certificate": str,
+        "CreatedTime": datetime,
+        "DisplayName": str,
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
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "FleetSummaryList": List[FleetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteAuthorizationProvidersResponseTypeDef = TypedDict(
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     {
         "WebsiteAuthorizationProviders": List[WebsiteAuthorizationProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
     {
         "WebsiteCertificateAuthorities": List[WebsiteCaSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink/type_defs.pyi` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_worklink.type_defs import AssociateDomainRequestRequestTypeDef
 
-    data: AssociateDomainRequestRequestTypeDef = {...}
+    data: AssociateDomainRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import DeviceStatusType, DomainStatusType, FleetStatusType
@@ -25,63 +25,63 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateDomainRequestRequestTypeDef",
     "AssociateWebsiteAuthorizationProviderRequestRequestTypeDef",
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
-    "DescribeAuditStreamConfigurationResponseTypeDef",
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
-    "DescribeDeviceResponseTypeDef",
     "DescribeDomainRequestRequestTypeDef",
-    "DescribeDomainResponseTypeDef",
     "DescribeFleetMetadataRequestRequestTypeDef",
-    "DescribeFleetMetadataResponseTypeDef",
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
     "DeviceSummaryTypeDef",
     "DisassociateDomainRequestRequestTypeDef",
     "DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef",
     "DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     "DomainSummaryTypeDef",
     "FleetSummaryTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFleetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     "WebsiteAuthorizationProviderSummaryTypeDef",
     "ListWebsiteCertificateAuthoritiesRequestRequestTypeDef",
     "WebsiteCaSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDomainAccessRequestRequestTypeDef",
     "RevokeDomainAccessRequestRequestTypeDef",
     "SignOutUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuditStreamConfigurationRequestRequestTypeDef",
     "UpdateCompanyNetworkConfigurationRequestRequestTypeDef",
     "UpdateDevicePolicyConfigurationRequestRequestTypeDef",
     "UpdateDomainMetadataRequestRequestTypeDef",
     "UpdateFleetMetadataRequestRequestTypeDef",
     "UpdateIdentityProviderConfigurationRequestRequestTypeDef",
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    "DescribeDeviceResponseTypeDef",
+    "DescribeDomainResponseTypeDef",
+    "DescribeFleetMetadataResponseTypeDef",
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
 )
 
@@ -123,19 +123,22 @@
 
 class AssociateWebsiteAuthorizationProviderRequestRequestTypeDef(
     _RequiredAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     _OptionalAssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
 ):
     pass
 
-AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
-    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AuthorizationProviderId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
@@ -152,22 +155,14 @@
 
 class AssociateWebsiteCertificateAuthorityRequestRequestTypeDef(
     _RequiredAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     _OptionalAssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "WebsiteCaId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFleetRequestRequestTypeDef",
     {
         "FleetName": str,
     },
 )
 _OptionalCreateFleetRequestRequestTypeDef = TypedDict(
@@ -181,177 +176,80 @@
 )
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "FleetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
 DescribeAuditStreamConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeAuditStreamConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
-    "DescribeAuditStreamConfigurationResponseTypeDef",
-    {
-        "AuditStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCompanyNetworkConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeCompanyNetworkConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
-    "DescribeCompanyNetworkConfigurationResponseTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDevicePolicyConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDevicePolicyConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
-    "DescribeDevicePolicyConfigurationResponseTypeDef",
-    {
-        "DeviceCaCertificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DeviceId": str,
     },
 )
 
-DescribeDeviceResponseTypeDef = TypedDict(
-    "DescribeDeviceResponseTypeDef",
-    {
-        "Status": DeviceStatusType,
-        "Model": str,
-        "Manufacturer": str,
-        "OperatingSystem": str,
-        "OperatingSystemVersion": str,
-        "PatchLevel": str,
-        "FirstAccessedTime": datetime,
-        "LastAccessedTime": datetime,
-        "Username": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainRequestRequestTypeDef = TypedDict(
     "DescribeDomainRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
 
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainName": str,
-        "DisplayName": str,
-        "CreatedTime": datetime,
-        "DomainStatus": DomainStatusType,
-        "AcmCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetadataRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetadataRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeFleetMetadataResponseTypeDef = TypedDict(
-    "DescribeFleetMetadataResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "FleetName": str,
-        "DisplayName": str,
-        "OptimizeForEndUserLocation": bool,
-        "CompanyCode": str,
-        "FleetStatus": FleetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeIdentityProviderConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeIdentityProviderConfigurationRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 
-DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
-    "DescribeIdentityProviderConfigurationResponseTypeDef",
-    {
-        "IdentityProviderType": Literal["SAML"],
-        "ServiceProviderSamlMetadata": str,
-        "IdentityProviderSamlMetadata": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWebsiteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeWebsiteCertificateAuthorityRequestRequestTypeDef",
     {
         "FleetArn": str,
         "WebsiteCaId": str,
     },
 )
 
-DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
-    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
-    {
-        "Certificate": str,
-        "CreatedTime": datetime,
-        "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "DeviceId": str,
         "DeviceStatus": DeviceStatusType,
     },
     total=False,
@@ -467,22 +365,14 @@
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
 _RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListWebsiteAuthorizationProvidersRequestRequestTypeDef",
     {
         "FleetArn": str,
     },
 )
 _OptionalListWebsiteAuthorizationProvidersRequestRequestTypeDef = TypedDict(
@@ -549,25 +439,14 @@
         "WebsiteCaId": str,
         "CreatedTime": datetime,
         "DisplayName": str,
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
 RestoreDomainAccessRequestRequestTypeDef = TypedDict(
     "RestoreDomainAccessRequestRequestTypeDef",
     {
         "FleetArn": str,
         "DomainName": str,
     },
 )
@@ -713,51 +592,172 @@
 
 class UpdateIdentityProviderConfigurationRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderConfigurationRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderConfigurationRequestRequestTypeDef,
 ):
     pass
 
+AssociateWebsiteAuthorizationProviderResponseTypeDef = TypedDict(
+    "AssociateWebsiteAuthorizationProviderResponseTypeDef",
+    {
+        "AuthorizationProviderId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "AssociateWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "WebsiteCaId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "FleetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAuditStreamConfigurationResponseTypeDef = TypedDict(
+    "DescribeAuditStreamConfigurationResponseTypeDef",
+    {
+        "AuditStreamArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCompanyNetworkConfigurationResponseTypeDef = TypedDict(
+    "DescribeCompanyNetworkConfigurationResponseTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "SecurityGroupIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDevicePolicyConfigurationResponseTypeDef = TypedDict(
+    "DescribeDevicePolicyConfigurationResponseTypeDef",
+    {
+        "DeviceCaCertificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDeviceResponseTypeDef = TypedDict(
+    "DescribeDeviceResponseTypeDef",
+    {
+        "Status": DeviceStatusType,
+        "Model": str,
+        "Manufacturer": str,
+        "OperatingSystem": str,
+        "OperatingSystemVersion": str,
+        "PatchLevel": str,
+        "FirstAccessedTime": datetime,
+        "LastAccessedTime": datetime,
+        "Username": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainName": str,
+        "DisplayName": str,
+        "CreatedTime": datetime,
+        "DomainStatus": DomainStatusType,
+        "AcmCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetadataResponseTypeDef = TypedDict(
+    "DescribeFleetMetadataResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "FleetName": str,
+        "DisplayName": str,
+        "OptimizeForEndUserLocation": bool,
+        "CompanyCode": str,
+        "FleetStatus": FleetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIdentityProviderConfigurationResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderConfigurationResponseTypeDef",
+    {
+        "IdentityProviderType": Literal["SAML"],
+        "ServiceProviderSamlMetadata": str,
+        "IdentityProviderSamlMetadata": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWebsiteCertificateAuthorityResponseTypeDef = TypedDict(
+    "DescribeWebsiteCertificateAuthorityResponseTypeDef",
+    {
+        "Certificate": str,
+        "CreatedTime": datetime,
+        "DisplayName": str,
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
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "FleetSummaryList": List[FleetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteAuthorizationProvidersResponseTypeDef = TypedDict(
     "ListWebsiteAuthorizationProvidersResponseTypeDef",
     {
         "WebsiteAuthorizationProviders": List[WebsiteAuthorizationProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWebsiteCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListWebsiteCertificateAuthoritiesResponseTypeDef",
     {
         "WebsiteCertificateAuthorities": List[WebsiteCaSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/PKG-INFO` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-worklink
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore worklink type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore worklink type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-worklink"></a>
 
 # types-aiobotocore-worklink
 
 [![PyPI - types-aiobotocore-worklink](https://img.shields.io/pypi/v/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-worklink.svg?color=blue)](https://pypi.org/project/types-aiobotocore-worklink)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-worklink?color=blue)](https://pypistats.org/packages/types-aiobotocore-worklink)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-worklink)](https://pepy.tech/project/types-aiobotocore-worklink)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkLink 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink)
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
 [types-aiobotocore-worklink docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink/).
 
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
@@ -283,83 +282,83 @@
 )
 
 
 def check_value(value: AuthorizationProviderTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_worklink.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_worklink.type_defs import (
     AssociateDomainRequestRequestTypeDef,
     AssociateWebsiteAuthorizationProviderRequestRequestTypeDef,
-    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateWebsiteCertificateAuthorityRequestRequestTypeDef,
-    AssociateWebsiteCertificateAuthorityResponseTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DescribeAuditStreamConfigurationRequestRequestTypeDef,
-    DescribeAuditStreamConfigurationResponseTypeDef,
     DescribeCompanyNetworkConfigurationRequestRequestTypeDef,
-    DescribeCompanyNetworkConfigurationResponseTypeDef,
     DescribeDevicePolicyConfigurationRequestRequestTypeDef,
-    DescribeDevicePolicyConfigurationResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
-    DescribeDeviceResponseTypeDef,
     DescribeDomainRequestRequestTypeDef,
-    DescribeDomainResponseTypeDef,
     DescribeFleetMetadataRequestRequestTypeDef,
-    DescribeFleetMetadataResponseTypeDef,
     DescribeIdentityProviderConfigurationRequestRequestTypeDef,
-    DescribeIdentityProviderConfigurationResponseTypeDef,
     DescribeWebsiteCertificateAuthorityRequestRequestTypeDef,
-    DescribeWebsiteCertificateAuthorityResponseTypeDef,
     DeviceSummaryTypeDef,
     DisassociateDomainRequestRequestTypeDef,
     DisassociateWebsiteAuthorizationProviderRequestRequestTypeDef,
     DisassociateWebsiteCertificateAuthorityRequestRequestTypeDef,
     DomainSummaryTypeDef,
     FleetSummaryTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFleetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWebsiteAuthorizationProvidersRequestRequestTypeDef,
     WebsiteAuthorizationProviderSummaryTypeDef,
     ListWebsiteCertificateAuthoritiesRequestRequestTypeDef,
     WebsiteCaSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDomainAccessRequestRequestTypeDef,
     RevokeDomainAccessRequestRequestTypeDef,
     SignOutUserRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuditStreamConfigurationRequestRequestTypeDef,
     UpdateCompanyNetworkConfigurationRequestRequestTypeDef,
     UpdateDevicePolicyConfigurationRequestRequestTypeDef,
     UpdateDomainMetadataRequestRequestTypeDef,
     UpdateFleetMetadataRequestRequestTypeDef,
     UpdateIdentityProviderConfigurationRequestRequestTypeDef,
+    AssociateWebsiteAuthorizationProviderResponseTypeDef,
+    AssociateWebsiteCertificateAuthorityResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    DescribeAuditStreamConfigurationResponseTypeDef,
+    DescribeCompanyNetworkConfigurationResponseTypeDef,
+    DescribeDevicePolicyConfigurationResponseTypeDef,
+    DescribeDeviceResponseTypeDef,
+    DescribeDomainResponseTypeDef,
+    DescribeFleetMetadataResponseTypeDef,
+    DescribeIdentityProviderConfigurationResponseTypeDef,
+    DescribeWebsiteCertificateAuthorityResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ListWebsiteAuthorizationProvidersResponseTypeDef,
     ListWebsiteCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDomainRequestRequestTypeDef:
+def get_value() -> AssociateDomainRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-worklink-2.5.2/types_aiobotocore_worklink.egg-info/SOURCES.txt` & `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/SOURCES.txt`

 * *Files identical despite different names*


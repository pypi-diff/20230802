# Comparing `tmp/types-aiobotocore-acm-pca-2.5.2.tar.gz` & `tmp/types-aiobotocore-acm-pca-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-pca-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-pca-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
```

## Comparing `types-aiobotocore-acm-pca-2.5.2.tar` & `types-aiobotocore-acm-pca-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24003 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23965 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27322 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:16.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-08 01:25:17.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.829605 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:09.000000 types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29793 2023-08-02 14:32:44.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29748 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/LICENSE` & `types-aiobotocore-acm-pca-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/PKG-INFO` & `types-aiobotocore-acm-pca-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm-pca
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore acm-pca type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore acm-pca type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-acm-pca"></a>
 
 # types-aiobotocore-acm-pca
 
 [![PyPI - types-aiobotocore-acm-pca](https://img.shields.io/pypi/v/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm-pca?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm-pca)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm-pca)](https://pepy.tech/project/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ACMPCA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [types-aiobotocore-acm-pca docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -368,25 +367,26 @@
 )
 
 
 def check_value(value: AccessMethodTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_acm_pca.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_acm_pca.type_defs import (
     CustomAttributeTypeDef,
     AccessMethodTypeDef,
+    BlobTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CrlConfigurationTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
@@ -399,27 +399,28 @@
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
+    ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
+    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
@@ -433,31 +434,36 @@
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
+    GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
+    AccessDescriptionOutputTypeDef,
     AccessDescriptionTypeDef,
     ExtensionsTypeDef,
+    CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_value() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/README.md` & `types-aiobotocore-acm-pca-2.5.2.post1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-acm-pca"></a>
 
 # types-aiobotocore-acm-pca
 
 [![PyPI - types-aiobotocore-acm-pca](https://img.shields.io/pypi/v/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm-pca?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm-pca)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm-pca)](https://pepy.tech/project/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ACMPCA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [types-aiobotocore-acm-pca docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -335,25 +335,26 @@
 )
 
 
 def check_value(value: AccessMethodTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_acm_pca.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_acm_pca.type_defs import (
     CustomAttributeTypeDef,
     AccessMethodTypeDef,
+    BlobTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CrlConfigurationTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
@@ -366,27 +367,28 @@
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
+    ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
+    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
@@ -400,31 +402,36 @@
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
+    GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
+    AccessDescriptionOutputTypeDef,
     AccessDescriptionTypeDef,
     ExtensionsTypeDef,
+    CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_value() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/setup.py` & `types-aiobotocore-acm-pca-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm-pca",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore acm-pca type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore acm-pca type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_acm_pca": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/"
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__init__.pyi` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/__main__.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACMPCA 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ACMPCA 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("acm-pca") as client:
         client: ACMPCAClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ActionTypeType,
     AuditReportResponseFormatType,
     CertificateAuthorityStatusType,
     CertificateAuthorityTypeType,
@@ -35,15 +34,16 @@
 from .paginator import (
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
-    CertificateAuthorityConfigurationTypeDef,
+    BlobTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -135,15 +135,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#close)
         """
 
     async def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
@@ -291,29 +291,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#get_policy)
         """
 
     async def import_certificate_authority_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...
+        Certificate: BlobTypeDef,
+        CertificateChain: BlobTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Imports a signed private CA certificate into Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.import_certificate_authority_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#import_certificate_authority_certificate)
         """
 
     async def issue_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Csr: Union[str, bytes, IO[Any], StreamingBody],
+        Csr: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmType,
         Validity: ValidityTypeDef,
         ApiPassthrough: ApiPassthroughTypeDef = ...,
         TemplateArn: str = ...,
         ValidityNotBefore: ValidityTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> IssueCertificateResponseTypeDef:
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/client.pyi` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("acm-pca") as client:
         client: ACMPCAClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ActionTypeType,
     AuditReportResponseFormatType,
     CertificateAuthorityStatusType,
     CertificateAuthorityTypeType,
@@ -35,15 +34,16 @@
 from .paginator import (
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
-    CertificateAuthorityConfigurationTypeDef,
+    BlobTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -128,15 +128,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#close)
         """
     async def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
@@ -271,28 +271,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.get_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#get_policy)
         """
     async def import_certificate_authority_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...
+        Certificate: BlobTypeDef,
+        CertificateChain: BlobTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Imports a signed private CA certificate into Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.import_certificate_authority_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#import_certificate_authority_certificate)
         """
     async def issue_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Csr: Union[str, bytes, IO[Any], StreamingBody],
+        Csr: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmType,
         Validity: ValidityTypeDef,
         ApiPassthrough: ApiPassthroughTypeDef = ...,
         TemplateArn: str = ...,
         ValidityNotBefore: ValidityTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> IssueCertificateResponseTypeDef:
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/literals.pyi` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/paginator.pyi` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_acm_pca.type_defs import CustomAttributeTypeDef
 
-    data: CustomAttributeTypeDef = {...}
+    data: CustomAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -45,14 +45,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CustomAttributeTypeDef",
     "AccessMethodTypeDef",
+    "BlobTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CrlConfigurationTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
@@ -65,27 +66,28 @@
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
+    "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
+    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
@@ -99,24 +101,29 @@
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
+    "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
+    "AccessDescriptionOutputTypeDef",
     "AccessDescriptionTypeDef",
     "ExtensionsTypeDef",
+    "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
+    "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
+    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
@@ -131,14 +138,15 @@
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateCertificateAuthorityAuditReportRequestRequestTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "S3BucketName": str,
         "AuditReportResponseFormat": AuditReportResponseFormatType,
     },
@@ -391,37 +399,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateAuthorityArn": str,
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
-    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
-):
-    pass
-
-
 ValidityTypeDef = TypedDict(
     "ValidityTypeDef",
     {
         "Value": int,
         "Type": ValidityPeriodTypeType,
     },
 )
@@ -551,14 +536,36 @@
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
 
+ASN1SubjectOutputTypeDef = TypedDict(
+    "ASN1SubjectOutputTypeDef",
+    {
+        "Country": str,
+        "Organization": str,
+        "OrganizationalUnit": str,
+        "DistinguishedNameQualifier": str,
+        "State": str,
+        "CommonName": str,
+        "SerialNumber": str,
+        "Locality": str,
+        "Title": str,
+        "Surname": str,
+        "GivenName": str,
+        "Initials": str,
+        "Pseudonym": str,
+        "GenerationQualifier": str,
+        "CustomAttributes": List[CustomAttributeTypeDef],
+    },
+    total=False,
+)
+
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
         "Country": str,
         "Organization": str,
         "OrganizationalUnit": str,
         "DistinguishedNameQualifier": str,
@@ -573,14 +580,37 @@
         "Pseudonym": str,
         "GenerationQualifier": str,
         "CustomAttributes": Sequence[CustomAttributeTypeDef],
     },
     total=False,
 )
 
+_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateAuthorityArn": str,
+        "Certificate": BlobTypeDef,
+    },
+)
+_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
+    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
+):
+    pass
+
+
 CreateCertificateAuthorityAuditReportResponseTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     {
         "AuditReportId": str,
         "S3Key": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -821,14 +851,29 @@
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
 
+GeneralNameOutputTypeDef = TypedDict(
+    "GeneralNameOutputTypeDef",
+    {
+        "OtherName": OtherNameTypeDef,
+        "Rfc822Name": str,
+        "DnsName": str,
+        "DirectoryName": ASN1SubjectOutputTypeDef,
+        "EdiPartyName": EdiPartyNameTypeDef,
+        "UniformResourceIdentifier": str,
+        "IpAddress": str,
+        "RegisteredId": str,
+    },
+    total=False,
+)
+
 GeneralNameTypeDef = TypedDict(
     "GeneralNameTypeDef",
     {
         "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectTypeDef,
@@ -880,14 +925,22 @@
 
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
 
+AccessDescriptionOutputTypeDef = TypedDict(
+    "AccessDescriptionOutputTypeDef",
+    {
+        "AccessMethod": AccessMethodTypeDef,
+        "AccessLocation": GeneralNameOutputTypeDef,
+    },
+)
+
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
     },
 )
@@ -900,14 +953,23 @@
         "KeyUsage": KeyUsageTypeDef,
         "SubjectAlternativeNames": Sequence[GeneralNameTypeDef],
         "CustomExtensions": Sequence[CustomExtensionTypeDef],
     },
     total=False,
 )
 
+CsrExtensionsOutputTypeDef = TypedDict(
+    "CsrExtensionsOutputTypeDef",
+    {
+        "KeyUsage": KeyUsageTypeDef,
+        "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
+    },
+    total=False,
+)
+
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": Sequence[AccessDescriptionTypeDef],
     },
     total=False,
@@ -918,14 +980,38 @@
     {
         "Extensions": ExtensionsTypeDef,
         "Subject": ASN1SubjectTypeDef,
     },
     total=False,
 )
 
+_RequiredCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "KeyAlgorithm": KeyAlgorithmType,
+        "SigningAlgorithm": SigningAlgorithmType,
+        "Subject": ASN1SubjectOutputTypeDef,
+    },
+)
+_OptionalCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "CsrExtensions": CsrExtensionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CertificateAuthorityConfigurationOutputTypeDef(
+    _RequiredCertificateAuthorityConfigurationOutputTypeDef,
+    _OptionalCertificateAuthorityConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -946,15 +1032,15 @@
     pass
 
 
 _RequiredIssueCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredIssueCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
-        "Csr": Union[str, bytes, IO[Any], StreamingBody],
+        "Csr": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmType,
         "Validity": ValidityTypeDef,
     },
 )
 _OptionalIssueCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalIssueCertificateRequestRequestTypeDef",
     {
@@ -982,23 +1068,26 @@
         "LastStateChangeAt": datetime,
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
-        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
+        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
+CertificateAuthorityConfigurationUnionTypeDef = Union[
+    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
+]
 _RequiredCreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
     },
 )
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/type_defs.pyi` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_acm_pca.type_defs import CustomAttributeTypeDef
 
-    data: CustomAttributeTypeDef = {...}
+    data: CustomAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -44,14 +44,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CustomAttributeTypeDef",
     "AccessMethodTypeDef",
+    "BlobTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CrlConfigurationTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
@@ -64,27 +65,28 @@
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
+    "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
+    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
@@ -98,24 +100,29 @@
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
+    "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
+    "AccessDescriptionOutputTypeDef",
     "AccessDescriptionTypeDef",
     "ExtensionsTypeDef",
+    "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
+    "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
+    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
@@ -130,14 +137,15 @@
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateCertificateAuthorityAuditReportRequestRequestTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "S3BucketName": str,
         "AuditReportResponseFormat": AuditReportResponseFormatType,
     },
@@ -376,35 +384,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateAuthorityArn": str,
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
-    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
-):
-    pass
-
 ValidityTypeDef = TypedDict(
     "ValidityTypeDef",
     {
         "Value": int,
         "Type": ValidityPeriodTypeType,
     },
 )
@@ -528,14 +515,36 @@
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
 
+ASN1SubjectOutputTypeDef = TypedDict(
+    "ASN1SubjectOutputTypeDef",
+    {
+        "Country": str,
+        "Organization": str,
+        "OrganizationalUnit": str,
+        "DistinguishedNameQualifier": str,
+        "State": str,
+        "CommonName": str,
+        "SerialNumber": str,
+        "Locality": str,
+        "Title": str,
+        "Surname": str,
+        "GivenName": str,
+        "Initials": str,
+        "Pseudonym": str,
+        "GenerationQualifier": str,
+        "CustomAttributes": List[CustomAttributeTypeDef],
+    },
+    total=False,
+)
+
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
         "Country": str,
         "Organization": str,
         "OrganizationalUnit": str,
         "DistinguishedNameQualifier": str,
@@ -550,14 +559,35 @@
         "Pseudonym": str,
         "GenerationQualifier": str,
         "CustomAttributes": Sequence[CustomAttributeTypeDef],
     },
     total=False,
 )
 
+_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateAuthorityArn": str,
+        "Certificate": BlobTypeDef,
+    },
+)
+_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": BlobTypeDef,
+    },
+    total=False,
+)
+
+class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
+    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
+):
+    pass
+
 CreateCertificateAuthorityAuditReportResponseTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     {
         "AuditReportId": str,
         "S3Key": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -788,14 +818,29 @@
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
 
+GeneralNameOutputTypeDef = TypedDict(
+    "GeneralNameOutputTypeDef",
+    {
+        "OtherName": OtherNameTypeDef,
+        "Rfc822Name": str,
+        "DnsName": str,
+        "DirectoryName": ASN1SubjectOutputTypeDef,
+        "EdiPartyName": EdiPartyNameTypeDef,
+        "UniformResourceIdentifier": str,
+        "IpAddress": str,
+        "RegisteredId": str,
+    },
+    total=False,
+)
+
 GeneralNameTypeDef = TypedDict(
     "GeneralNameTypeDef",
     {
         "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectTypeDef,
@@ -843,14 +888,22 @@
 )
 
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
+AccessDescriptionOutputTypeDef = TypedDict(
+    "AccessDescriptionOutputTypeDef",
+    {
+        "AccessMethod": AccessMethodTypeDef,
+        "AccessLocation": GeneralNameOutputTypeDef,
+    },
+)
+
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
     },
 )
@@ -863,14 +916,23 @@
         "KeyUsage": KeyUsageTypeDef,
         "SubjectAlternativeNames": Sequence[GeneralNameTypeDef],
         "CustomExtensions": Sequence[CustomExtensionTypeDef],
     },
     total=False,
 )
 
+CsrExtensionsOutputTypeDef = TypedDict(
+    "CsrExtensionsOutputTypeDef",
+    {
+        "KeyUsage": KeyUsageTypeDef,
+        "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
+    },
+    total=False,
+)
+
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": Sequence[AccessDescriptionTypeDef],
     },
     total=False,
@@ -881,14 +943,36 @@
     {
         "Extensions": ExtensionsTypeDef,
         "Subject": ASN1SubjectTypeDef,
     },
     total=False,
 )
 
+_RequiredCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "KeyAlgorithm": KeyAlgorithmType,
+        "SigningAlgorithm": SigningAlgorithmType,
+        "Subject": ASN1SubjectOutputTypeDef,
+    },
+)
+_OptionalCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "CsrExtensions": CsrExtensionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CertificateAuthorityConfigurationOutputTypeDef(
+    _RequiredCertificateAuthorityConfigurationOutputTypeDef,
+    _OptionalCertificateAuthorityConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -907,15 +991,15 @@
 ):
     pass
 
 _RequiredIssueCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredIssueCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
-        "Csr": Union[str, bytes, IO[Any], StreamingBody],
+        "Csr": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmType,
         "Validity": ValidityTypeDef,
     },
 )
 _OptionalIssueCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalIssueCertificateRequestRequestTypeDef",
     {
@@ -941,23 +1025,26 @@
         "LastStateChangeAt": datetime,
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
-        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
+        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
+CertificateAuthorityConfigurationUnionTypeDef = Union[
+    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
+]
 _RequiredCreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
     },
 )
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.py` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca/waiter.pyi` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/PKG-INFO` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm-pca
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore acm-pca type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore acm-pca type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-acm-pca"></a>
 
 # types-aiobotocore-acm-pca
 
 [![PyPI - types-aiobotocore-acm-pca](https://img.shields.io/pypi/v/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm-pca.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-acm-pca?color=blue)](https://pypistats.org/packages/types-aiobotocore-acm-pca)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm-pca)](https://pepy.tech/project/types-aiobotocore-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ACMPCA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [types-aiobotocore-acm-pca docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -368,25 +367,26 @@
 )
 
 
 def check_value(value: AccessMethodTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_acm_pca.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_acm_pca.type_defs import (
     CustomAttributeTypeDef,
     AccessMethodTypeDef,
+    BlobTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CrlConfigurationTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
@@ -399,27 +399,28 @@
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
+    ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
+    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
@@ -433,31 +434,36 @@
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
+    GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
+    AccessDescriptionOutputTypeDef,
     AccessDescriptionTypeDef,
     ExtensionsTypeDef,
+    CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_value() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-acm-pca-2.5.2/types_aiobotocore_acm_pca.egg-info/SOURCES.txt` & `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-outposts-2.5.2.tar.gz` & `tmp/types-aiobotocore-outposts-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-outposts-2.5.2.tar", last modified: Sat Jul  8 01:44:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-outposts-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
```

## Comparing `types-aiobotocore-outposts-2.5.2.tar` & `types-aiobotocore-outposts-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.102646 types-aiobotocore-outposts-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-08 01:44:05.098646 types-aiobotocore-outposts-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:05.102646 types-aiobotocore-outposts-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:36:13.000000 types-aiobotocore-outposts-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.090646 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20144 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21442 2023-07-08 01:36:16.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21423 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:14.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:05.098646 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-07-08 01:44:04.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:44:04.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:04.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:04.000000 types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.793503 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20144 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-08-02 14:44:32.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-08-02 14:44:32.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-08-02 14:44:34.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21379 2023-08-02 14:44:32.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:31.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.801504 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:45.000000 types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-outposts-2.5.2/LICENSE` & `types-aiobotocore-outposts-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.5.2/PKG-INFO` & `types-aiobotocore-outposts-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-outposts
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore outposts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore outposts type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-outposts"></a>
 
 # types-aiobotocore-outposts
 
 [![PyPI - types-aiobotocore-outposts](https://img.shields.io/pypi/v/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-outposts?color=blue)](https://pypistats.org/packages/types-aiobotocore-outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-outposts)](https://pepy.tech/project/types-aiobotocore-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Outposts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
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
@@ -302,30 +301,31 @@
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_outposts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_outposts.type_defs import (
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
@@ -340,30 +340,29 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
-    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
-    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    GetConnectionResponseTypeDef,
     CreateOrderInputRequestTypeDef,
+    GetConnectionResponseTypeDef,
+    GetSiteAddressOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartConnectionResponseTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
     SiteTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
@@ -379,15 +378,15 @@
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
     OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-outposts-2.5.2/README.md` & `types-aiobotocore-outposts-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-outposts"></a>
 
 # types-aiobotocore-outposts
 
 [![PyPI - types-aiobotocore-outposts](https://img.shields.io/pypi/v/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-outposts?color=blue)](https://pypistats.org/packages/types-aiobotocore-outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-outposts)](https://pepy.tech/project/types-aiobotocore-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Outposts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
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
@@ -269,30 +269,31 @@
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_outposts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_outposts.type_defs import (
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
@@ -307,30 +308,29 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
-    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
-    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    GetConnectionResponseTypeDef,
     CreateOrderInputRequestTypeDef,
+    GetConnectionResponseTypeDef,
+    GetSiteAddressOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartConnectionResponseTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
     SiteTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
@@ -346,15 +346,15 @@
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
     OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-outposts-2.5.2/setup.py` & `types-aiobotocore-outposts-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-outposts",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore outposts type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore outposts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_outposts": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/"
```

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/__main__.py` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Outposts 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Outposts 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
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

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/client.py` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/client.pyi` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/literals.py` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/literals.pyi` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/type_defs.py` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_outposts.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -45,23 +45,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
@@ -76,30 +76,29 @@
     "ListAssetsInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartConnectionRequestRequestTypeDef",
-    "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
-    "GetSiteAddressOutputTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
-    "UpdateSiteAddressOutputTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
-    "GetConnectionResponseTypeDef",
     "CreateOrderInputRequestTypeDef",
+    "GetConnectionResponseTypeDef",
+    "GetSiteAddressOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartConnectionResponseTypeDef",
+    "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
@@ -137,19 +136,17 @@
         "AddressLine3": str,
         "DistrictOrCounty": str,
         "Municipality": str,
     },
     total=False,
 )
 
-
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
-
 AssetLocationTypeDef = TypedDict(
     "AssetLocationTypeDef",
     {
         "RackElevation": float,
     },
     total=False,
 )
@@ -198,14 +195,25 @@
     {
         "CatalogItemId": str,
         "Quantity": int,
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
 _RequiredCreateOutpostInputRequestTypeDef = TypedDict(
     "_RequiredCreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
     },
 )
@@ -217,21 +225,19 @@
         "AvailabilityZoneId": str,
         "Tags": Mapping[str, str],
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
-
 class CreateOutpostInputRequestTypeDef(
     _RequiredCreateOutpostInputRequestTypeDef, _OptionalCreateOutpostInputRequestTypeDef
 ):
     pass
 
-
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "OutpostId": str,
         "OwnerId": str,
         "OutpostArn": str,
         "SiteId": str,
@@ -316,22 +322,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetOutpostInstanceTypesInputRequestTypeDef(
     _RequiredGetOutpostInstanceTypesInputRequestTypeDef,
     _OptionalGetOutpostInstanceTypesInputRequestTypeDef,
 ):
     pass
 
-
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": str,
     },
     total=False,
 )
@@ -382,21 +386,19 @@
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": Sequence[AssetStateType],
     },
     total=False,
 )
 
-
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
-
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
@@ -456,52 +458,24 @@
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
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
     },
 )
 
-StartConnectionResponseTypeDef = TypedDict(
-    "StartConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "UnderlayIpAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -526,21 +500,19 @@
         "Name": str,
         "Description": str,
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
-
 class UpdateOutpostInputRequestTypeDef(
     _RequiredUpdateOutpostInputRequestTypeDef, _OptionalUpdateOutpostInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteInputRequestTypeDef = TypedDict(
@@ -549,21 +521,19 @@
         "Name": str,
         "Description": str,
         "Notes": str,
     },
     total=False,
 )
 
-
 class UpdateSiteInputRequestTypeDef(
     _RequiredUpdateSiteInputRequestTypeDef, _OptionalUpdateSiteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
@@ -578,50 +548,29 @@
         "FiberOpticCableType": FiberOpticCableTypeType,
         "OpticalStandard": OpticalStandardType,
         "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
     },
     total=False,
 )
 
-
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
-
-GetSiteAddressOutputTypeDef = TypedDict(
-    "GetSiteAddressOutputTypeDef",
-    {
-        "SiteId": str,
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
 )
 
-UpdateSiteAddressOutputTypeDef = TypedDict(
-    "UpdateSiteAddressOutputTypeDef",
-    {
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssetInfoTypeDef = TypedDict(
     "AssetInfoTypeDef",
     {
         "AssetId": str,
         "RackId": str,
         "AssetType": Literal["COMPUTE"],
         "ComputeAttributes": ComputeAttributesTypeDef,
@@ -640,23 +589,14 @@
         "WeightLbs": int,
         "SupportedUplinkGbps": List[int],
         "SupportedStorage": List[SupportedStorageEnumType],
     },
     total=False,
 )
 
-GetConnectionResponseTypeDef = TypedDict(
-    "GetConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "ConnectionDetails": ConnectionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateOrderInputRequestTypeDef = TypedDict(
     "_RequiredCreateOrderInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
         "LineItems": Sequence[LineItemRequestTypeDef],
         "PaymentOption": PaymentOptionType,
     },
@@ -665,51 +605,94 @@
     "_OptionalCreateOrderInputRequestTypeDef",
     {
         "PaymentTerm": PaymentTermType,
     },
     total=False,
 )
 
-
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
+GetConnectionResponseTypeDef = TypedDict(
+    "GetConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "ConnectionDetails": ConnectionDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSiteAddressOutputTypeDef = TypedDict(
+    "GetSiteAddressOutputTypeDef",
+    {
+        "SiteId": str,
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
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
+StartConnectionResponseTypeDef = TypedDict(
+    "StartConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "UnderlayIpAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSiteAddressOutputTypeDef = TypedDict(
+    "UpdateSiteAddressOutputTypeDef",
+    {
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOutpostOutputTypeDef = TypedDict(
     "GetOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutpostsOutputTypeDef = TypedDict(
     "ListOutpostsOutputTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOutpostOutputTypeDef = TypedDict(
     "UpdateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSiteInputRequestTypeDef = TypedDict(
     "_RequiredCreateSiteInputRequestTypeDef",
     {
         "Name": str,
@@ -724,21 +707,19 @@
         "OperatingAddress": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
-
 SiteTypeDef = TypedDict(
     "SiteTypeDef",
     {
         "SiteId": str,
         "AccountId": str,
         "Name": str,
         "Description": str,
@@ -756,15 +737,15 @@
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": str,
@@ -780,82 +761,82 @@
 )
 
 ListOrdersOutputTypeDef = TypedDict(
     "ListOrdersOutputTypeDef",
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCatalogItemOutputTypeDef = TypedDict(
     "GetCatalogItemOutputTypeDef",
     {
         "CatalogItem": CatalogItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCatalogItemsOutputTypeDef = TypedDict(
     "ListCatalogItemsOutputTypeDef",
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteOutputTypeDef = TypedDict(
     "GetSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSitesOutputTypeDef = TypedDict(
     "ListSitesOutputTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteOutputTypeDef = TypedDict(
     "UpdateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteRackPhysicalPropertiesOutputTypeDef = TypedDict(
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderTypeDef = TypedDict(
     "OrderTypeDef",
     {
         "OutpostId": str,
@@ -871,18 +852,18 @@
     total=False,
 )
 
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOrderOutputTypeDef = TypedDict(
     "GetOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts/type_defs.pyi` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_outposts.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -45,22 +45,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateOutpostInputRequestTypeDef",
     "OutpostTypeDef",
     "RackPhysicalPropertiesTypeDef",
     "DeleteOutpostInputRequestTypeDef",
     "DeleteSiteInputRequestTypeDef",
     "GetCatalogItemInputRequestTypeDef",
     "GetConnectionRequestRequestTypeDef",
@@ -75,30 +77,29 @@
     "ListAssetsInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartConnectionRequestRequestTypeDef",
-    "StartConnectionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
-    "GetSiteAddressOutputTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
-    "UpdateSiteAddressOutputTypeDef",
     "AssetInfoTypeDef",
     "CatalogItemTypeDef",
-    "GetConnectionResponseTypeDef",
     "CreateOrderInputRequestTypeDef",
+    "GetConnectionResponseTypeDef",
+    "GetSiteAddressOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartConnectionResponseTypeDef",
+    "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
     "SiteTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
@@ -136,17 +137,19 @@
         "AddressLine3": str,
         "DistrictOrCounty": str,
         "Municipality": str,
     },
     total=False,
 )
 
+
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
+
 AssetLocationTypeDef = TypedDict(
     "AssetLocationTypeDef",
     {
         "RackElevation": float,
     },
     total=False,
 )
@@ -195,14 +198,25 @@
     {
         "CatalogItemId": str,
         "Quantity": int,
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
 _RequiredCreateOutpostInputRequestTypeDef = TypedDict(
     "_RequiredCreateOutpostInputRequestTypeDef",
     {
         "Name": str,
         "SiteId": str,
     },
 )
@@ -214,19 +228,21 @@
         "AvailabilityZoneId": str,
         "Tags": Mapping[str, str],
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
+
 class CreateOutpostInputRequestTypeDef(
     _RequiredCreateOutpostInputRequestTypeDef, _OptionalCreateOutpostInputRequestTypeDef
 ):
     pass
 
+
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "OutpostId": str,
         "OwnerId": str,
         "OutpostArn": str,
         "SiteId": str,
@@ -311,20 +327,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetOutpostInstanceTypesInputRequestTypeDef(
     _RequiredGetOutpostInstanceTypesInputRequestTypeDef,
     _OptionalGetOutpostInstanceTypesInputRequestTypeDef,
 ):
     pass
 
+
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": str,
     },
     total=False,
 )
@@ -375,19 +393,21 @@
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": Sequence[AssetStateType],
     },
     total=False,
 )
 
+
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
+
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
@@ -447,52 +467,24 @@
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
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
     },
 )
 
-StartConnectionResponseTypeDef = TypedDict(
-    "StartConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "UnderlayIpAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -517,19 +509,21 @@
         "Name": str,
         "Description": str,
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
+
 class UpdateOutpostInputRequestTypeDef(
     _RequiredUpdateOutpostInputRequestTypeDef, _OptionalUpdateOutpostInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteInputRequestTypeDef = TypedDict(
@@ -538,19 +532,21 @@
         "Name": str,
         "Description": str,
         "Notes": str,
     },
     total=False,
 )
 
+
 class UpdateSiteInputRequestTypeDef(
     _RequiredUpdateSiteInputRequestTypeDef, _OptionalUpdateSiteInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
@@ -565,48 +561,31 @@
         "FiberOpticCableType": FiberOpticCableTypeType,
         "OpticalStandard": OpticalStandardType,
         "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
     },
     total=False,
 )
 
+
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
-GetSiteAddressOutputTypeDef = TypedDict(
-    "GetSiteAddressOutputTypeDef",
-    {
-        "SiteId": str,
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
 )
 
-UpdateSiteAddressOutputTypeDef = TypedDict(
-    "UpdateSiteAddressOutputTypeDef",
-    {
-        "AddressType": AddressTypeType,
-        "Address": AddressTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssetInfoTypeDef = TypedDict(
     "AssetInfoTypeDef",
     {
         "AssetId": str,
         "RackId": str,
         "AssetType": Literal["COMPUTE"],
         "ComputeAttributes": ComputeAttributesTypeDef,
@@ -625,23 +604,14 @@
         "WeightLbs": int,
         "SupportedUplinkGbps": List[int],
         "SupportedStorage": List[SupportedStorageEnumType],
     },
     total=False,
 )
 
-GetConnectionResponseTypeDef = TypedDict(
-    "GetConnectionResponseTypeDef",
-    {
-        "ConnectionId": str,
-        "ConnectionDetails": ConnectionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateOrderInputRequestTypeDef = TypedDict(
     "_RequiredCreateOrderInputRequestTypeDef",
     {
         "OutpostIdentifier": str,
         "LineItems": Sequence[LineItemRequestTypeDef],
         "PaymentOption": PaymentOptionType,
     },
@@ -650,49 +620,96 @@
     "_OptionalCreateOrderInputRequestTypeDef",
     {
         "PaymentTerm": PaymentTermType,
     },
     total=False,
 )
 
+
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
+
+GetConnectionResponseTypeDef = TypedDict(
+    "GetConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "ConnectionDetails": ConnectionDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSiteAddressOutputTypeDef = TypedDict(
+    "GetSiteAddressOutputTypeDef",
+    {
+        "SiteId": str,
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
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
+StartConnectionResponseTypeDef = TypedDict(
+    "StartConnectionResponseTypeDef",
+    {
+        "ConnectionId": str,
+        "UnderlayIpAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSiteAddressOutputTypeDef = TypedDict(
+    "UpdateSiteAddressOutputTypeDef",
+    {
+        "AddressType": AddressTypeType,
+        "Address": AddressTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOutpostOutputTypeDef = TypedDict(
     "GetOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutpostsOutputTypeDef = TypedDict(
     "ListOutpostsOutputTypeDef",
     {
         "Outposts": List[OutpostTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOutpostOutputTypeDef = TypedDict(
     "UpdateOutpostOutputTypeDef",
     {
         "Outpost": OutpostTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSiteInputRequestTypeDef = TypedDict(
     "_RequiredCreateSiteInputRequestTypeDef",
     {
         "Name": str,
@@ -707,19 +724,21 @@
         "OperatingAddress": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
+
 SiteTypeDef = TypedDict(
     "SiteTypeDef",
     {
         "SiteId": str,
         "AccountId": str,
         "Name": str,
         "Description": str,
@@ -737,15 +756,15 @@
 GetOutpostInstanceTypesOutputTypeDef = TypedDict(
     "GetOutpostInstanceTypesOutputTypeDef",
     {
         "InstanceTypes": List[InstanceTypeItemTypeDef],
         "NextToken": str,
         "OutpostId": str,
         "OutpostArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemTypeDef = TypedDict(
     "LineItemTypeDef",
     {
         "CatalogItemId": str,
@@ -761,82 +780,82 @@
 )
 
 ListOrdersOutputTypeDef = TypedDict(
     "ListOrdersOutputTypeDef",
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCatalogItemOutputTypeDef = TypedDict(
     "GetCatalogItemOutputTypeDef",
     {
         "CatalogItem": CatalogItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCatalogItemsOutputTypeDef = TypedDict(
     "ListCatalogItemsOutputTypeDef",
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteOutputTypeDef = TypedDict(
     "GetSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSitesOutputTypeDef = TypedDict(
     "ListSitesOutputTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteOutputTypeDef = TypedDict(
     "UpdateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteRackPhysicalPropertiesOutputTypeDef = TypedDict(
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderTypeDef = TypedDict(
     "OrderTypeDef",
     {
         "OutpostId": str,
@@ -852,18 +871,18 @@
     total=False,
 )
 
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOrderOutputTypeDef = TypedDict(
     "GetOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/PKG-INFO` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-outposts
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Outposts 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore outposts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore outposts type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-outposts"></a>
 
 # types-aiobotocore-outposts
 
 [![PyPI - types-aiobotocore-outposts](https://img.shields.io/pypi/v/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-outposts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-outposts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-outposts?color=blue)](https://pypistats.org/packages/types-aiobotocore-outposts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-outposts)](https://pepy.tech/project/types-aiobotocore-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Outposts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [types-aiobotocore-outposts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_outposts/).
 
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
@@ -302,30 +301,31 @@
 )
 
 
 def check_value(value: AddressTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_outposts.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_outposts.type_defs import (
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateOutpostInputRequestTypeDef,
     OutpostTypeDef,
     RackPhysicalPropertiesTypeDef,
     DeleteOutpostInputRequestTypeDef,
     DeleteSiteInputRequestTypeDef,
     GetCatalogItemInputRequestTypeDef,
     GetConnectionRequestRequestTypeDef,
@@ -340,30 +340,29 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartConnectionRequestRequestTypeDef,
-    StartConnectionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
-    GetSiteAddressOutputTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
-    UpdateSiteAddressOutputTypeDef,
     AssetInfoTypeDef,
     CatalogItemTypeDef,
-    GetConnectionResponseTypeDef,
     CreateOrderInputRequestTypeDef,
+    GetConnectionResponseTypeDef,
+    GetSiteAddressOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartConnectionResponseTypeDef,
+    UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
     SiteTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
@@ -379,15 +378,15 @@
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
     OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-outposts-2.5.2/types_aiobotocore_outposts.egg-info/SOURCES.txt` & `types-aiobotocore-outposts-2.5.2.post1/types_aiobotocore_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*


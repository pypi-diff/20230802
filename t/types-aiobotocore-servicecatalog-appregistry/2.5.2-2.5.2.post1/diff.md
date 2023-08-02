# Comparing `tmp/types-aiobotocore-servicecatalog-appregistry-2.5.2.tar.gz` & `tmp/types-aiobotocore-servicecatalog-appregistry-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicecatalog-appregistry-2.5.2.tar", last modified: Sat Jul  8 01:44:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicecatalog-appregistry-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:00 2023, max compression
```

## Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2.tar` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.886894 types-aiobotocore-servicecatalog-appregistry-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-07-08 01:44:18.886894 types-aiobotocore-servicecatalog-appregistry-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:18.886894 types-aiobotocore-servicecatalog-appregistry-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.866894 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21742 2023-07-08 01:40:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21721 2023-07-08 01:40:58.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:55.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:18.886894 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 01:44:18.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15887 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-02 14:49:34.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.009460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:35.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.033460 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 14:52:59.000000 types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/LICENSE` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/PKG-INFO` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog-appregistry
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicecatalog-appregistry type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore servicecatalog-appregistry type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicecatalog-appregistry)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog-appregistry)](https://pepy.tech/project/types-aiobotocore-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppRegistry 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
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
@@ -333,93 +332,93 @@
 )
 
 
 def check_value(value: ListApplicationsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicecatalog_appregistry.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_servicecatalog_appregistry.type_defs import (
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
-    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
-    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
     AppRegistryConfigurationTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
+    AssociateResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    CreateApplicationResponseTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SyncResourceResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationTypeDef:
+def get_value() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/README.md` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicecatalog-appregistry)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog-appregistry)](https://pepy.tech/project/types-aiobotocore-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppRegistry 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
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
@@ -300,93 +300,93 @@
 )
 
 
 def check_value(value: ListApplicationsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicecatalog_appregistry.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_servicecatalog_appregistry.type_defs import (
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
-    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
-    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
     AppRegistryConfigurationTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
+    AssociateResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    CreateApplicationResponseTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SyncResourceResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationTypeDef:
+def get_value() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/setup.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicecatalog-appregistry",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore servicecatalog-appregistry type-annotations boto3-stubs mypy typeshed"
+        "aiobotocore servicecatalog-appregistry type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_servicecatalog_appregistry": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/__init__.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/__init__.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/__main__.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppRegistry 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AppRegistry 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry\nOther"
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

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/client.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/client.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/literals.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/literals.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/paginator.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,73 +64,73 @@
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listapplicationspaginator)
         """
 
 
 class ListAssociatedAttributeGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociatedAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
         """
 
 
 class ListAssociatedResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociatedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
         """
 
 
 class ListAttributeGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
         """
 
 
 class ListAttributeGroupsForApplicationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttributeGroupsForApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
         """
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/paginator.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,69 +61,69 @@
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listapplicationspaginator)
         """
 
 class ListAssociatedAttributeGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociatedAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
         """
 
 class ListAssociatedResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociatedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
         """
 
 class ListAttributeGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
         """
 
 class ListAttributeGroupsForApplicationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttributeGroupsForApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
         """
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/type_defs.py` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
-    data: TagQueryConfigurationTypeDef = {...}
+    data: TagQueryConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceGroupStateType, ResourceTypeType, SyncActionType
@@ -24,68 +24,68 @@
 
 
 __all__ = (
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
-    "AssociateAttributeGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateResourceRequestRequestTypeDef",
-    "AssociateResourceResponseTypeDef",
     "AttributeGroupDetailsTypeDef",
     "AttributeGroupSummaryTypeDef",
     "AttributeGroupTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateAttributeGroupRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteAttributeGroupRequestRequestTypeDef",
     "DisassociateAttributeGroupRequestRequestTypeDef",
-    "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceRequestRequestTypeDef",
-    "DisassociateResourceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetAssociatedResourceRequestRequestTypeDef",
     "GetAttributeGroupRequestRequestTypeDef",
-    "GetAttributeGroupResponseTypeDef",
     "ResourceGroupTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
     "ListAssociatedAttributeGroupsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
     "ListAssociatedResourcesRequestRequestTypeDef",
-    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
     "ListAttributeGroupsForApplicationRequestRequestTypeDef",
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ListAttributeGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "SyncResourceRequestRequestTypeDef",
-    "SyncResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
     "AppRegistryConfigurationTypeDef",
+    "AssociateAttributeGroupResponseTypeDef",
+    "AssociateResourceResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
+    "DisassociateAttributeGroupResponseTypeDef",
+    "DisassociateResourceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributeGroupResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SyncResourceResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListAttributeGroupsForApplicationResponseTypeDef",
     "DeleteAttributeGroupResponseTypeDef",
     "ListAttributeGroupsResponseTypeDef",
     "CreateAttributeGroupResponseTypeDef",
     "UpdateAttributeGroupResponseTypeDef",
     "IntegrationsTypeDef",
     "ResourceIntegrationsTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ResourceInfoTypeDef",
     "GetConfigurationResponseTypeDef",
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
@@ -130,41 +130,34 @@
     "AssociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-AssociateAttributeGroupResponseTypeDef = TypedDict(
-    "AssociateAttributeGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-AssociateResourceResponseTypeDef = TypedDict(
-    "AssociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeGroupDetailsTypeDef = TypedDict(
     "AttributeGroupDetailsTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "createdBy": str,
@@ -266,48 +259,23 @@
     "DisassociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-DisassociateAttributeGroupResponseTypeDef = TypedDict(
-    "DisassociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateResourceRequestRequestTypeDef = TypedDict(
     "DisassociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-DisassociateResourceResponseTypeDef = TypedDict(
-    "DisassociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 
@@ -323,83 +291,43 @@
 GetAttributeGroupRequestRequestTypeDef = TypedDict(
     "GetAttributeGroupRequestRequestTypeDef",
     {
         "attributeGroup": str,
     },
 )
 
-GetAttributeGroupResponseTypeDef = TypedDict(
-    "GetAttributeGroupResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "attributes": str,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "tags": Dict[str, str],
-        "createdBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceGroupTypeDef = TypedDict(
     "ResourceGroupTypeDef",
     {
         "state": ResourceGroupStateType,
         "arn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "application": str,
-        },
-    )
-)
-_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
-    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAttributeGroupsRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
@@ -415,45 +343,14 @@
 class ListAssociatedAttributeGroupsRequestRequestTypeDef(
     _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef,
     _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    {
-        "attributeGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
-    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedResourcesRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedResourcesRequestRequestTypeDef = TypedDict(
@@ -469,36 +366,14 @@
 class ListAssociatedResourcesRequestRequestTypeDef(
     _RequiredListAssociatedResourcesRequestRequestTypeDef,
     _OptionalListAssociatedResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
-    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributeGroupsForApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
@@ -514,22 +389,14 @@
 class ListAttributeGroupsForApplicationRequestRequestTypeDef(
     _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef,
     _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef,
 ):
     pass
 
 
-ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAttributeGroupsRequestRequestTypeDef = TypedDict(
     "ListAttributeGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -538,69 +405,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "tagValue": str,
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
 SyncResourceRequestRequestTypeDef = TypedDict(
     "SyncResourceRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-SyncResourceResponseTypeDef = TypedDict(
-    "SyncResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "actionTaken": SyncActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -663,86 +491,172 @@
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
 
+AssociateAttributeGroupResponseTypeDef = TypedDict(
+    "AssociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateResourceResponseTypeDef = TypedDict(
+    "AssociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "application": ApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteApplicationResponseTypeDef = TypedDict(
     "DeleteApplicationResponseTypeDef",
     {
         "application": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateAttributeGroupResponseTypeDef = TypedDict(
+    "DisassociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateResourceResponseTypeDef = TypedDict(
+    "DisassociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAttributeGroupResponseTypeDef = TypedDict(
+    "GetAttributeGroupResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "attributes": str,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "tags": Dict[str, str],
+        "createdBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
+    "ListAssociatedAttributeGroupsResponseTypeDef",
     {
-        "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attributeGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SyncResourceResponseTypeDef = TypedDict(
+    "SyncResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "actionTaken": SyncActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsForApplicationResponseTypeDef = TypedDict(
     "ListAttributeGroupsForApplicationResponseTypeDef",
     {
         "attributeGroupsDetails": List[AttributeGroupDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAttributeGroupResponseTypeDef = TypedDict(
     "DeleteAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsResponseTypeDef = TypedDict(
     "ListAttributeGroupsResponseTypeDef",
     {
         "attributeGroups": List[AttributeGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttributeGroupResponseTypeDef = TypedDict(
     "CreateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAttributeGroupResponseTypeDef = TypedDict(
     "UpdateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationsTypeDef = TypedDict(
     "IntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
@@ -754,14 +668,100 @@
     "ResourceIntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
     },
     total=False,
 )
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "application": str,
+        },
+    )
+)
+_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
+    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
+    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
+    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+):
+    pass
+
+
+ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "name": str,
         "arn": str,
         "resourceType": ResourceTypeType,
         "resourceDetails": ResourceDetailsTypeDef,
@@ -769,15 +769,15 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
@@ -792,15 +792,15 @@
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "associatedResourceCount": int,
         "tags": Dict[str, str],
         "integrations": IntegrationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "name": str,
@@ -812,18 +812,18 @@
 )
 
 ListAssociatedResourcesResponseTypeDef = TypedDict(
     "ListAssociatedResourcesResponseTypeDef",
     {
         "resources": List[ResourceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssociatedResourceResponseTypeDef = TypedDict(
     "GetAssociatedResourceResponseTypeDef",
     {
         "resource": ResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
-    data: TagQueryConfigurationTypeDef = {...}
+    data: TagQueryConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceGroupStateType, ResourceTypeType, SyncActionType
@@ -23,68 +23,68 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
-    "AssociateAttributeGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateResourceRequestRequestTypeDef",
-    "AssociateResourceResponseTypeDef",
     "AttributeGroupDetailsTypeDef",
     "AttributeGroupSummaryTypeDef",
     "AttributeGroupTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateAttributeGroupRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteAttributeGroupRequestRequestTypeDef",
     "DisassociateAttributeGroupRequestRequestTypeDef",
-    "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceRequestRequestTypeDef",
-    "DisassociateResourceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetAssociatedResourceRequestRequestTypeDef",
     "GetAttributeGroupRequestRequestTypeDef",
-    "GetAttributeGroupResponseTypeDef",
     "ResourceGroupTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
     "ListAssociatedAttributeGroupsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
     "ListAssociatedResourcesRequestRequestTypeDef",
-    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
     "ListAttributeGroupsForApplicationRequestRequestTypeDef",
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ListAttributeGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "SyncResourceRequestRequestTypeDef",
-    "SyncResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
     "AppRegistryConfigurationTypeDef",
+    "AssociateAttributeGroupResponseTypeDef",
+    "AssociateResourceResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
+    "DisassociateAttributeGroupResponseTypeDef",
+    "DisassociateResourceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributeGroupResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SyncResourceResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListAttributeGroupsForApplicationResponseTypeDef",
     "DeleteAttributeGroupResponseTypeDef",
     "ListAttributeGroupsResponseTypeDef",
     "CreateAttributeGroupResponseTypeDef",
     "UpdateAttributeGroupResponseTypeDef",
     "IntegrationsTypeDef",
     "ResourceIntegrationsTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ResourceInfoTypeDef",
     "GetConfigurationResponseTypeDef",
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
@@ -129,41 +129,34 @@
     "AssociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-AssociateAttributeGroupResponseTypeDef = TypedDict(
-    "AssociateAttributeGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-AssociateResourceResponseTypeDef = TypedDict(
-    "AssociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeGroupDetailsTypeDef = TypedDict(
     "AttributeGroupDetailsTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "createdBy": str,
@@ -261,48 +254,23 @@
     "DisassociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-DisassociateAttributeGroupResponseTypeDef = TypedDict(
-    "DisassociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateResourceRequestRequestTypeDef = TypedDict(
     "DisassociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-DisassociateResourceResponseTypeDef = TypedDict(
-    "DisassociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 
@@ -318,81 +286,43 @@
 GetAttributeGroupRequestRequestTypeDef = TypedDict(
     "GetAttributeGroupRequestRequestTypeDef",
     {
         "attributeGroup": str,
     },
 )
 
-GetAttributeGroupResponseTypeDef = TypedDict(
-    "GetAttributeGroupResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "attributes": str,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "tags": Dict[str, str],
-        "createdBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceGroupTypeDef = TypedDict(
     "ResourceGroupTypeDef",
     {
         "state": ResourceGroupStateType,
         "arn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "application": str,
-        },
-    )
-)
-_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
-    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAttributeGroupsRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
@@ -406,43 +336,14 @@
 
 class ListAssociatedAttributeGroupsRequestRequestTypeDef(
     _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef,
     _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef,
 ):
     pass
 
-ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    {
-        "attributeGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
-    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedResourcesRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedResourcesRequestRequestTypeDef = TypedDict(
@@ -456,34 +357,14 @@
 
 class ListAssociatedResourcesRequestRequestTypeDef(
     _RequiredListAssociatedResourcesRequestRequestTypeDef,
     _OptionalListAssociatedResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
-    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributeGroupsForApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
@@ -497,22 +378,14 @@
 
 class ListAttributeGroupsForApplicationRequestRequestTypeDef(
     _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef,
     _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef,
 ):
     pass
 
-ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAttributeGroupsRequestRequestTypeDef = TypedDict(
     "ListAttributeGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -521,69 +394,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "tagValue": str,
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
 SyncResourceRequestRequestTypeDef = TypedDict(
     "SyncResourceRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-SyncResourceResponseTypeDef = TypedDict(
-    "SyncResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "actionTaken": SyncActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -642,86 +476,172 @@
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
 
+AssociateAttributeGroupResponseTypeDef = TypedDict(
+    "AssociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateResourceResponseTypeDef = TypedDict(
+    "AssociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "application": ApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteApplicationResponseTypeDef = TypedDict(
     "DeleteApplicationResponseTypeDef",
     {
         "application": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateAttributeGroupResponseTypeDef = TypedDict(
+    "DisassociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateResourceResponseTypeDef = TypedDict(
+    "DisassociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAttributeGroupResponseTypeDef = TypedDict(
+    "GetAttributeGroupResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "attributes": str,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "tags": Dict[str, str],
+        "createdBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
+    "ListAssociatedAttributeGroupsResponseTypeDef",
     {
-        "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attributeGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SyncResourceResponseTypeDef = TypedDict(
+    "SyncResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "actionTaken": SyncActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsForApplicationResponseTypeDef = TypedDict(
     "ListAttributeGroupsForApplicationResponseTypeDef",
     {
         "attributeGroupsDetails": List[AttributeGroupDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAttributeGroupResponseTypeDef = TypedDict(
     "DeleteAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsResponseTypeDef = TypedDict(
     "ListAttributeGroupsResponseTypeDef",
     {
         "attributeGroups": List[AttributeGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttributeGroupResponseTypeDef = TypedDict(
     "CreateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAttributeGroupResponseTypeDef = TypedDict(
     "UpdateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationsTypeDef = TypedDict(
     "IntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
@@ -733,14 +653,94 @@
     "ResourceIntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
     },
     total=False,
 )
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "application": str,
+        },
+    )
+)
+_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
+    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
+    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
+    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+):
+    pass
+
+ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "name": str,
         "arn": str,
         "resourceType": ResourceTypeType,
         "resourceDetails": ResourceDetailsTypeDef,
@@ -748,15 +748,15 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
@@ -771,15 +771,15 @@
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "associatedResourceCount": int,
         "tags": Dict[str, str],
         "integrations": IntegrationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "name": str,
@@ -791,18 +791,18 @@
 )
 
 ListAssociatedResourcesResponseTypeDef = TypedDict(
     "ListAssociatedResourcesResponseTypeDef",
     {
         "resources": List[ResourceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssociatedResourceResponseTypeDef = TypedDict(
     "GetAssociatedResourceResponseTypeDef",
     {
         "resource": ResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-servicecatalog-appregistry
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppRegistry 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore servicecatalog-appregistry type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore servicecatalog-appregistry type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-servicecatalog-appregistry"></a>
 
 # types-aiobotocore-servicecatalog-appregistry
 
 [![PyPI - types-aiobotocore-servicecatalog-appregistry](https://img.shields.io/pypi/v/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/types-aiobotocore-servicecatalog-appregistry)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-servicecatalog-appregistry)](https://pepy.tech/project/types-aiobotocore-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppRegistry 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [types-aiobotocore-servicecatalog-appregistry docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog_appregistry/).
 
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
@@ -333,93 +332,93 @@
 )
 
 
 def check_value(value: ListApplicationsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_servicecatalog_appregistry.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_servicecatalog_appregistry.type_defs import (
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
-    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
-    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
     AppRegistryConfigurationTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
+    AssociateResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    CreateApplicationResponseTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SyncResourceResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationTypeDef:
+def get_value() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-servicecatalog-appregistry-2.5.2/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt` & `types-aiobotocore-servicecatalog-appregistry-2.5.2.post1/types_aiobotocore_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*


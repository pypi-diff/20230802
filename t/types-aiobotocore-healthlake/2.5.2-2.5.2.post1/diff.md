# Comparing `tmp/types-aiobotocore-healthlake-2.5.2.tar.gz` & `tmp/types-aiobotocore-healthlake-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-healthlake-2.5.2.tar", last modified: Sat Jul  8 01:43:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-healthlake-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:22 2023, max compression
```

## Comparing `types-aiobotocore-healthlake-2.5.2.tar` & `types-aiobotocore-healthlake-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.378221 types-aiobotocore-healthlake-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-07-08 01:43:42.378221 types-aiobotocore-healthlake-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:42.378221 types-aiobotocore-healthlake-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.378221 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-08 01:31:57.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-07-08 01:31:57.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:56.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.378221 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-07-08 01:43:42.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-08 01:43:42.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:42.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:42.000000 types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:22.117575 types-aiobotocore-healthlake-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-02 14:52:22.109575 types-aiobotocore-healthlake-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:22.117575 types-aiobotocore-healthlake-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:22.109575 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:55.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:22.109575 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:21.000000 types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-healthlake-2.5.2/LICENSE` & `types-aiobotocore-healthlake-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2/PKG-INFO` & `types-aiobotocore-healthlake-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-healthlake
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.HealthLake 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.HealthLake 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore healthlake type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore healthlake type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-healthlake"></a>
 
 # types-aiobotocore-healthlake
 
 [![PyPI - types-aiobotocore-healthlake](https://img.shields.io/pypi/v/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-healthlake?color=blue)](https://pypistats.org/packages/types-aiobotocore-healthlake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.HealthLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [types-aiobotocore-healthlake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/).
 
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
@@ -286,48 +285,49 @@
 )
 
 
 def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_healthlake.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
-    DatastoreFilterTypeDef,
+    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
-    ListFHIRExportJobsRequestRequestTypeDef,
-    ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    StartFHIRExportJobResponseTypeDef,
-    StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListFHIRDatastoresRequestRequestTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartFHIRExportJobResponseTypeDef,
+    StartFHIRImportJobResponseTypeDef,
+    DatastoreFilterTypeDef,
+    ListFHIRExportJobsRequestRequestTypeDef,
+    ListFHIRImportJobsRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
+    ListFHIRDatastoresRequestRequestTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
@@ -335,15 +335,15 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityProviderConfigurationTypeDef:
+def get_value() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-healthlake-2.5.2/README.md` & `types-aiobotocore-healthlake-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-healthlake"></a>
 
 # types-aiobotocore-healthlake
 
 [![PyPI - types-aiobotocore-healthlake](https://img.shields.io/pypi/v/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-healthlake?color=blue)](https://pypistats.org/packages/types-aiobotocore-healthlake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.HealthLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [types-aiobotocore-healthlake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/).
 
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
@@ -253,48 +253,49 @@
 )
 
 
 def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_healthlake.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
-    DatastoreFilterTypeDef,
+    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
-    ListFHIRExportJobsRequestRequestTypeDef,
-    ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    StartFHIRExportJobResponseTypeDef,
-    StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListFHIRDatastoresRequestRequestTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartFHIRExportJobResponseTypeDef,
+    StartFHIRImportJobResponseTypeDef,
+    DatastoreFilterTypeDef,
+    ListFHIRExportJobsRequestRequestTypeDef,
+    ListFHIRImportJobsRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
+    ListFHIRDatastoresRequestRequestTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
@@ -302,15 +303,15 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityProviderConfigurationTypeDef:
+def get_value() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-healthlake-2.5.2/setup.py` & `types-aiobotocore-healthlake-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-healthlake",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.HealthLake 2.5.2 service generated with"
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
-    keywords="aiobotocore healthlake type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore healthlake type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_healthlake": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/"
```

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/__main__.py` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.HealthLake 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.HealthLake 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
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

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/client.py` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("healthlake") as client:
         client: HealthLakeClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import JobStatusType
 from .type_defs import (
     CreateFHIRDatastoreResponseTypeDef,
@@ -37,14 +36,15 @@
     ListTagsForResourceResponseTypeDef,
     OutputDataConfigTypeDef,
     PreloadDataConfigTypeDef,
     SseConfigurationTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -194,16 +194,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRExportJobsResponseTypeDef:
         """
         Lists all FHIR export jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_export_jobs)
         """
@@ -212,16 +212,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRImportJobsResponseTypeDef:
         """
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_import_jobs)
         """
```

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/client.pyi` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("healthlake") as client:
         client: HealthLakeClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import JobStatusType
 from .type_defs import (
     CreateFHIRDatastoreResponseTypeDef,
@@ -37,14 +36,15 @@
     ListTagsForResourceResponseTypeDef,
     OutputDataConfigTypeDef,
     PreloadDataConfigTypeDef,
     SseConfigurationTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -180,16 +180,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRExportJobsResponseTypeDef:
         """
         Lists all FHIR export jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_export_jobs)
         """
@@ -197,16 +197,16 @@
         self,
         *,
         DatastoreId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         JobName: str = ...,
         JobStatus: JobStatusType = ...,
-        SubmittedBefore: Union[datetime, str] = ...,
-        SubmittedAfter: Union[datetime, str] = ...
+        SubmittedBefore: TimestampTypeDef = ...,
+        SubmittedAfter: TimestampTypeDef = ...
     ) -> ListFHIRImportJobsResponseTypeDef:
         """
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/client/#list_fhir_import_jobs)
         """
```

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/literals.py` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/literals.pyi` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/type_defs.py` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_healthlake.type_defs import IdentityProviderConfigurationTypeDef
 
-    data: IdentityProviderConfigurationTypeDef = {...}
+    data: IdentityProviderConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
@@ -22,41 +22,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
-    "CreateFHIRDatastoreResponseTypeDef",
-    "DatastoreFilterTypeDef",
+    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
-    "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "KmsEncryptionConfigTypeDef",
-    "ListFHIRExportJobsRequestRequestTypeDef",
-    "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartFHIRExportJobResponseTypeDef",
-    "StartFHIRImportJobResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListFHIRDatastoresRequestRequestTypeDef",
+    "CreateFHIRDatastoreResponseTypeDef",
+    "DeleteFHIRDatastoreResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartFHIRExportJobResponseTypeDef",
+    "StartFHIRImportJobResponseTypeDef",
+    "DatastoreFilterTypeDef",
+    "ListFHIRExportJobsRequestRequestTypeDef",
+    "ListFHIRImportJobsRequestRequestTypeDef",
     "SseConfigurationTypeDef",
     "OutputDataConfigTypeDef",
+    "ListFHIRDatastoresRequestRequestTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
@@ -79,21 +79,19 @@
         "FineGrainedAuthorizationEnabled": bool,
         "Metadata": str,
         "IdpLambdaArn": str,
     },
     total=False,
 )
 
-
 class IdentityProviderConfigurationTypeDef(
     _RequiredIdentityProviderConfigurationTypeDef, _OptionalIdentityProviderConfigurationTypeDef
 ):
     pass
 
-
 PreloadDataConfigTypeDef = TypedDict(
     "PreloadDataConfigTypeDef",
     {
         "PreloadDataType": Literal["SYNTHEA"],
     },
 )
 
@@ -101,54 +99,33 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateFHIRDatastoreResponseTypeDef = TypedDict(
-    "CreateFHIRDatastoreResponseTypeDef",
-    {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DatastoreFilterTypeDef = TypedDict(
-    "DatastoreFilterTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "DatastoreName": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
-DeleteFHIRDatastoreResponseTypeDef = TypedDict(
-    "DeleteFHIRDatastoreResponseTypeDef",
-    {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -186,155 +163,161 @@
     "_OptionalKmsEncryptionConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class KmsEncryptionConfigTypeDef(
     _RequiredKmsEncryptionConfigTypeDef, _OptionalKmsEncryptionConfigTypeDef
 ):
     pass
 
-
-_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "DatastoreId": str,
+        "ResourceARN": str,
     },
 )
-_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
+
+S3ConfigurationTypeDef = TypedDict(
+    "S3ConfigurationTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
+        "S3Uri": str,
+        "KmsKeyId": str,
     },
-    total=False,
 )
 
-
-class ListFHIRExportJobsRequestRequestTypeDef(
-    _RequiredListFHIRExportJobsRequestRequestTypeDef,
-    _OptionalListFHIRExportJobsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "DatastoreId": str,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
-_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-
-class ListFHIRImportJobsRequestRequestTypeDef(
-    _RequiredListFHIRImportJobsRequestRequestTypeDef,
-    _OptionalListFHIRImportJobsRequestRequestTypeDef,
-):
-    pass
-
-
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+CreateFHIRDatastoreResponseTypeDef = TypedDict(
+    "CreateFHIRDatastoreResponseTypeDef",
     {
-        "ResourceARN": str,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-S3ConfigurationTypeDef = TypedDict(
-    "S3ConfigurationTypeDef",
+DeleteFHIRDatastoreResponseTypeDef = TypedDict(
+    "DeleteFHIRDatastoreResponseTypeDef",
     {
-        "S3Uri": str,
-        "KmsKeyId": str,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRExportJobResponseTypeDef = TypedDict(
     "StartFHIRExportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRImportJobResponseTypeDef = TypedDict(
     "StartFHIRImportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+DatastoreFilterTypeDef = TypedDict(
+    "DatastoreFilterTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "DatastoreName": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DatastoreId": str,
     },
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "NextToken": str,
+        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
     },
+    total=False,
 )
 
-ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
-    "ListFHIRDatastoresRequestRequestTypeDef",
+class ListFHIRExportJobsRequestRequestTypeDef(
+    _RequiredListFHIRExportJobsRequestRequestTypeDef,
+    _OptionalListFHIRExportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
+    {
+        "DatastoreId": str,
+    },
+)
+_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
     {
-        "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+class ListFHIRImportJobsRequestRequestTypeDef(
+    _RequiredListFHIRImportJobsRequestRequestTypeDef,
+    _OptionalListFHIRImportJobsRequestRequestTypeDef,
+):
+    pass
+
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
@@ -342,14 +325,24 @@
     "OutputDataConfigTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
+ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
+    "ListFHIRDatastoresRequestRequestTypeDef",
+    {
+        "Filter": DatastoreFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreTypeVersion": Literal["R4"],
     },
 )
 _OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
@@ -361,22 +354,20 @@
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFHIRDatastoreRequestRequestTypeDef(
     _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
     _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDatastorePropertiesTypeDef = TypedDict(
     "_RequiredDatastorePropertiesTypeDef",
     {
         "DatastoreId": str,
         "DatastoreArn": str,
         "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
@@ -391,21 +382,19 @@
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DatastorePropertiesTypeDef(
     _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
 ):
     pass
 
-
 _RequiredExportJobPropertiesTypeDef = TypedDict(
     "_RequiredExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
@@ -419,21 +408,19 @@
         "EndTime": datetime,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
-
 class ExportJobPropertiesTypeDef(
     _RequiredExportJobPropertiesTypeDef, _OptionalExportJobPropertiesTypeDef
 ):
     pass
 
-
 _RequiredImportJobPropertiesTypeDef = TypedDict(
     "_RequiredImportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
@@ -448,21 +435,19 @@
         "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
-
 class ImportJobPropertiesTypeDef(
     _RequiredImportJobPropertiesTypeDef, _OptionalImportJobPropertiesTypeDef
 ):
     pass
 
-
 _RequiredStartFHIRExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRExportJobRequestRequestTypeDef",
     {
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
         "ClientToken": str,
@@ -472,22 +457,20 @@
     "_OptionalStartFHIRExportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
-
 class StartFHIRExportJobRequestRequestTypeDef(
     _RequiredStartFHIRExportJobRequestRequestTypeDef,
     _OptionalStartFHIRExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartFHIRImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRImportJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
@@ -498,65 +481,63 @@
     "_OptionalStartFHIRImportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
-
 class StartFHIRImportJobRequestRequestTypeDef(
     _RequiredStartFHIRImportJobRequestRequestTypeDef,
     _OptionalStartFHIRImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRDatastoresResponseTypeDef = TypedDict(
     "ListFHIRDatastoresResponseTypeDef",
     {
         "DatastorePropertiesList": List[DatastorePropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRExportJobResponseTypeDef = TypedDict(
     "DescribeFHIRExportJobResponseTypeDef",
     {
         "ExportJobProperties": ExportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRExportJobsResponseTypeDef = TypedDict(
     "ListFHIRExportJobsResponseTypeDef",
     {
         "ExportJobPropertiesList": List[ExportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRImportJobResponseTypeDef = TypedDict(
     "DescribeFHIRImportJobResponseTypeDef",
     {
         "ImportJobProperties": ImportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRImportJobsResponseTypeDef = TypedDict(
     "ListFHIRImportJobsResponseTypeDef",
     {
         "ImportJobPropertiesList": List[ImportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake/type_defs.pyi` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_healthlake.type_defs import IdentityProviderConfigurationTypeDef
 
-    data: IdentityProviderConfigurationTypeDef = {...}
+    data: IdentityProviderConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
@@ -22,40 +22,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
-    "CreateFHIRDatastoreResponseTypeDef",
-    "DatastoreFilterTypeDef",
+    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
-    "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
     "InputDataConfigTypeDef",
     "KmsEncryptionConfigTypeDef",
-    "ListFHIRExportJobsRequestRequestTypeDef",
-    "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartFHIRExportJobResponseTypeDef",
-    "StartFHIRImportJobResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListFHIRDatastoresRequestRequestTypeDef",
+    "CreateFHIRDatastoreResponseTypeDef",
+    "DeleteFHIRDatastoreResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartFHIRExportJobResponseTypeDef",
+    "StartFHIRImportJobResponseTypeDef",
+    "DatastoreFilterTypeDef",
+    "ListFHIRExportJobsRequestRequestTypeDef",
+    "ListFHIRImportJobsRequestRequestTypeDef",
     "SseConfigurationTypeDef",
     "OutputDataConfigTypeDef",
+    "ListFHIRDatastoresRequestRequestTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
@@ -78,19 +80,21 @@
         "FineGrainedAuthorizationEnabled": bool,
         "Metadata": str,
         "IdpLambdaArn": str,
     },
     total=False,
 )
 
+
 class IdentityProviderConfigurationTypeDef(
     _RequiredIdentityProviderConfigurationTypeDef, _OptionalIdentityProviderConfigurationTypeDef
 ):
     pass
 
+
 PreloadDataConfigTypeDef = TypedDict(
     "PreloadDataConfigTypeDef",
     {
         "PreloadDataType": Literal["SYNTHEA"],
     },
 )
 
@@ -98,54 +102,33 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateFHIRDatastoreResponseTypeDef = TypedDict(
-    "CreateFHIRDatastoreResponseTypeDef",
-    {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DatastoreFilterTypeDef = TypedDict(
-    "DatastoreFilterTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "DatastoreName": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
-DeleteFHIRDatastoreResponseTypeDef = TypedDict(
-    "DeleteFHIRDatastoreResponseTypeDef",
-    {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -183,149 +166,167 @@
     "_OptionalKmsEncryptionConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class KmsEncryptionConfigTypeDef(
     _RequiredKmsEncryptionConfigTypeDef, _OptionalKmsEncryptionConfigTypeDef
 ):
     pass
 
-_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
+
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "DatastoreId": str,
+        "ResourceARN": str,
     },
 )
-_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
+
+S3ConfigurationTypeDef = TypedDict(
+    "S3ConfigurationTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
+        "S3Uri": str,
+        "KmsKeyId": str,
     },
-    total=False,
 )
 
-class ListFHIRExportJobsRequestRequestTypeDef(
-    _RequiredListFHIRExportJobsRequestRequestTypeDef,
-    _OptionalListFHIRExportJobsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "DatastoreId": str,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
-_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmittedBefore": Union[datetime, str],
-        "SubmittedAfter": Union[datetime, str],
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
-    total=False,
 )
 
-class ListFHIRImportJobsRequestRequestTypeDef(
-    _RequiredListFHIRImportJobsRequestRequestTypeDef,
-    _OptionalListFHIRImportJobsRequestRequestTypeDef,
-):
-    pass
-
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+CreateFHIRDatastoreResponseTypeDef = TypedDict(
+    "CreateFHIRDatastoreResponseTypeDef",
     {
-        "ResourceARN": str,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-S3ConfigurationTypeDef = TypedDict(
-    "S3ConfigurationTypeDef",
+DeleteFHIRDatastoreResponseTypeDef = TypedDict(
+    "DeleteFHIRDatastoreResponseTypeDef",
     {
-        "S3Uri": str,
-        "KmsKeyId": str,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRExportJobResponseTypeDef = TypedDict(
     "StartFHIRExportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRImportJobResponseTypeDef = TypedDict(
     "StartFHIRImportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+DatastoreFilterTypeDef = TypedDict(
+    "DatastoreFilterTypeDef",
     {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
+        "DatastoreName": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRExportJobsRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DatastoreId": str,
     },
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRExportJobsRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "NextToken": str,
+        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
     },
+    total=False,
 )
 
-ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
-    "ListFHIRDatastoresRequestRequestTypeDef",
+
+class ListFHIRExportJobsRequestRequestTypeDef(
+    _RequiredListFHIRExportJobsRequestRequestTypeDef,
+    _OptionalListFHIRExportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFHIRImportJobsRequestRequestTypeDef",
+    {
+        "DatastoreId": str,
+    },
+)
+_OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFHIRImportJobsRequestRequestTypeDef",
     {
-        "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmittedBefore": TimestampTypeDef,
+        "SubmittedAfter": TimestampTypeDef,
     },
     total=False,
 )
 
+
+class ListFHIRImportJobsRequestRequestTypeDef(
+    _RequiredListFHIRImportJobsRequestRequestTypeDef,
+    _OptionalListFHIRImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
@@ -333,14 +334,24 @@
     "OutputDataConfigTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
+ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
+    "ListFHIRDatastoresRequestRequestTypeDef",
+    {
+        "Filter": DatastoreFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 _RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreTypeVersion": Literal["R4"],
     },
 )
 _OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
@@ -352,20 +363,22 @@
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFHIRDatastoreRequestRequestTypeDef(
     _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
     _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDatastorePropertiesTypeDef = TypedDict(
     "_RequiredDatastorePropertiesTypeDef",
     {
         "DatastoreId": str,
         "DatastoreArn": str,
         "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
@@ -380,19 +393,21 @@
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DatastorePropertiesTypeDef(
     _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
 ):
     pass
 
+
 _RequiredExportJobPropertiesTypeDef = TypedDict(
     "_RequiredExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
@@ -406,19 +421,21 @@
         "EndTime": datetime,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
+
 class ExportJobPropertiesTypeDef(
     _RequiredExportJobPropertiesTypeDef, _OptionalExportJobPropertiesTypeDef
 ):
     pass
 
+
 _RequiredImportJobPropertiesTypeDef = TypedDict(
     "_RequiredImportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
@@ -433,19 +450,21 @@
         "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
+
 class ImportJobPropertiesTypeDef(
     _RequiredImportJobPropertiesTypeDef, _OptionalImportJobPropertiesTypeDef
 ):
     pass
 
+
 _RequiredStartFHIRExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRExportJobRequestRequestTypeDef",
     {
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
         "ClientToken": str,
@@ -455,20 +474,22 @@
     "_OptionalStartFHIRExportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
+
 class StartFHIRExportJobRequestRequestTypeDef(
     _RequiredStartFHIRExportJobRequestRequestTypeDef,
     _OptionalStartFHIRExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartFHIRImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRImportJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
@@ -479,63 +500,65 @@
     "_OptionalStartFHIRImportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
+
 class StartFHIRImportJobRequestRequestTypeDef(
     _RequiredStartFHIRImportJobRequestRequestTypeDef,
     _OptionalStartFHIRImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRDatastoresResponseTypeDef = TypedDict(
     "ListFHIRDatastoresResponseTypeDef",
     {
         "DatastorePropertiesList": List[DatastorePropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRExportJobResponseTypeDef = TypedDict(
     "DescribeFHIRExportJobResponseTypeDef",
     {
         "ExportJobProperties": ExportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRExportJobsResponseTypeDef = TypedDict(
     "ListFHIRExportJobsResponseTypeDef",
     {
         "ExportJobPropertiesList": List[ExportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRImportJobResponseTypeDef = TypedDict(
     "DescribeFHIRImportJobResponseTypeDef",
     {
         "ImportJobProperties": ImportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRImportJobsResponseTypeDef = TypedDict(
     "ListFHIRImportJobsResponseTypeDef",
     {
         "ImportJobPropertiesList": List[ImportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/PKG-INFO` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-healthlake
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.HealthLake 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.HealthLake 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore healthlake type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore healthlake type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-healthlake"></a>
 
 # types-aiobotocore-healthlake
 
 [![PyPI - types-aiobotocore-healthlake](https://img.shields.io/pypi/v/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-healthlake.svg?color=blue)](https://pypi.org/project/types-aiobotocore-healthlake)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-healthlake?color=blue)](https://pypistats.org/packages/types-aiobotocore-healthlake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-healthlake)](https://pepy.tech/project/types-aiobotocore-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.HealthLake 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [types-aiobotocore-healthlake docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_healthlake/).
 
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
@@ -286,48 +285,49 @@
 )
 
 
 def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_healthlake.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
-    DatastoreFilterTypeDef,
+    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
     InputDataConfigTypeDef,
     KmsEncryptionConfigTypeDef,
-    ListFHIRExportJobsRequestRequestTypeDef,
-    ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    StartFHIRExportJobResponseTypeDef,
-    StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListFHIRDatastoresRequestRequestTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartFHIRExportJobResponseTypeDef,
+    StartFHIRImportJobResponseTypeDef,
+    DatastoreFilterTypeDef,
+    ListFHIRExportJobsRequestRequestTypeDef,
+    ListFHIRImportJobsRequestRequestTypeDef,
     SseConfigurationTypeDef,
     OutputDataConfigTypeDef,
+    ListFHIRDatastoresRequestRequestTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
@@ -335,15 +335,15 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> IdentityProviderConfigurationTypeDef:
+def get_value() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-healthlake-2.5.2/types_aiobotocore_healthlake.egg-info/SOURCES.txt` & `types-aiobotocore-healthlake-2.5.2.post1/types_aiobotocore_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-iot1click-projects-2.5.2.tar.gz` & `tmp/types-aiobotocore-iot1click-projects-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-projects-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-projects-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-iot1click-projects-2.5.2.tar` & `types-aiobotocore-iot1click-projects-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.614263 types-aiobotocore-iot1click-projects-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-07-08 01:43:44.614263 types-aiobotocore-iot1click-projects-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.614263 types-aiobotocore-iot1click-projects-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.606263 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-08 01:32:38.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.614263 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.437569 types-aiobotocore-iot1click-projects-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-08-02 14:52:24.433569 types-aiobotocore-iot1click-projects-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.437569 types-aiobotocore-iot1click-projects-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.433569 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-08-02 14:40:39.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-08-02 14:40:39.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.433569 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/LICENSE` & `types-aiobotocore-iot1click-projects-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot1click-projects type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot1click-projects"></a>
 
 # types-aiobotocore-iot1click-projects
 
 [![PyPI - types-aiobotocore-iot1click-projects](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot1click-projects?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot1click-projects)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT1ClickProjects 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
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
@@ -310,59 +309,62 @@
 )
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot1click_projects.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
+    CreateProjectRequestRequestTypeDef,
+    PlacementTemplateUnionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
+def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/README.md` & `types-aiobotocore-iot1click-projects-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iot1click-projects"></a>
 
 # types-aiobotocore-iot1click-projects
 
 [![PyPI - types-aiobotocore-iot1click-projects](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot1click-projects?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot1click-projects)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT1ClickProjects 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
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
@@ -277,59 +277,62 @@
 )
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot1click_projects.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
+    CreateProjectRequestRequestTypeDef,
+    PlacementTemplateUnionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
+def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/setup.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-projects",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore iot1click-projects type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot1click_projects": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/"
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/__init__.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/__init__.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/__main__.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/client.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .type_defs import (
     DescribePlacementResponseTypeDef,
     DescribeProjectResponseTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PlacementTemplateTypeDef,
+    PlacementTemplateUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -111,15 +111,15 @@
         """
 
     async def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateTypeDef = ...,
+        placementTemplate: PlacementTemplateUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_project)
@@ -252,15 +252,15 @@
         """
 
     async def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateTypeDef = ...
+        placementTemplate: PlacementTemplateUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/client.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .type_defs import (
     DescribePlacementResponseTypeDef,
     DescribeProjectResponseTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PlacementTemplateTypeDef,
+    PlacementTemplateUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -102,15 +102,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_placement)
         """
     async def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateTypeDef = ...,
+        placementTemplate: PlacementTemplateUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_project)
@@ -229,15 +229,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_placement)
         """
     async def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateTypeDef = ...
+        placementTemplate: PlacementTemplateUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/literals.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/literals.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/paginator.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,46 +31,42 @@
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListPlacementsPaginator", "ListProjectsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListPlacementsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listplacementspaginator)
     """
 
     def paginate(
-        self, *, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPlacementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listplacementspaginator)
         """
 
-
 class ListProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listprojectspaginator)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/paginator.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,42 +31,46 @@
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListPlacementsPaginator", "ListProjectsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListPlacementsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listplacementspaginator)
     """
 
     def paginate(
-        self, *, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPlacementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listplacementspaginator)
         """
 
+
 class ListProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/paginators/#listprojectspaginator)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/type_defs.py` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,58 +4,61 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot1click_projects.type_defs import AssociateDeviceWithPlacementRequestRequestTypeDef
 
-    data: AssociateDeviceWithPlacementRequestRequestTypeDef = {...}
+    data: AssociateDeviceWithPlacementRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
+    "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
-    "GetDevicesInPlacementResponseTypeDef",
-    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
+    "GetDevicesInPlacementResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
+    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
-    "CreateProjectRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
+    "CreateProjectRequestRequestTypeDef",
+    "PlacementTemplateUnionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -118,21 +121,41 @@
         "placementName": str,
         "attributes": Dict[str, str],
         "createdDate": datetime,
         "updatedDate": datetime,
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
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
+DeviceTemplateOutputTypeDef = TypedDict(
+    "DeviceTemplateOutputTypeDef",
+    {
+        "deviceType": str,
+        "callbackOverrides": Dict[str, str],
+    },
+    total=False,
+)
+
 DeviceTemplateTypeDef = TypedDict(
     "DeviceTemplateTypeDef",
     {
         "deviceType": str,
         "callbackOverrides": Mapping[str, str],
     },
     total=False,
@@ -151,44 +174,24 @@
     "GetDevicesInPlacementRequestRequestTypeDef",
     {
         "projectName": str,
         "placementName": str,
     },
 )
 
-GetDevicesInPlacementResponseTypeDef = TypedDict(
-    "GetDevicesInPlacementResponseTypeDef",
-    {
-        "devices": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
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
-class ListPlacementsRequestListPlacementsPaginateTypeDef(
-    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
-    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPlacementsRequestRequestTypeDef = TypedDict(
     "_RequiredListPlacementsRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListPlacementsRequestRequestTypeDef = TypedDict(
@@ -213,22 +216,14 @@
         "projectName": str,
         "placementName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -259,43 +254,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -330,94 +296,150 @@
     pass
 
 
 DescribePlacementResponseTypeDef = TypedDict(
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDevicesInPlacementResponseTypeDef = TypedDict(
+    "GetDevicesInPlacementResponseTypeDef",
+    {
+        "devices": Dict[str, str],
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
+PlacementTemplateOutputTypeDef = TypedDict(
+    "PlacementTemplateOutputTypeDef",
+    {
+        "defaultAttributes": Dict[str, str],
+        "deviceTemplates": Dict[str, DeviceTemplateOutputTypeDef],
     },
+    total=False,
 )
 
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
 )
 
+_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPlacementsRequestListPlacementsPaginateTypeDef(
+    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
+    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
+):
+    pass
+
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPlacementsResponseTypeDef = TypedDict(
     "ListPlacementsResponseTypeDef",
     {
         "placements": List[PlacementSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectRequestRequestTypeDef",
+_RequiredProjectDescriptionTypeDef = TypedDict(
+    "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
+        "createdDate": datetime,
+        "updatedDate": datetime,
     },
 )
-_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectRequestRequestTypeDef",
+_OptionalProjectDescriptionTypeDef = TypedDict(
+    "_OptionalProjectDescriptionTypeDef",
     {
+        "arn": str,
         "description": str,
-        "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Mapping[str, str],
+        "placementTemplate": PlacementTemplateOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateProjectRequestRequestTypeDef(
-    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
+class ProjectDescriptionTypeDef(
+    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
 
-_RequiredProjectDescriptionTypeDef = TypedDict(
-    "_RequiredProjectDescriptionTypeDef",
+_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
-        "createdDate": datetime,
-        "updatedDate": datetime,
     },
 )
-_OptionalProjectDescriptionTypeDef = TypedDict(
-    "_OptionalProjectDescriptionTypeDef",
+_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectRequestRequestTypeDef",
     {
-        "arn": str,
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class ProjectDescriptionTypeDef(
-    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
+class CreateProjectRequestRequestTypeDef(
+    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
+PlacementTemplateUnionTypeDef = Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef]
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -436,10 +458,10 @@
     pass
 
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "project": ProjectDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects/type_defs.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,57 +4,60 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot1click_projects.type_defs import AssociateDeviceWithPlacementRequestRequestTypeDef
 
-    data: AssociateDeviceWithPlacementRequestRequestTypeDef = {...}
+    data: AssociateDeviceWithPlacementRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
+    "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
-    "GetDevicesInPlacementResponseTypeDef",
-    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
+    "GetDevicesInPlacementResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
+    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
-    "CreateProjectRequestRequestTypeDef",
     "ProjectDescriptionTypeDef",
+    "CreateProjectRequestRequestTypeDef",
+    "PlacementTemplateUnionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -115,21 +118,41 @@
         "placementName": str,
         "attributes": Dict[str, str],
         "createdDate": datetime,
         "updatedDate": datetime,
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
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
+DeviceTemplateOutputTypeDef = TypedDict(
+    "DeviceTemplateOutputTypeDef",
+    {
+        "deviceType": str,
+        "callbackOverrides": Dict[str, str],
+    },
+    total=False,
+)
+
 DeviceTemplateTypeDef = TypedDict(
     "DeviceTemplateTypeDef",
     {
         "deviceType": str,
         "callbackOverrides": Mapping[str, str],
     },
     total=False,
@@ -148,42 +171,24 @@
     "GetDevicesInPlacementRequestRequestTypeDef",
     {
         "projectName": str,
         "placementName": str,
     },
 )
 
-GetDevicesInPlacementResponseTypeDef = TypedDict(
-    "GetDevicesInPlacementResponseTypeDef",
-    {
-        "devices": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
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
 
-class ListPlacementsRequestListPlacementsPaginateTypeDef(
-    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
-    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPlacementsRequestRequestTypeDef = TypedDict(
     "_RequiredListPlacementsRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListPlacementsRequestRequestTypeDef = TypedDict(
@@ -206,22 +211,14 @@
         "projectName": str,
         "placementName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -250,43 +247,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -319,90 +287,144 @@
 ):
     pass
 
 DescribePlacementResponseTypeDef = TypedDict(
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDevicesInPlacementResponseTypeDef = TypedDict(
+    "GetDevicesInPlacementResponseTypeDef",
+    {
+        "devices": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PlacementTemplateOutputTypeDef = TypedDict(
+    "PlacementTemplateOutputTypeDef",
+    {
+        "defaultAttributes": Dict[str, str],
+        "deviceTemplates": Dict[str, DeviceTemplateOutputTypeDef],
+    },
+    total=False,
+)
+
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
 )
 
+_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPlacementsRequestListPlacementsPaginateTypeDef(
+    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
+    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
+):
+    pass
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPlacementsResponseTypeDef = TypedDict(
     "ListPlacementsResponseTypeDef",
     {
         "placements": List[PlacementSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectRequestRequestTypeDef",
+_RequiredProjectDescriptionTypeDef = TypedDict(
+    "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
+        "createdDate": datetime,
+        "updatedDate": datetime,
     },
 )
-_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectRequestRequestTypeDef",
+_OptionalProjectDescriptionTypeDef = TypedDict(
+    "_OptionalProjectDescriptionTypeDef",
     {
+        "arn": str,
         "description": str,
-        "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Mapping[str, str],
+        "placementTemplate": PlacementTemplateOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateProjectRequestRequestTypeDef(
-    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
+class ProjectDescriptionTypeDef(
+    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
-_RequiredProjectDescriptionTypeDef = TypedDict(
-    "_RequiredProjectDescriptionTypeDef",
+_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
-        "createdDate": datetime,
-        "updatedDate": datetime,
     },
 )
-_OptionalProjectDescriptionTypeDef = TypedDict(
-    "_OptionalProjectDescriptionTypeDef",
+_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectRequestRequestTypeDef",
     {
-        "arn": str,
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class ProjectDescriptionTypeDef(
-    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
+class CreateProjectRequestRequestTypeDef(
+    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+PlacementTemplateUnionTypeDef = Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef]
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -419,10 +441,10 @@
 ):
     pass
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "project": ProjectDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot1click-projects type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot1click-projects"></a>
 
 # types-aiobotocore-iot1click-projects
 
 [![PyPI - types-aiobotocore-iot1click-projects](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-projects.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot1click-projects?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot1click-projects)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-projects)](https://pepy.tech/project/types-aiobotocore-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT1ClickProjects 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
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
@@ -310,59 +309,62 @@
 )
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot1click_projects.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
+    DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ProjectDescriptionTypeDef,
+    CreateProjectRequestRequestTypeDef,
+    PlacementTemplateUnionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
+def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*


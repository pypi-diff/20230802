# Comparing `tmp/types-aiobotocore-arc-zonal-shift-2.5.2.tar.gz` & `tmp/types-aiobotocore-arc-zonal-shift-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-arc-zonal-shift-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
```

## Comparing `types-aiobotocore-arc-zonal-shift-2.5.2.tar` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.729697 types-aiobotocore-arc-zonal-shift-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14186 2023-07-08 01:43:14.729697 types-aiobotocore-arc-zonal-shift-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.729697 types-aiobotocore-arc-zonal-shift-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.721696 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-08 01:26:03.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:02.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.729697 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14186 2023-07-08 01:43:14.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:43:14.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:14.000000 types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.985653 types-aiobotocore-arc-zonal-shift-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-08-02 14:51:52.981654 types-aiobotocore-arc-zonal-shift-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.985653 types-aiobotocore-arc-zonal-shift-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.981654 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-02 14:33:30.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-02 14:33:30.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:29.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.981654 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:51:52.000000 types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/LICENSE` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore arc-zonal-shift type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-arc-zonal-shift"></a>
 
 # types-aiobotocore-arc-zonal-shift
 
 [![PyPI - types-aiobotocore-arc-zonal-shift](https://img.shields.io/pypi/v/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-arc-zonal-shift?color=blue)](https://pypistats.org/packages/types-aiobotocore-arc-zonal-shift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ARCZonalShift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
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
@@ -316,44 +315,44 @@
 )
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_arc_zonal_shift.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
+def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/README.md` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-arc-zonal-shift"></a>
 
 # types-aiobotocore-arc-zonal-shift
 
 [![PyPI - types-aiobotocore-arc-zonal-shift](https://img.shields.io/pypi/v/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-arc-zonal-shift?color=blue)](https://pypistats.org/packages/types-aiobotocore-arc-zonal-shift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ARCZonalShift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
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
@@ -283,44 +283,44 @@
 )
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_arc_zonal_shift.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
+def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/setup.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-arc-zonal-shift",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with"
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
-    keywords="aiobotocore arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore arc-zonal-shift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_arc_zonal_shift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/"
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/__init__.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/__init__.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/__main__.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ARCZonalShift 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ARCZonalShift 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/client.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/client.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/literals.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/literals.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/paginator.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,31 +50,28 @@
 class ListManagedResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
         """
 
 
 class ListZonalShiftsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listzonalshiftspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: ZonalShiftStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: ZonalShiftStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/paginator.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -47,30 +47,27 @@
 class ListManagedResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
         """
 
 class ListZonalShiftsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listzonalshiftspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: ZonalShiftStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: ZonalShiftStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/type_defs.py` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -4,45 +4,44 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
-    data: CancelZonalShiftRequestRequestTypeDef = {...}
+    data: CancelZonalShiftRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import AppliedStatusType, ZonalShiftStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelZonalShiftRequestRequestTypeDef",
     "GetManagedResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ZonalShiftInResourceTypeDef",
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListManagedResourcesRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListZonalShiftsRequestRequestTypeDef",
     "ZonalShiftSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartZonalShiftRequestRequestTypeDef",
     "UpdateZonalShiftRequestRequestTypeDef",
     "ZonalShiftTypeDef",
     "GetManagedResourceResponseTypeDef",
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListManagedResourcesResponseTypeDef",
     "ListZonalShiftsResponseTypeDef",
 )
 
 CancelZonalShiftRequestRequestTypeDef = TypedDict(
     "CancelZonalShiftRequestRequestTypeDef",
     {
@@ -53,31 +52,44 @@
 GetManagedResourceRequestRequestTypeDef = TypedDict(
     "GetManagedResourceRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
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
 ZonalShiftInResourceTypeDef = TypedDict(
     "ZonalShiftInResourceTypeDef",
     {
         "appliedStatus": AppliedStatusType,
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "zonalShiftId": str,
     },
 )
 
-ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
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
 
 ListManagedResourcesRequestRequestTypeDef = TypedDict(
     "ListManagedResourcesRequestRequestTypeDef",
     {
@@ -98,30 +110,19 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
-
 class ManagedResourceSummaryTypeDef(
     _RequiredManagedResourceSummaryTypeDef, _OptionalManagedResourceSummaryTypeDef
 ):
     pass
 
-
-ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
-    {
-        "status": ZonalShiftStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListZonalShiftsRequestRequestTypeDef = TypedDict(
     "ListZonalShiftsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "status": ZonalShiftStatusType,
     },
@@ -137,35 +138,14 @@
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
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
 StartZonalShiftRequestRequestTypeDef = TypedDict(
     "StartZonalShiftRequestRequestTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiresIn": str,
         "resourceIdentifier": str,
@@ -183,56 +163,71 @@
     {
         "comment": str,
         "expiresIn": str,
     },
     total=False,
 )
 
-
 class UpdateZonalShiftRequestRequestTypeDef(
     _RequiredUpdateZonalShiftRequestRequestTypeDef, _OptionalUpdateZonalShiftRequestRequestTypeDef
 ):
     pass
 
-
 ZonalShiftTypeDef = TypedDict(
     "ZonalShiftTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetManagedResourceResponseTypeDef = TypedDict(
     "GetManagedResourceResponseTypeDef",
     {
         "appliedWeights": Dict[str, float],
         "arn": str,
         "name": str,
         "zonalShifts": List[ZonalShiftInResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
+    {
+        "status": ZonalShiftStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListManagedResourcesResponseTypeDef = TypedDict(
     "ListManagedResourcesResponseTypeDef",
     {
         "items": List[ManagedResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListZonalShiftsResponseTypeDef = TypedDict(
     "ListZonalShiftsResponseTypeDef",
     {
         "items": List[ZonalShiftSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift/type_defs.pyi` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_arc_zonal_shift.type_defs import CancelZonalShiftRequestRequestTypeDef
 
-    data: CancelZonalShiftRequestRequestTypeDef = {...}
+    data: CancelZonalShiftRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import AppliedStatusType, ZonalShiftStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelZonalShiftRequestRequestTypeDef",
     "GetManagedResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ZonalShiftInResourceTypeDef",
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListManagedResourcesRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListZonalShiftsRequestRequestTypeDef",
     "ZonalShiftSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartZonalShiftRequestRequestTypeDef",
     "UpdateZonalShiftRequestRequestTypeDef",
     "ZonalShiftTypeDef",
     "GetManagedResourceResponseTypeDef",
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListManagedResourcesResponseTypeDef",
     "ListZonalShiftsResponseTypeDef",
 )
 
 CancelZonalShiftRequestRequestTypeDef = TypedDict(
     "CancelZonalShiftRequestRequestTypeDef",
     {
@@ -52,31 +53,44 @@
 GetManagedResourceRequestRequestTypeDef = TypedDict(
     "GetManagedResourceRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
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
 ZonalShiftInResourceTypeDef = TypedDict(
     "ZonalShiftInResourceTypeDef",
     {
         "appliedStatus": AppliedStatusType,
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "zonalShiftId": str,
     },
 )
 
-ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
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
 
 ListManagedResourcesRequestRequestTypeDef = TypedDict(
     "ListManagedResourcesRequestRequestTypeDef",
     {
@@ -97,27 +111,20 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
+
 class ManagedResourceSummaryTypeDef(
     _RequiredManagedResourceSummaryTypeDef, _OptionalManagedResourceSummaryTypeDef
 ):
     pass
 
-ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
-    {
-        "status": ZonalShiftStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListZonalShiftsRequestRequestTypeDef = TypedDict(
     "ListZonalShiftsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "status": ZonalShiftStatusType,
@@ -134,35 +141,14 @@
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
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
 StartZonalShiftRequestRequestTypeDef = TypedDict(
     "StartZonalShiftRequestRequestTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiresIn": str,
         "resourceIdentifier": str,
@@ -180,54 +166,73 @@
     {
         "comment": str,
         "expiresIn": str,
     },
     total=False,
 )
 
+
 class UpdateZonalShiftRequestRequestTypeDef(
     _RequiredUpdateZonalShiftRequestRequestTypeDef, _OptionalUpdateZonalShiftRequestRequestTypeDef
 ):
     pass
 
+
 ZonalShiftTypeDef = TypedDict(
     "ZonalShiftTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetManagedResourceResponseTypeDef = TypedDict(
     "GetManagedResourceResponseTypeDef",
     {
         "appliedWeights": Dict[str, float],
         "arn": str,
         "name": str,
         "zonalShifts": List[ZonalShiftInResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
+    {
+        "status": ZonalShiftStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListManagedResourcesResponseTypeDef = TypedDict(
     "ListManagedResourcesResponseTypeDef",
     {
         "items": List[ManagedResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListZonalShiftsResponseTypeDef = TypedDict(
     "ListZonalShiftsResponseTypeDef",
     {
         "items": List[ZonalShiftSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-arc-zonal-shift
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ARCZonalShift 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore arc-zonal-shift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore arc-zonal-shift type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-arc-zonal-shift"></a>
 
 # types-aiobotocore-arc-zonal-shift
 
 [![PyPI - types-aiobotocore-arc-zonal-shift](https://img.shields.io/pypi/v/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-arc-zonal-shift?color=blue)](https://pypistats.org/packages/types-aiobotocore-arc-zonal-shift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-arc-zonal-shift)](https://pepy.tech/project/types-aiobotocore-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ARCZonalShift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [types-aiobotocore-arc-zonal-shift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_arc_zonal_shift/).
 
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
@@ -316,44 +315,44 @@
 )
 
 
 def check_value(value: AppliedStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_arc_zonal_shift.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
+def get_value() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-arc-zonal-shift-2.5.2/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt` & `types-aiobotocore-arc-zonal-shift-2.5.2.post1/types_aiobotocore_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-codestar-2.5.2.tar.gz` & `tmp/types-aiobotocore-codestar-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-2.5.2.tar", last modified: Sat Jul  8 01:43:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
```

## Comparing `types-aiobotocore-codestar-2.5.2.tar` & `types-aiobotocore-codestar-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.049911 types-aiobotocore-codestar-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-07-08 01:43:26.049911 types-aiobotocore-codestar-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:26.049911 types-aiobotocore-codestar-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.049911 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17177 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-08 01:27:41.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:40.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:26.049911 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:25.000000 types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17177 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-2.5.2/LICENSE` & `types-aiobotocore-codestar-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/PKG-INFO` & `types-aiobotocore-codestar-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codestar type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar)](https://pepy.tech/project/types-aiobotocore-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStar 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
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
@@ -319,79 +318,79 @@
 )
 
 
 def check_value(value: ListProjectsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
+    ResponseMetadataTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
-    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
-    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
-    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
-    ListTagsForProjectResultTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
-    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
+    AssociateTeamMemberResultTypeDef,
+    CreateProjectResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DeleteProjectResultTypeDef,
+    DeleteUserProfileResultTypeDef,
+    DescribeUserProfileResultTypeDef,
+    ListTagsForProjectResultTypeDef,
+    TagProjectResultTypeDef,
+    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateTeamMemberRequestRequestTypeDef:
+def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-2.5.2/README.md` & `types-aiobotocore-codestar-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar)](https://pepy.tech/project/types-aiobotocore-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStar 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
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
@@ -286,79 +286,79 @@
 )
 
 
 def check_value(value: ListProjectsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
+    ResponseMetadataTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
-    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
-    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
-    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
-    ListTagsForProjectResultTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
-    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
+    AssociateTeamMemberResultTypeDef,
+    CreateProjectResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DeleteProjectResultTypeDef,
+    DeleteUserProfileResultTypeDef,
+    DescribeUserProfileResultTypeDef,
+    ListTagsForProjectResultTypeDef,
+    TagProjectResultTypeDef,
+    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateTeamMemberRequestRequestTypeDef:
+def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-2.5.2/setup.py` & `types-aiobotocore-codestar-2.5.2.post1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codestar"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore codestar type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codestar type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codestar": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/"
```

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/__init__.py` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/__init__.pyi` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/__main__.py` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStar 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeStar 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar\nOther"
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

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/client.py` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/client.pyi` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/literals.py` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/literals.pyi` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/paginator.py` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,58 +60,58 @@
 class ListProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listprojectspaginator)
         """
 
 
 class ListResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listresourcespaginator)
         """
 
 
 class ListTeamMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listteammemberspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTeamMembersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listteammemberspaginator)
         """
 
 
 class ListUserProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listuserprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listuserprofilespaginator)
         """
```

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/paginator.pyi` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -57,55 +57,55 @@
 class ListProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listprojectspaginator)
         """
 
 class ListResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listresourcespaginator)
         """
 
 class ListTeamMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listteammemberspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTeamMembersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listteammemberspaginator)
         """
 
 class ListUserProfilesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listuserprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUserProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/paginators/#listuserprofilespaginator)
         """
```

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/type_defs.py` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,73 +4,73 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef
 
-    data: AssociateTeamMemberRequestRequestTypeDef = {...}
+    data: AssociateTeamMemberRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
-    "AssociateTeamMemberResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
-    "CreateProjectResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
-    "CreateUserProfileResultTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResultTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
-    "DeleteUserProfileResultTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ProjectStatusTypeDef",
     "DescribeUserProfileRequestRequestTypeDef",
-    "DescribeUserProfileResultTypeDef",
     "DisassociateTeamMemberRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForProjectRequestRequestTypeDef",
-    "ListTagsForProjectResultTypeDef",
-    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
     "ListTeamMembersRequestRequestTypeDef",
     "TeamMemberTypeDef",
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagProjectRequestRequestTypeDef",
-    "TagProjectResultTypeDef",
     "UntagProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateTeamMemberRequestRequestTypeDef",
-    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
+    "AssociateTeamMemberResultTypeDef",
+    "CreateProjectResultTypeDef",
+    "CreateUserProfileResultTypeDef",
+    "DeleteProjectResultTypeDef",
+    "DeleteUserProfileResultTypeDef",
+    "DescribeUserProfileResultTypeDef",
+    "ListTagsForProjectResultTypeDef",
+    "TagProjectResultTypeDef",
+    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileResultTypeDef",
     "CodeDestinationTypeDef",
     "CodeSourceTypeDef",
     "ToolchainSourceTypeDef",
     "DescribeProjectResultTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
+    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "ListResourcesResultTypeDef",
     "ListTeamMembersResultTypeDef",
     "ListUserProfilesResultTypeDef",
     "CodeTypeDef",
     "ToolchainTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -97,19 +97,22 @@
 class AssociateTeamMemberRequestRequestTypeDef(
     _RequiredAssociateTeamMemberRequestRequestTypeDef,
     _OptionalAssociateTeamMemberRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateTeamMemberResultTypeDef = TypedDict(
-    "AssociateTeamMemberResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "clientRequestToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CodeCommitCodeDestinationTypeDef = TypedDict(
     "CodeCommitCodeDestinationTypeDef",
     {
         "name": str,
@@ -147,25 +150,14 @@
     {
         "bucketName": str,
         "bucketKey": str,
     },
     total=False,
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "clientRequestToken": str,
-        "projectTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
     },
@@ -181,27 +173,14 @@
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -216,38 +195,21 @@
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
 
-DeleteProjectResultTypeDef = TypedDict(
-    "DeleteProjectResultTypeDef",
-    {
-        "stackId": str,
-        "projectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DeleteUserProfileResultTypeDef = TypedDict(
-    "DeleteUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -273,39 +235,28 @@
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DescribeUserProfileResultTypeDef = TypedDict(
-    "DescribeUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateTeamMemberRequestRequestTypeDef = TypedDict(
     "DisassociateTeamMemberRequestRequestTypeDef",
     {
         "projectId": str,
         "userArn": str,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
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
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
@@ -320,36 +271,14 @@
     {
         "projectId": str,
         "projectArn": str,
     },
     total=False,
 )
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -394,45 +323,14 @@
 class ListTagsForProjectRequestRequestTypeDef(
     _RequiredListTagsForProjectRequestRequestTypeDef,
     _OptionalListTagsForProjectRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForProjectResultTypeDef = TypedDict(
-    "ListTagsForProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
-    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTeamMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListTeamMembersRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListTeamMembersRequestRequestTypeDef = TypedDict(
@@ -467,22 +365,14 @@
 )
 
 
 class TeamMemberTypeDef(_RequiredTeamMemberTypeDef, _OptionalTeamMemberTypeDef):
     pass
 
 
-ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUserProfilesRequestRequestTypeDef = TypedDict(
     "ListUserProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -495,51 +385,22 @@
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
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
 TagProjectRequestRequestTypeDef = TypedDict(
     "TagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Mapping[str, str],
     },
 )
 
-TagProjectResultTypeDef = TypedDict(
-    "TagProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagProjectRequestRequestTypeDef = TypedDict(
     "UntagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Sequence[str],
     },
 )
@@ -585,24 +446,14 @@
 
 class UpdateTeamMemberRequestRequestTypeDef(
     _RequiredUpdateTeamMemberRequestRequestTypeDef, _OptionalUpdateTeamMemberRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTeamMemberResultTypeDef = TypedDict(
-    "UpdateTeamMemberResultTypeDef",
-    {
-        "userArn": str,
-        "projectRole": str,
-        "remoteAccessAllowed": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -618,24 +469,113 @@
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
+AssociateTeamMemberResultTypeDef = TypedDict(
+    "AssociateTeamMemberResultTypeDef",
+    {
+        "clientRequestToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "clientRequestToken": str,
+        "projectTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResultTypeDef = TypedDict(
+    "DeleteProjectResultTypeDef",
+    {
+        "stackId": str,
+        "projectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteUserProfileResultTypeDef = TypedDict(
+    "DeleteUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserProfileResultTypeDef = TypedDict(
+    "DescribeUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForProjectResultTypeDef = TypedDict(
+    "ListTagsForProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagProjectResultTypeDef = TypedDict(
+    "TagProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTeamMemberResultTypeDef = TypedDict(
+    "UpdateTeamMemberResultTypeDef",
+    {
+        "userArn": str,
+        "projectRole": str,
+        "remoteAccessAllowed": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateUserProfileResultTypeDef = TypedDict(
     "UpdateUserProfileResultTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeDestinationTypeDef = TypedDict(
     "CodeDestinationTypeDef",
     {
         "codeCommit": CodeCommitCodeDestinationTypeDef,
@@ -666,51 +606,111 @@
         "arn": str,
         "description": str,
         "clientRequestToken": str,
         "createdTimeStamp": datetime,
         "stackId": str,
         "projectTemplateId": str,
         "status": ProjectStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
+    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
+):
+    pass
+
+
+ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResultTypeDef = TypedDict(
     "ListResourcesResultTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTeamMembersResultTypeDef = TypedDict(
     "ListTeamMembersResultTypeDef",
     {
         "teamMembers": List[TeamMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserProfilesResultTypeDef = TypedDict(
     "ListUserProfilesResultTypeDef",
     {
         "userProfiles": List[UserProfileSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeTypeDef = TypedDict(
     "CodeTypeDef",
     {
         "source": CodeSourceTypeDef,
```

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar/type_defs.pyi` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,72 +4,72 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef
 
-    data: AssociateTeamMemberRequestRequestTypeDef = {...}
+    data: AssociateTeamMemberRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
-    "AssociateTeamMemberResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
-    "CreateProjectResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
-    "CreateUserProfileResultTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResultTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
-    "DeleteUserProfileResultTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ProjectStatusTypeDef",
     "DescribeUserProfileRequestRequestTypeDef",
-    "DescribeUserProfileResultTypeDef",
     "DisassociateTeamMemberRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForProjectRequestRequestTypeDef",
-    "ListTagsForProjectResultTypeDef",
-    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
     "ListTeamMembersRequestRequestTypeDef",
     "TeamMemberTypeDef",
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagProjectRequestRequestTypeDef",
-    "TagProjectResultTypeDef",
     "UntagProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateTeamMemberRequestRequestTypeDef",
-    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
+    "AssociateTeamMemberResultTypeDef",
+    "CreateProjectResultTypeDef",
+    "CreateUserProfileResultTypeDef",
+    "DeleteProjectResultTypeDef",
+    "DeleteUserProfileResultTypeDef",
+    "DescribeUserProfileResultTypeDef",
+    "ListTagsForProjectResultTypeDef",
+    "TagProjectResultTypeDef",
+    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileResultTypeDef",
     "CodeDestinationTypeDef",
     "CodeSourceTypeDef",
     "ToolchainSourceTypeDef",
     "DescribeProjectResultTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
+    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "ListResourcesResultTypeDef",
     "ListTeamMembersResultTypeDef",
     "ListUserProfilesResultTypeDef",
     "CodeTypeDef",
     "ToolchainTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -94,19 +94,22 @@
 
 class AssociateTeamMemberRequestRequestTypeDef(
     _RequiredAssociateTeamMemberRequestRequestTypeDef,
     _OptionalAssociateTeamMemberRequestRequestTypeDef,
 ):
     pass
 
-AssociateTeamMemberResultTypeDef = TypedDict(
-    "AssociateTeamMemberResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "clientRequestToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CodeCommitCodeDestinationTypeDef = TypedDict(
     "CodeCommitCodeDestinationTypeDef",
     {
         "name": str,
@@ -142,25 +145,14 @@
     {
         "bucketName": str,
         "bucketKey": str,
     },
     total=False,
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "clientRequestToken": str,
-        "projectTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
     },
@@ -174,27 +166,14 @@
 )
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -207,38 +186,21 @@
 )
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-DeleteProjectResultTypeDef = TypedDict(
-    "DeleteProjectResultTypeDef",
-    {
-        "stackId": str,
-        "projectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DeleteUserProfileResultTypeDef = TypedDict(
-    "DeleteUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -262,39 +224,28 @@
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DescribeUserProfileResultTypeDef = TypedDict(
-    "DescribeUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateTeamMemberRequestRequestTypeDef = TypedDict(
     "DisassociateTeamMemberRequestRequestTypeDef",
     {
         "projectId": str,
         "userArn": str,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
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
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
@@ -309,34 +260,14 @@
     {
         "projectId": str,
         "projectArn": str,
     },
     total=False,
 )
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -377,43 +308,14 @@
 
 class ListTagsForProjectRequestRequestTypeDef(
     _RequiredListTagsForProjectRequestRequestTypeDef,
     _OptionalListTagsForProjectRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForProjectResultTypeDef = TypedDict(
-    "ListTagsForProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
-    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListTeamMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListTeamMembersRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListTeamMembersRequestRequestTypeDef = TypedDict(
@@ -444,22 +346,14 @@
     },
     total=False,
 )
 
 class TeamMemberTypeDef(_RequiredTeamMemberTypeDef, _OptionalTeamMemberTypeDef):
     pass
 
-ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUserProfilesRequestRequestTypeDef = TypedDict(
     "ListUserProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -472,51 +366,22 @@
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
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
 TagProjectRequestRequestTypeDef = TypedDict(
     "TagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Mapping[str, str],
     },
 )
 
-TagProjectResultTypeDef = TypedDict(
-    "TagProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagProjectRequestRequestTypeDef = TypedDict(
     "UntagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Sequence[str],
     },
 )
@@ -558,24 +423,14 @@
 )
 
 class UpdateTeamMemberRequestRequestTypeDef(
     _RequiredUpdateTeamMemberRequestRequestTypeDef, _OptionalUpdateTeamMemberRequestRequestTypeDef
 ):
     pass
 
-UpdateTeamMemberResultTypeDef = TypedDict(
-    "UpdateTeamMemberResultTypeDef",
-    {
-        "userArn": str,
-        "projectRole": str,
-        "remoteAccessAllowed": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -589,24 +444,113 @@
 )
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
+AssociateTeamMemberResultTypeDef = TypedDict(
+    "AssociateTeamMemberResultTypeDef",
+    {
+        "clientRequestToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "clientRequestToken": str,
+        "projectTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResultTypeDef = TypedDict(
+    "DeleteProjectResultTypeDef",
+    {
+        "stackId": str,
+        "projectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteUserProfileResultTypeDef = TypedDict(
+    "DeleteUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserProfileResultTypeDef = TypedDict(
+    "DescribeUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForProjectResultTypeDef = TypedDict(
+    "ListTagsForProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagProjectResultTypeDef = TypedDict(
+    "TagProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTeamMemberResultTypeDef = TypedDict(
+    "UpdateTeamMemberResultTypeDef",
+    {
+        "userArn": str,
+        "projectRole": str,
+        "remoteAccessAllowed": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateUserProfileResultTypeDef = TypedDict(
     "UpdateUserProfileResultTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeDestinationTypeDef = TypedDict(
     "CodeDestinationTypeDef",
     {
         "codeCommit": CodeCommitCodeDestinationTypeDef,
@@ -637,51 +581,107 @@
         "arn": str,
         "description": str,
         "clientRequestToken": str,
         "createdTimeStamp": datetime,
         "stackId": str,
         "projectTemplateId": str,
         "status": ProjectStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
+    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
+):
+    pass
+
+ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResultTypeDef = TypedDict(
     "ListResourcesResultTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTeamMembersResultTypeDef = TypedDict(
     "ListTeamMembersResultTypeDef",
     {
         "teamMembers": List[TeamMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserProfilesResultTypeDef = TypedDict(
     "ListUserProfilesResultTypeDef",
     {
         "userProfiles": List[UserProfileSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeTypeDef = TypedDict(
     "CodeTypeDef",
     {
         "source": CodeSourceTypeDef,
```

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/PKG-INFO` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codestar type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codestar?color=blue)](https://pypistats.org/packages/types-aiobotocore-codestar)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codestar)](https://pepy.tech/project/types-aiobotocore-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeStar 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
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
@@ -319,79 +318,79 @@
 )
 
 
 def check_value(value: ListProjectsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codestar.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
+    ResponseMetadataTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
-    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
-    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
-    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
-    ListTagsForProjectResultTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
-    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
+    AssociateTeamMemberResultTypeDef,
+    CreateProjectResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DeleteProjectResultTypeDef,
+    DeleteUserProfileResultTypeDef,
+    DescribeUserProfileResultTypeDef,
+    ListTagsForProjectResultTypeDef,
+    TagProjectResultTypeDef,
+    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateTeamMemberRequestRequestTypeDef:
+def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codestar-2.5.2/types_aiobotocore_codestar.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/SOURCES.txt`

 * *Files identical despite different names*


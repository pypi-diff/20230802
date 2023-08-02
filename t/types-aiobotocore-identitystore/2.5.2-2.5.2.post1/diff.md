# Comparing `tmp/types-aiobotocore-identitystore-2.5.2.tar.gz` & `tmp/types-aiobotocore-identitystore-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-identitystore-2.5.2.tar", last modified: Sat Jul  8 01:43:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-identitystore-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:23 2023, max compression
```

## Comparing `types-aiobotocore-identitystore-2.5.2.tar` & `types-aiobotocore-identitystore-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:43.738247 types-aiobotocore-identitystore-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-07-08 01:43:43.738247 types-aiobotocore-identitystore-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:43.738247 types-aiobotocore-identitystore-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:43.738247 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-07-08 01:32:08.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-07-08 01:32:08.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-08 01:32:08.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-08 01:32:08.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-08 01:32:08.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-08 01:32:08.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-07-08 01:32:09.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-07-08 01:32:09.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:07.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:43.738247 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-07-08 01:43:43.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:43:43.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:43.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:43.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:43.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:43.000000 types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.861570 types-aiobotocore-identitystore-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-08-02 14:52:23.857570 types-aiobotocore-identitystore-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:23.861570 types-aiobotocore-identitystore-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.857570 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:07.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.857570 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-08-02 14:52:23.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:23.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:23.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:23.000000 types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-identitystore-2.5.2/LICENSE` & `types-aiobotocore-identitystore-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/PKG-INFO` & `types-aiobotocore-identitystore-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-identitystore
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IdentityStore 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IdentityStore 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore identitystore type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore identitystore type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-identitystore"></a>
 
 # types-aiobotocore-identitystore
 
 [![PyPI - types-aiobotocore-identitystore](https://img.shields.io/pypi/v/types-aiobotocore-identitystore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-identitystore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-identitystore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-identitystore?color=blue)](https://pypistats.org/packages/types-aiobotocore-identitystore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-identitystore)](https://pepy.tech/project/types-aiobotocore-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IdentityStore 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [types-aiobotocore-identitystore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/).
 
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
@@ -320,80 +319,80 @@
 )
 
 
 def check_value(value: ListGroupMembershipsForMemberPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_identitystore.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_identitystore.type_defs import (
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    CreateGroupMembershipResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
-    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
     DescribeGroupRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     FilterTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeGroupResponseTypeDef,
+    ListGroupMembershipsRequestRequestTypeDef,
     GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
     GroupMembershipExistenceResultTypeDef,
     GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
+    CreateGroupMembershipResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
+    DescribeGroupResponseTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-identitystore-2.5.2/README.md` & `types-aiobotocore-identitystore-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-identitystore"></a>
 
 # types-aiobotocore-identitystore
 
 [![PyPI - types-aiobotocore-identitystore](https://img.shields.io/pypi/v/types-aiobotocore-identitystore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-identitystore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-identitystore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-identitystore?color=blue)](https://pypistats.org/packages/types-aiobotocore-identitystore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-identitystore)](https://pepy.tech/project/types-aiobotocore-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IdentityStore 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [types-aiobotocore-identitystore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/).
 
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
@@ -287,80 +287,80 @@
 )
 
 
 def check_value(value: ListGroupMembershipsForMemberPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_identitystore.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_identitystore.type_defs import (
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    CreateGroupMembershipResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
-    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
     DescribeGroupRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     FilterTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeGroupResponseTypeDef,
+    ListGroupMembershipsRequestRequestTypeDef,
     GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
     GroupMembershipExistenceResultTypeDef,
     GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
+    CreateGroupMembershipResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
+    DescribeGroupResponseTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-identitystore-2.5.2/setup.py` & `types-aiobotocore-identitystore-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-identitystore",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_identitystore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IdentityStore 2.5.2 service generated with"
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
-    keywords="aiobotocore identitystore type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore identitystore type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_identitystore": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/"
```

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/__init__.py` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/__init__.pyi` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/__main__.py` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IdentityStore 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IdentityStore 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore\nOther"
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

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/client.py` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/client.pyi` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/literals.py` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/literals.pyi` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/paginator.py` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,15 @@
 class ListGroupMembershipsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        IdentityStoreId: str,
-        GroupId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IdentityStoreId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupmembershipspaginator)
         """
 
 
@@ -85,15 +81,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         MemberId: MemberIdTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupMembershipsForMemberResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupmembershipsformemberpaginator)
         """
 
 
@@ -104,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupspaginator)
         """
 
 
@@ -123,13 +119,13 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/paginator.pyi` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,15 @@
 class ListGroupMembershipsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        IdentityStoreId: str,
-        GroupId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IdentityStoreId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupmembershipspaginator)
         """
 
 class ListGroupMembershipsForMemberPaginator(AioPaginator):
@@ -81,15 +77,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         MemberId: MemberIdTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupMembershipsForMemberResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupmembershipsformemberpaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
@@ -99,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listgroupspaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
@@ -117,13 +113,13 @@
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/type_defs.py` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_identitystore.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -22,55 +22,55 @@
 
 __all__ = (
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
-    "CreateGroupMembershipResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "CreateGroupResponseTypeDef",
     "EmailTypeDef",
     "NameTypeDef",
     "PhoneNumberTypeDef",
-    "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
     "DescribeGroupRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "FilterTypeDef",
-    "GetGroupIdResponseTypeDef",
-    "GetGroupMembershipIdResponseTypeDef",
-    "GetUserIdResponseTypeDef",
-    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    "ListGroupMembershipsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "DescribeGroupResponseTypeDef",
+    "ListGroupMembershipsRequestRequestTypeDef",
     "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
-    "DescribeGroupMembershipResponseTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
     "GroupMembershipExistenceResultTypeDef",
     "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
-    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
+    "CreateGroupMembershipResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "DescribeGroupMembershipResponseTypeDef",
+    "DescribeGroupResponseTypeDef",
+    "GetGroupIdResponseTypeDef",
+    "GetGroupMembershipIdResponseTypeDef",
+    "GetUserIdResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -132,20 +132,22 @@
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-CreateGroupMembershipResponseTypeDef = TypedDict(
-    "CreateGroupMembershipResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -163,23 +165,14 @@
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EmailTypeDef = TypedDict(
     "EmailTypeDef",
     {
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
@@ -205,23 +198,14 @@
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
     total=False,
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGroupMembershipRequestRequestTypeDef = TypedDict(
     "DeleteGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
@@ -270,64 +254,24 @@
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
 
-GetGroupIdResponseTypeDef = TypedDict(
-    "GetGroupIdResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetGroupMembershipIdResponseTypeDef = TypedDict(
-    "GetGroupMembershipIdResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetUserIdResponseTypeDef = TypedDict(
-    "GetUserIdResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "IdentityStoreId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
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
-class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
-    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -344,47 +288,14 @@
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
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
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGroupTypeDef = TypedDict(
     "_RequiredGroupTypeDef",
     {
         "GroupId": str,
         "IdentityStoreId": str,
     },
 )
@@ -435,25 +346,14 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-DescribeGroupMembershipResponseTypeDef = TypedDict(
-    "DescribeGroupMembershipResponseTypeDef",
-    {
-        "IdentityStoreId": str,
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupMembershipIdRequestRequestTypeDef = TypedDict(
     "GetGroupMembershipIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
@@ -495,41 +395,14 @@
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
         "GroupIds": Sequence[str],
     },
 )
 
-_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "IdentityStoreId": str,
-            "MemberId": MemberIdTypeDef,
-        },
-    )
-)
-_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
-    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -546,14 +419,91 @@
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
 
+CreateGroupMembershipResponseTypeDef = TypedDict(
+    "CreateGroupMembershipResponseTypeDef",
+    {
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGroupMembershipResponseTypeDef = TypedDict(
+    "DescribeGroupMembershipResponseTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupIdResponseTypeDef = TypedDict(
+    "GetGroupIdResponseTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupMembershipIdResponseTypeDef = TypedDict(
+    "GetGroupMembershipIdResponseTypeDef",
+    {
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserIdResponseTypeDef = TypedDict(
+    "GetUserIdResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -598,15 +548,15 @@
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "UserId": str,
@@ -635,112 +585,162 @@
 )
 
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+_RequiredListGroupsRequestRequestTypeDef = TypedDict(
+    "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+_OptionalListGroupsRequestRequestTypeDef = TypedDict(
+    "_OptionalListGroupsRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+class ListGroupsRequestRequestTypeDef(
+    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListGroupsRequestRequestTypeDef = TypedDict(
-    "_RequiredListGroupsRequestRequestTypeDef",
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestRequestTypeDef = TypedDict(
-    "_OptionalListGroupsRequestRequestTypeDef",
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 
-class ListGroupsRequestRequestTypeDef(
-    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "IdentityStoreId": str,
+            "MemberId": MemberIdTypeDef,
+        },
+    )
+)
+_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
+    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     {
         "IdentityStoreId": str,
+        "GroupId": str,
     },
 )
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
+    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListUsersRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsersRequestRequestTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsersRequestRequestTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListUsersRequestRequestTypeDef(
-    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -756,37 +756,37 @@
     },
 )
 
 IsMemberInGroupsResponseTypeDef = TypedDict(
     "IsMemberInGroupsResponseTypeDef",
     {
         "Results": List[GroupMembershipExistenceResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsForMemberResponseTypeDef = TypedDict(
     "ListGroupMembershipsForMemberResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore/type_defs.pyi` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_identitystore.type_defs import AddressTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressTypeDef = ...
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -21,55 +21,55 @@
 
 __all__ = (
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
-    "CreateGroupMembershipResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "CreateGroupResponseTypeDef",
     "EmailTypeDef",
     "NameTypeDef",
     "PhoneNumberTypeDef",
-    "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
     "DescribeGroupRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "FilterTypeDef",
-    "GetGroupIdResponseTypeDef",
-    "GetGroupMembershipIdResponseTypeDef",
-    "GetUserIdResponseTypeDef",
-    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    "ListGroupMembershipsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "DescribeGroupResponseTypeDef",
+    "ListGroupMembershipsRequestRequestTypeDef",
     "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
-    "DescribeGroupMembershipResponseTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
     "GroupMembershipExistenceResultTypeDef",
     "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
-    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
+    "CreateGroupMembershipResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "DescribeGroupMembershipResponseTypeDef",
+    "DescribeGroupResponseTypeDef",
+    "GetGroupIdResponseTypeDef",
+    "GetGroupMembershipIdResponseTypeDef",
+    "GetUserIdResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -129,20 +129,22 @@
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-CreateGroupMembershipResponseTypeDef = TypedDict(
-    "CreateGroupMembershipResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -158,23 +160,14 @@
 )
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EmailTypeDef = TypedDict(
     "EmailTypeDef",
     {
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
@@ -200,23 +193,14 @@
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
     total=False,
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGroupMembershipRequestRequestTypeDef = TypedDict(
     "DeleteGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
@@ -265,62 +249,24 @@
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
 
-GetGroupIdResponseTypeDef = TypedDict(
-    "GetGroupIdResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetGroupMembershipIdResponseTypeDef = TypedDict(
-    "GetGroupMembershipIdResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetUserIdResponseTypeDef = TypedDict(
-    "GetUserIdResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "IdentityStoreId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
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
 
-class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
-    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -335,47 +281,14 @@
 
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
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
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGroupTypeDef = TypedDict(
     "_RequiredGroupTypeDef",
     {
         "GroupId": str,
         "IdentityStoreId": str,
     },
 )
@@ -424,25 +337,14 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-DescribeGroupMembershipResponseTypeDef = TypedDict(
-    "DescribeGroupMembershipResponseTypeDef",
-    {
-        "IdentityStoreId": str,
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupMembershipIdRequestRequestTypeDef = TypedDict(
     "GetGroupMembershipIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
@@ -482,39 +384,14 @@
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
         "GroupIds": Sequence[str],
     },
 )
 
-_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "IdentityStoreId": str,
-            "MemberId": MemberIdTypeDef,
-        },
-    )
-)
-_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
-    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -529,14 +406,91 @@
 
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
+CreateGroupMembershipResponseTypeDef = TypedDict(
+    "CreateGroupMembershipResponseTypeDef",
+    {
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGroupMembershipResponseTypeDef = TypedDict(
+    "DescribeGroupMembershipResponseTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupIdResponseTypeDef = TypedDict(
+    "GetGroupIdResponseTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupMembershipIdResponseTypeDef = TypedDict(
+    "GetGroupMembershipIdResponseTypeDef",
+    {
+        "MembershipId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserIdResponseTypeDef = TypedDict(
+    "GetUserIdResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -579,15 +533,15 @@
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "UserId": str,
@@ -614,104 +568,150 @@
     },
     total=False,
 )
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+_RequiredListGroupsRequestRequestTypeDef = TypedDict(
+    "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+_OptionalListGroupsRequestRequestTypeDef = TypedDict(
+    "_OptionalListGroupsRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+class ListGroupsRequestRequestTypeDef(
+    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListGroupsRequestRequestTypeDef = TypedDict(
-    "_RequiredListGroupsRequestRequestTypeDef",
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestRequestTypeDef = TypedDict(
-    "_OptionalListGroupsRequestRequestTypeDef",
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class ListGroupsRequestRequestTypeDef(
-    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "IdentityStoreId": str,
+            "MemberId": MemberIdTypeDef,
+        },
+    )
+)
+_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
+    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     {
         "IdentityStoreId": str,
+        "GroupId": str,
     },
 )
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
+    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
-_RequiredListUsersRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsersRequestRequestTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsersRequestRequestTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListUsersRequestRequestTypeDef(
-    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -727,37 +727,37 @@
     },
 )
 
 IsMemberInGroupsResponseTypeDef = TypedDict(
     "IsMemberInGroupsResponseTypeDef",
     {
         "Results": List[GroupMembershipExistenceResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsForMemberResponseTypeDef = TypedDict(
     "ListGroupMembershipsForMemberResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/PKG-INFO` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-identitystore
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IdentityStore 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IdentityStore 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore identitystore type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore identitystore type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-identitystore"></a>
 
 # types-aiobotocore-identitystore
 
 [![PyPI - types-aiobotocore-identitystore](https://img.shields.io/pypi/v/types-aiobotocore-identitystore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-identitystore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-identitystore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-identitystore?color=blue)](https://pypistats.org/packages/types-aiobotocore-identitystore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-identitystore)](https://pepy.tech/project/types-aiobotocore-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IdentityStore 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [types-aiobotocore-identitystore docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_identitystore/).
 
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
@@ -320,80 +319,80 @@
 )
 
 
 def check_value(value: ListGroupMembershipsForMemberPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_identitystore.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_identitystore.type_defs import (
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    CreateGroupMembershipResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
-    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
     DescribeGroupRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     FilterTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeGroupResponseTypeDef,
+    ListGroupMembershipsRequestRequestTypeDef,
     GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
     GroupMembershipExistenceResultTypeDef,
     GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
+    CreateGroupMembershipResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
+    DescribeGroupResponseTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_value() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-identitystore-2.5.2/types_aiobotocore_identitystore.egg-info/SOURCES.txt` & `types-aiobotocore-identitystore-2.5.2.post1/types_aiobotocore_identitystore.egg-info/SOURCES.txt`

 * *Files identical despite different names*


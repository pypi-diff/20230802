# Comparing `tmp/types-aiobotocore-workdocs-2.5.2.tar.gz` & `tmp/types-aiobotocore-workdocs-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workdocs-2.5.2.tar", last modified: Sat Jul  8 01:44:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-workdocs-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
```

## Comparing `types-aiobotocore-workdocs-2.5.2.tar` & `types-aiobotocore-workdocs-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.507052 types-aiobotocore-workdocs-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-07-08 01:44:28.507052 types-aiobotocore-workdocs-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18520 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:28.507052 types-aiobotocore-workdocs-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.499052 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40882 2023-07-08 01:42:39.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40819 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-08 01:42:39.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-08 01:42:39.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-08 01:42:39.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-08 01:42:39.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50632 2023-07-08 01:42:40.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50541 2023-07-08 01:42:39.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:38.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.507052 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-07-08 01:44:28.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:44:28.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:28.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:28.000000 types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.517426 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40851 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40788 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-08-02 14:51:17.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-08-02 14:51:14.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50590 2023-08-02 14:51:18.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50499 2023-08-02 14:51:17.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workdocs-2.5.2/LICENSE` & `types-aiobotocore-workdocs-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2/PKG-INFO` & `types-aiobotocore-workdocs-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workdocs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore workdocs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore workdocs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-workdocs"></a>
 
 # types-aiobotocore-workdocs
 
 [![PyPI - types-aiobotocore-workdocs](https://img.shields.io/pypi/v/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workdocs?color=blue)](https://pypistats.org/packages/types-aiobotocore-workdocs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkDocs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [types-aiobotocore-workdocs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/).
 
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
@@ -383,137 +382,138 @@
 )
 
 
 def check_value(value: ActivityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_workdocs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
     FolderMetadataTypeDef,
     CreateLabelsRequestRequestTypeDef,
     CreateNotificationSubscriptionRequestRequestTypeDef,
     SubscriptionTypeDef,
     StorageRuleTypeTypeDef,
-    DateRangeTypeTypeDef,
+    TimestampTypeDef,
     DeactivateUserRequestRequestTypeDef,
     DeleteCommentRequestRequestTypeDef,
     DeleteCustomMetadataRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
-    DescribeActivitiesRequestRequestTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCommentsRequestRequestTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
-    InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
+    DateRangeTypeTypeDef,
+    DescribeActivitiesRequestRequestTypeDef,
+    InitiateDocumentVersionUploadRequestRequestTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
-    FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
     UserTypeDef,
+    FiltersTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
-    SearchResourcesRequestRequestTypeDef,
-    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
+    SearchResourcesRequestRequestTypeDef,
+    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     ActivityTypeDef,
     ResponseItemTypeDef,
     CreateCommentResponseTypeDef,
     DescribeCommentsResponseTypeDef,
     DescribeActivitiesResponseTypeDef,
     SearchResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> AbortDocumentVersionUploadRequestRequestTypeDef:
+def get_value() -> AbortDocumentVersionUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-workdocs-2.5.2/README.md` & `types-aiobotocore-workdocs-2.5.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-workdocs"></a>
 
 # types-aiobotocore-workdocs
 
 [![PyPI - types-aiobotocore-workdocs](https://img.shields.io/pypi/v/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workdocs?color=blue)](https://pypistats.org/packages/types-aiobotocore-workdocs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkDocs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [types-aiobotocore-workdocs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/).
 
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
@@ -350,137 +350,138 @@
 )
 
 
 def check_value(value: ActivityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_workdocs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
     FolderMetadataTypeDef,
     CreateLabelsRequestRequestTypeDef,
     CreateNotificationSubscriptionRequestRequestTypeDef,
     SubscriptionTypeDef,
     StorageRuleTypeTypeDef,
-    DateRangeTypeTypeDef,
+    TimestampTypeDef,
     DeactivateUserRequestRequestTypeDef,
     DeleteCommentRequestRequestTypeDef,
     DeleteCustomMetadataRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
-    DescribeActivitiesRequestRequestTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCommentsRequestRequestTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
-    InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
+    DateRangeTypeTypeDef,
+    DescribeActivitiesRequestRequestTypeDef,
+    InitiateDocumentVersionUploadRequestRequestTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
-    FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
     UserTypeDef,
+    FiltersTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
-    SearchResourcesRequestRequestTypeDef,
-    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
+    SearchResourcesRequestRequestTypeDef,
+    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     ActivityTypeDef,
     ResponseItemTypeDef,
     CreateCommentResponseTypeDef,
     DescribeCommentsResponseTypeDef,
     DescribeActivitiesResponseTypeDef,
     SearchResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> AbortDocumentVersionUploadRequestRequestTypeDef:
+def get_value() -> AbortDocumentVersionUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-workdocs-2.5.2/setup.py` & `types-aiobotocore-workdocs-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workdocs",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore workdocs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore workdocs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_workdocs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/"
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/__init__.py` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/__init__.pyi` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/__main__.py` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkDocs 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WorkDocs 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/client.py` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("workdocs") as client:
         client: WorkDocsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BooleanEnumTypeType,
     CommentVisibilityTypeType,
@@ -75,14 +74,15 @@
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     NotificationOptionsTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
     SharePrincipalTypeDef,
     StorageRuleTypeTypeDef,
+    TimestampTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -406,16 +406,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_user)
         """
 
     async def describe_activities(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -665,16 +665,16 @@
 
     async def initiate_document_version_upload(
         self,
         *,
         AuthenticationToken: str = ...,
         Id: str = ...,
         Name: str = ...,
-        ContentCreatedTimestamp: Union[datetime, str] = ...,
-        ContentModifiedTimestamp: Union[datetime, str] = ...,
+        ContentCreatedTimestamp: TimestampTypeDef = ...,
+        ContentModifiedTimestamp: TimestampTypeDef = ...,
         ContentType: str = ...,
         DocumentSizeInBytes: int = ...,
         ParentFolderId: str = ...
     ) -> InitiateDocumentVersionUploadResponseTypeDef:
         """
         Creates a new document object and version object.
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/client.pyi` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("workdocs") as client:
         client: WorkDocsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BooleanEnumTypeType,
     CommentVisibilityTypeType,
@@ -75,14 +74,15 @@
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     NotificationOptionsTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
     SharePrincipalTypeDef,
     StorageRuleTypeTypeDef,
+    TimestampTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -380,16 +380,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/client/#delete_user)
         """
     async def describe_activities(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -622,16 +622,16 @@
         """
     async def initiate_document_version_upload(
         self,
         *,
         AuthenticationToken: str = ...,
         Id: str = ...,
         Name: str = ...,
-        ContentCreatedTimestamp: Union[datetime, str] = ...,
-        ContentModifiedTimestamp: Union[datetime, str] = ...,
+        ContentCreatedTimestamp: TimestampTypeDef = ...,
+        ContentModifiedTimestamp: TimestampTypeDef = ...,
         ContentType: str = ...,
         DocumentSizeInBytes: int = ...,
         ParentFolderId: str = ...
     ) -> InitiateDocumentVersionUploadResponseTypeDef:
         """
         Creates a new document object and version object.
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/literals.py` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/literals.pyi` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/paginator.py` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         describe_resource_permissions_paginator: DescribeResourcePermissionsPaginator = client.get_paginator("describe_resource_permissions")
         describe_root_folders_paginator: DescribeRootFoldersPaginator = client.get_paginator("describe_root_folders")
         describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
         search_resources_paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     FolderContentTypeType,
     OrderTypeType,
@@ -63,14 +62,15 @@
     DescribeResourcePermissionsResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FiltersTypeDef,
     PaginatorConfigTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -105,22 +105,22 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeactivitiespaginator)
         """
 
 
@@ -132,15 +132,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describecommentspaginator)
         """
 
 
@@ -153,15 +153,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 
@@ -176,15 +176,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 
@@ -196,30 +196,30 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describegroupspaginator)
         """
 
 
 class DescribeNotificationSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describenotificationsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeNotificationSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describenotificationsubscriptionspaginator)
         """
 
 
@@ -231,30 +231,30 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 
 class DescribeRootFoldersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describerootfolderspaginator)
     """
 
     def paginate(
-        self, *, AuthenticationToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AuthenticationToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRootFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describerootfolderspaginator)
         """
 
 
@@ -271,15 +271,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeuserspaginator)
         """
 
 
@@ -295,13 +295,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/paginator.pyi` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         describe_resource_permissions_paginator: DescribeResourcePermissionsPaginator = client.get_paginator("describe_resource_permissions")
         describe_root_folders_paginator: DescribeRootFoldersPaginator = client.get_paginator("describe_root_folders")
         describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
         search_resources_paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     FolderContentTypeType,
     OrderTypeType,
@@ -63,14 +62,15 @@
     DescribeResourcePermissionsResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FiltersTypeDef,
     PaginatorConfigTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -101,22 +101,22 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeactivitiespaginator)
         """
 
 class DescribeCommentsPaginator(AioPaginator):
@@ -127,15 +127,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describecommentspaginator)
         """
 
 class DescribeDocumentVersionsPaginator(AioPaginator):
@@ -147,15 +147,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 class DescribeFolderContentsPaginator(AioPaginator):
@@ -169,15 +169,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 class DescribeGroupsPaginator(AioPaginator):
@@ -188,29 +188,29 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describegroupspaginator)
         """
 
 class DescribeNotificationSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describenotificationsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeNotificationSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describenotificationsubscriptionspaginator)
         """
 
 class DescribeResourcePermissionsPaginator(AioPaginator):
@@ -221,29 +221,29 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 class DescribeRootFoldersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describerootfolderspaginator)
     """
 
     def paginate(
-        self, *, AuthenticationToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AuthenticationToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRootFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describerootfolderspaginator)
         """
 
 class DescribeUsersPaginator(AioPaginator):
@@ -259,15 +259,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#describeuserspaginator)
         """
 
 class SearchResourcesPaginator(AioPaginator):
@@ -282,13 +282,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/type_defs.py` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_workdocs.type_defs import AbortDocumentVersionUploadRequestRequestTypeDef
 
-    data: AbortDocumentVersionUploadRequestRequestTypeDef = {...}
+    data: AbortDocumentVersionUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -55,120 +55,120 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
     "ShareResultTypeDef",
     "CreateCommentRequestRequestTypeDef",
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "FolderMetadataTypeDef",
     "CreateLabelsRequestRequestTypeDef",
     "CreateNotificationSubscriptionRequestRequestTypeDef",
     "SubscriptionTypeDef",
     "StorageRuleTypeTypeDef",
-    "DateRangeTypeTypeDef",
+    "TimestampTypeDef",
     "DeactivateUserRequestRequestTypeDef",
     "DeleteCommentRequestRequestTypeDef",
     "DeleteCustomMetadataRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    "DescribeActivitiesRequestRequestTypeDef",
-    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
-    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
-    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
-    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
-    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
-    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestRequestTypeDef",
-    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeRootFoldersRequestRequestTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "LongRangeTypeTypeDef",
     "SearchPrincipalTypeTypeDef",
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserStorageMetadataTypeDef",
+    "DateRangeTypeTypeDef",
+    "DescribeActivitiesRequestRequestTypeDef",
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
-    "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
     "UserTypeDef",
+    "FiltersTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
-    "SearchResourcesRequestRequestTypeDef",
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
+    "SearchResourcesRequestRequestTypeDef",
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "ActivityTypeDef",
     "ResponseItemTypeDef",
     "CreateCommentResponseTypeDef",
     "DescribeCommentsResponseTypeDef",
     "DescribeActivitiesResponseTypeDef",
     "SearchResourcesResponseTypeDef",
 )
@@ -184,42 +184,49 @@
     "_OptionalAbortDocumentVersionUploadRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class AbortDocumentVersionUploadRequestRequestTypeDef(
     _RequiredAbortDocumentVersionUploadRequestRequestTypeDef,
     _OptionalAbortDocumentVersionUploadRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredActivateUserRequestRequestTypeDef = TypedDict(
     "_RequiredActivateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalActivateUserRequestRequestTypeDef = TypedDict(
     "_OptionalActivateUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class ActivateUserRequestRequestTypeDef(
     _RequiredActivateUserRequestRequestTypeDef, _OptionalActivateUserRequestRequestTypeDef
 ):
     pass
 
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
 
 UserMetadataTypeDef = TypedDict(
     "UserMetadataTypeDef",
     {
         "Id": str,
         "Username": str,
         "GivenName": str,
@@ -276,21 +283,19 @@
         "ThreadId": str,
         "Visibility": CommentVisibilityTypeType,
         "NotifyCollaborators": bool,
     },
     total=False,
 )
 
-
 class CreateCommentRequestRequestTypeDef(
     _RequiredCreateCommentRequestRequestTypeDef, _OptionalCreateCommentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCustomMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
         "CustomMetadata": Mapping[str, str],
     },
 )
@@ -299,22 +304,20 @@
     {
         "AuthenticationToken": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class CreateCustomMetadataRequestRequestTypeDef(
     _RequiredCreateCustomMetadataRequestRequestTypeDef,
     _OptionalCreateCustomMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFolderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFolderRequestRequestTypeDef",
     {
         "ParentFolderId": str,
     },
 )
 _OptionalCreateFolderRequestRequestTypeDef = TypedDict(
@@ -322,21 +325,19 @@
     {
         "AuthenticationToken": str,
         "Name": str,
     },
     total=False,
 )
 
-
 class CreateFolderRequestRequestTypeDef(
     _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
 ):
     pass
 
-
 FolderMetadataTypeDef = TypedDict(
     "FolderMetadataTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatorId": str,
         "ParentFolderId": str,
@@ -362,21 +363,19 @@
     "_OptionalCreateLabelsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class CreateLabelsRequestRequestTypeDef(
     _RequiredCreateLabelsRequestRequestTypeDef, _OptionalCreateLabelsRequestRequestTypeDef
 ):
     pass
 
-
 CreateNotificationSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateNotificationSubscriptionRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Endpoint": str,
         "Protocol": SubscriptionProtocolTypeType,
         "SubscriptionType": Literal["ALL"],
@@ -398,44 +397,34 @@
     {
         "StorageAllocatedInBytes": int,
         "StorageType": StorageTypeType,
     },
     total=False,
 )
 
-DateRangeTypeTypeDef = TypedDict(
-    "DateRangeTypeTypeDef",
-    {
-        "StartValue": Union[datetime, str],
-        "EndValue": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeactivateUserRequestRequestTypeDef = TypedDict(
     "_RequiredDeactivateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalDeactivateUserRequestRequestTypeDef = TypedDict(
     "_OptionalDeactivateUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeactivateUserRequestRequestTypeDef(
     _RequiredDeactivateUserRequestRequestTypeDef, _OptionalDeactivateUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteCommentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCommentRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
         "CommentId": str,
     },
@@ -444,21 +433,19 @@
     "_OptionalDeleteCommentRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeleteCommentRequestRequestTypeDef(
     _RequiredDeleteCommentRequestRequestTypeDef, _OptionalDeleteCommentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteCustomMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDeleteCustomMetadataRequestRequestTypeDef = TypedDict(
@@ -468,43 +455,39 @@
         "VersionId": str,
         "Keys": Sequence[str],
         "DeleteAll": bool,
     },
     total=False,
 )
 
-
 class DeleteCustomMetadataRequestRequestTypeDef(
     _RequiredDeleteCustomMetadataRequestRequestTypeDef,
     _OptionalDeleteCustomMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDeleteDocumentRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDocumentRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteDocumentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDocumentVersionRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
         "DeletePriorVersions": bool,
     },
@@ -513,65 +496,59 @@
     "_OptionalDeleteDocumentVersionRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeleteDocumentVersionRequestRequestTypeDef(
     _RequiredDeleteDocumentVersionRequestRequestTypeDef,
     _OptionalDeleteDocumentVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDeleteFolderContentsRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFolderContentsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeleteFolderContentsRequestRequestTypeDef(
     _RequiredDeleteFolderContentsRequestRequestTypeDef,
     _OptionalDeleteFolderContentsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFolderRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFolderRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDeleteFolderRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFolderRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeleteFolderRequestRequestTypeDef(
     _RequiredDeleteFolderRequestRequestTypeDef, _OptionalDeleteFolderRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLabelsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDeleteLabelsRequestRequestTypeDef = TypedDict(
@@ -580,21 +557,19 @@
         "AuthenticationToken": str,
         "Labels": Sequence[str],
         "DeleteAll": bool,
     },
     total=False,
 )
 
-
 class DeleteLabelsRequestRequestTypeDef(
     _RequiredDeleteLabelsRequestRequestTypeDef, _OptionalDeleteLabelsRequestRequestTypeDef
 ):
     pass
 
-
 DeleteNotificationSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     {
         "SubscriptionId": str,
         "OrganizationId": str,
     },
 )
@@ -609,78 +584,29 @@
     "_OptionalDeleteUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
-
-DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeActivitiesRequestRequestTypeDef = TypedDict(
-    "DescribeActivitiesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "DocumentId": str,
-        "VersionId": str,
-    },
-)
-_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AuthenticationToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
-    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -690,46 +616,19 @@
         "AuthenticationToken": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeCommentsRequestRequestTypeDef(
     _RequiredDescribeCommentsRequestRequestTypeDef, _OptionalDescribeCommentsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Include": str,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
-    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -740,22 +639,20 @@
         "Limit": int,
         "Include": str,
         "Fields": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentVersionsRequestRequestTypeDef(
     _RequiredDescribeDocumentVersionsRequestRequestTypeDef,
     _OptionalDescribeDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 DocumentVersionMetadataTypeDef = TypedDict(
     "DocumentVersionMetadataTypeDef",
     {
         "Id": str,
         "Name": str,
         "ContentType": str,
         "Size": int,
@@ -768,41 +665,14 @@
         "CreatorId": str,
         "Thumbnail": Dict[DocumentThumbnailTypeType, str],
         "Source": Dict[DocumentSourceTypeType, str],
     },
     total=False,
 )
 
-_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "FolderId": str,
-    },
-)
-_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Sort": ResourceSortTypeType,
-        "Order": OrderTypeType,
-        "Type": FolderContentTypeType,
-        "Include": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
-    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDescribeFolderContentsRequestRequestTypeDef = TypedDict(
@@ -815,46 +685,20 @@
         "Marker": str,
         "Type": FolderContentTypeType,
         "Include": str,
     },
     total=False,
 )
 
-
 class DescribeFolderContentsRequestRequestTypeDef(
     _RequiredDescribeFolderContentsRequestRequestTypeDef,
     _OptionalDescribeFolderContentsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "SearchQuery": str,
-    },
-)
-_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
-    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeGroupsRequestRequestTypeDef",
     {
         "SearchQuery": str,
     },
 )
 _OptionalDescribeGroupsRequestRequestTypeDef = TypedDict(
@@ -864,52 +708,28 @@
         "OrganizationId": str,
         "Marker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeGroupsRequestRequestTypeDef(
     _RequiredDescribeGroupsRequestRequestTypeDef, _OptionalDescribeGroupsRequestRequestTypeDef
 ):
     pass
 
-
 GroupMetadataTypeDef = TypedDict(
     "GroupMetadataTypeDef",
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
-_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
-    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -917,46 +737,20 @@
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeNotificationSubscriptionsRequestRequestTypeDef(
     _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef,
     _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PrincipalId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
-    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourcePermissionsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
@@ -966,44 +760,20 @@
         "PrincipalId": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeResourcePermissionsRequestRequestTypeDef(
     _RequiredDescribeResourcePermissionsRequestRequestTypeDef,
     _OptionalDescribeResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-    },
-)
-_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
-    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeRootFoldersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRootFoldersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 _OptionalDescribeRootFoldersRequestRequestTypeDef = TypedDict(
@@ -1011,38 +781,20 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeRootFoldersRequestRequestTypeDef(
     _RequiredDescribeRootFoldersRequestRequestTypeDef,
     _OptionalDescribeRootFoldersRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "UserIds": str,
-        "Query": str,
-        "Include": UserFilterTypeType,
-        "Order": OrderTypeType,
-        "Sort": UserSortTypeType,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "OrganizationId": str,
         "UserIds": str,
         "Query": str,
@@ -1052,21 +804,14 @@
         "Marker": str,
         "Limit": int,
         "Fields": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LongRangeTypeTypeDef = TypedDict(
     "LongRangeTypeTypeDef",
     {
         "StartValue": int,
         "EndValue": int,
     },
     total=False,
@@ -1082,21 +827,19 @@
     "_OptionalSearchPrincipalTypeTypeDef",
     {
         "Roles": Sequence[PrincipalRoleTypeType],
     },
     total=False,
 )
 
-
 class SearchPrincipalTypeTypeDef(
     _RequiredSearchPrincipalTypeTypeDef, _OptionalSearchPrincipalTypeTypeDef
 ):
     pass
 
-
 GetCurrentUserRequestRequestTypeDef = TypedDict(
     "GetCurrentUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 
@@ -1113,21 +856,19 @@
         "Limit": int,
         "Fields": str,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetDocumentPathRequestRequestTypeDef(
     _RequiredGetDocumentPathRequestRequestTypeDef, _OptionalGetDocumentPathRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -1135,21 +876,19 @@
     {
         "AuthenticationToken": str,
         "IncludeCustomMetadata": bool,
     },
     total=False,
 )
 
-
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetDocumentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentVersionRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -1159,22 +898,20 @@
         "AuthenticationToken": str,
         "Fields": str,
         "IncludeCustomMetadata": bool,
     },
     total=False,
 )
 
-
 class GetDocumentVersionRequestRequestTypeDef(
     _RequiredGetDocumentVersionRequestRequestTypeDef,
     _OptionalGetDocumentVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetFolderPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetFolderPathRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalGetFolderPathRequestRequestTypeDef = TypedDict(
@@ -1184,21 +921,19 @@
         "Limit": int,
         "Fields": str,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetFolderPathRequestRequestTypeDef(
     _RequiredGetFolderPathRequestRequestTypeDef, _OptionalGetFolderPathRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetFolderRequestRequestTypeDef = TypedDict(
     "_RequiredGetFolderRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalGetFolderRequestRequestTypeDef = TypedDict(
@@ -1206,67 +941,40 @@
     {
         "AuthenticationToken": str,
         "IncludeCustomMetadata": bool,
     },
     total=False,
 )
 
-
 class GetFolderRequestRequestTypeDef(
     _RequiredGetFolderRequestRequestTypeDef, _OptionalGetFolderRequestRequestTypeDef
 ):
     pass
 
-
 GetResourcesRequestRequestTypeDef = TypedDict(
     "GetResourcesRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "UserId": str,
         "CollectionType": Literal["SHARED_WITH_ME"],
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Id": str,
-        "Name": str,
-        "ContentCreatedTimestamp": Union[datetime, str],
-        "ContentModifiedTimestamp": Union[datetime, str],
-        "ContentType": str,
-        "DocumentSizeInBytes": int,
-        "ParentFolderId": str,
-    },
-    total=False,
-)
-
 UploadMetadataTypeDef = TypedDict(
     "UploadMetadataTypeDef",
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
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
 PermissionInfoTypeDef = TypedDict(
     "PermissionInfoTypeDef",
     {
         "Role": RoleTypeType,
         "Type": RolePermissionTypeType,
     },
     total=False,
@@ -1282,22 +990,20 @@
     "_OptionalRemoveAllResourcePermissionsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class RemoveAllResourcePermissionsRequestRequestTypeDef(
     _RequiredRemoveAllResourcePermissionsRequestRequestTypeDef,
     _OptionalRemoveAllResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRemoveResourcePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveResourcePermissionRequestRequestTypeDef",
     {
         "ResourceId": str,
         "PrincipalId": str,
     },
 )
@@ -1306,64 +1012,49 @@
     {
         "AuthenticationToken": str,
         "PrincipalType": PrincipalTypeType,
     },
     total=False,
 )
 
-
 class RemoveResourcePermissionRequestRequestTypeDef(
     _RequiredRemoveResourcePermissionRequestRequestTypeDef,
     _OptionalRemoveResourcePermissionRequestRequestTypeDef,
 ):
     pass
 
-
 ResourcePathComponentTypeDef = TypedDict(
     "ResourcePathComponentTypeDef",
     {
         "Id": str,
         "Name": str,
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
 _RequiredRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_OptionalRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class RestoreDocumentVersionsRequestRequestTypeDef(
     _RequiredRestoreDocumentVersionsRequestRequestTypeDef,
     _OptionalRestoreDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 SearchSortResultTypeDef = TypedDict(
     "SearchSortResultTypeDef",
     {
         "Field": OrderByFieldTypeType,
         "Order": SortOrderType,
     },
     total=False,
@@ -1382,21 +1073,19 @@
         "Name": str,
         "ParentFolderId": str,
         "ResourceState": ResourceStateTypeType,
     },
     total=False,
 )
 
-
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDocumentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentVersionRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -1405,22 +1094,20 @@
     {
         "AuthenticationToken": str,
         "VersionStatus": Literal["ACTIVE"],
     },
     total=False,
 )
 
-
 class UpdateDocumentVersionRequestRequestTypeDef(
     _RequiredUpdateDocumentVersionRequestRequestTypeDef,
     _OptionalUpdateDocumentVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFolderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFolderRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalUpdateFolderRequestRequestTypeDef = TypedDict(
@@ -1430,20 +1117,25 @@
         "Name": str,
         "ParentFolderId": str,
         "ResourceState": ResourceStateTypeType,
     },
     total=False,
 )
 
-
 class UpdateFolderRequestRequestTypeDef(
     _RequiredUpdateFolderRequestRequestTypeDef, _OptionalUpdateFolderRequestRequestTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ResourceMetadataTypeDef = TypedDict(
     "ResourceMetadataTypeDef",
     {
         "Type": ResourceTypeType,
         "Name": str,
         "OriginalName": str,
@@ -1467,70 +1159,68 @@
     {
         "AuthenticationToken": str,
         "NotificationOptions": NotificationOptionsTypeDef,
     },
     total=False,
 )
 
-
 class AddResourcePermissionsRequestRequestTypeDef(
     _RequiredAddResourcePermissionsRequestRequestTypeDef,
     _OptionalAddResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 AddResourcePermissionsResponseTypeDef = TypedDict(
     "AddResourcePermissionsResponseTypeDef",
     {
         "ShareResults": List[ShareResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFolderResponseTypeDef = TypedDict(
     "CreateFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRootFoldersResponseTypeDef = TypedDict(
     "DescribeRootFoldersResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderResponseTypeDef = TypedDict(
     "GetFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNotificationSubscriptionResponseTypeDef = TypedDict(
     "CreateNotificationSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationSubscriptionsResponseTypeDef = TypedDict(
     "DescribeNotificationSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "Username": str,
@@ -1547,21 +1237,19 @@
         "TimeZoneId": str,
         "StorageRule": StorageRuleTypeTypeDef,
         "AuthenticationToken": str,
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
@@ -1575,36 +1263,261 @@
         "TimeZoneId": str,
         "Locale": LocaleTypeType,
         "GrantPoweruserPrivileges": BooleanEnumTypeType,
     },
     total=False,
 )
 
-
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
-
 UserStorageMetadataTypeDef = TypedDict(
     "UserStorageMetadataTypeDef",
     {
         "StorageUtilizedInBytes": int,
         "StorageRule": StorageRuleTypeTypeDef,
     },
     total=False,
 )
 
+DateRangeTypeTypeDef = TypedDict(
+    "DateRangeTypeTypeDef",
+    {
+        "StartValue": TimestampTypeDef,
+        "EndValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DescribeActivitiesRequestRequestTypeDef = TypedDict(
+    "DescribeActivitiesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "Limit": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Id": str,
+        "Name": str,
+        "ContentCreatedTimestamp": TimestampTypeDef,
+        "ContentModifiedTimestamp": TimestampTypeDef,
+        "ContentType": str,
+        "DocumentSizeInBytes": int,
+        "ParentFolderId": str,
+    },
+    total=False,
+)
+
+DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "DocumentId": str,
+        "VersionId": str,
+    },
+)
+_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
+    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Include": str,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
+    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "FolderId": str,
+    },
+)
+_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Sort": ResourceSortTypeType,
+        "Order": OrderTypeType,
+        "Type": FolderContentTypeType,
+        "Include": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
+    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "SearchQuery": str,
+    },
+)
+_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
+    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
+    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PrincipalId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
+    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+    },
+)
+_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
+    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+):
+    pass
+
+DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "UserIds": str,
+        "Query": str,
+        "Include": UserFilterTypeType,
+        "Order": OrderTypeType,
+        "Sort": UserSortTypeType,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeDocumentVersionsResponseTypeDef = TypedDict(
     "DescribeDocumentVersionsResponseTypeDef",
     {
         "DocumentVersions": List[DocumentVersionMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Id": str,
@@ -1620,53 +1533,36 @@
 )
 
 GetDocumentVersionResponseTypeDef = TypedDict(
     "GetDocumentVersionResponseTypeDef",
     {
         "Metadata": DocumentVersionMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGroupsResponseTypeDef = TypedDict(
     "DescribeGroupsResponseTypeDef",
     {
         "Groups": List[GroupMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParticipantsTypeDef = TypedDict(
     "ParticipantsTypeDef",
     {
         "Users": List[UserMetadataTypeDef],
         "Groups": List[GroupMetadataTypeDef],
     },
     total=False,
 )
 
-FiltersTypeDef = TypedDict(
-    "FiltersTypeDef",
-    {
-        "TextLocales": Sequence[LanguageCodeTypeType],
-        "ContentCategories": Sequence[ContentCategoryTypeType],
-        "ResourceTypes": Sequence[SearchResourceTypeType],
-        "Labels": Sequence[str],
-        "Principals": Sequence[SearchPrincipalTypeTypeDef],
-        "AncestorIds": Sequence[str],
-        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
-        "SizeRange": LongRangeTypeTypeDef,
-        "CreatedRange": DateRangeTypeTypeDef,
-        "ModifiedRange": DateRangeTypeTypeDef,
-    },
-    total=False,
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "Id": str,
         "Type": PrincipalTypeType,
         "Roles": List[PermissionInfoTypeDef],
     },
@@ -1699,113 +1595,99 @@
         "TimeZoneId": str,
         "Locale": LocaleTypeType,
         "Storage": UserStorageMetadataTypeDef,
     },
     total=False,
 )
 
+FiltersTypeDef = TypedDict(
+    "FiltersTypeDef",
+    {
+        "TextLocales": Sequence[LanguageCodeTypeType],
+        "ContentCategories": Sequence[ContentCategoryTypeType],
+        "ResourceTypes": Sequence[SearchResourceTypeType],
+        "Labels": Sequence[str],
+        "Principals": Sequence[SearchPrincipalTypeTypeDef],
+        "AncestorIds": Sequence[str],
+        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
+        "SizeRange": LongRangeTypeTypeDef,
+        "CreatedRange": DateRangeTypeTypeDef,
+        "ModifiedRange": DateRangeTypeTypeDef,
+    },
+    total=False,
+)
+
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentResponseTypeDef = TypedDict(
     "GetDocumentResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesResponseTypeDef = TypedDict(
     "GetResourcesResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateDocumentVersionUploadResponseTypeDef = TypedDict(
     "InitiateDocumentVersionUploadResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchResourcesRequestRequestTypeDef = TypedDict(
-    "SearchResourcesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentPathResponseTypeDef = TypedDict(
     "GetDocumentPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderPathResponseTypeDef = TypedDict(
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentMetadataTypeDef = TypedDict(
     "CommentMetadataTypeDef",
     {
         "CommentId": str,
@@ -1835,51 +1717,80 @@
         "Status": CommentStatusTypeType,
         "Visibility": CommentVisibilityTypeType,
         "RecipientId": str,
     },
     total=False,
 )
 
-
 class CommentTypeDef(_RequiredCommentTypeDef, _OptionalCommentTypeDef):
     pass
 
-
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "TotalNumberOfUsers": int,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCurrentUserResponseTypeDef = TypedDict(
     "GetCurrentUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchResourcesRequestRequestTypeDef = TypedDict(
+    "SearchResourcesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "Limit": int,
+        "Marker": str,
     },
+    total=False,
+)
+
+SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
         "TimeStamp": datetime,
@@ -1907,37 +1818,37 @@
     total=False,
 )
 
 CreateCommentResponseTypeDef = TypedDict(
     "CreateCommentResponseTypeDef",
     {
         "Comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCommentsResponseTypeDef = TypedDict(
     "DescribeCommentsResponseTypeDef",
     {
         "Comments": List[CommentTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeActivitiesResponseTypeDef = TypedDict(
     "DescribeActivitiesResponseTypeDef",
     {
         "UserActivities": List[ActivityTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "Items": List[ResponseItemTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs/type_defs.pyi` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_workdocs.type_defs import AbortDocumentVersionUploadRequestRequestTypeDef
 
-    data: AbortDocumentVersionUploadRequestRequestTypeDef = {...}
+    data: AbortDocumentVersionUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -55,119 +55,121 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
     "ShareResultTypeDef",
     "CreateCommentRequestRequestTypeDef",
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "FolderMetadataTypeDef",
     "CreateLabelsRequestRequestTypeDef",
     "CreateNotificationSubscriptionRequestRequestTypeDef",
     "SubscriptionTypeDef",
     "StorageRuleTypeTypeDef",
-    "DateRangeTypeTypeDef",
+    "TimestampTypeDef",
     "DeactivateUserRequestRequestTypeDef",
     "DeleteCommentRequestRequestTypeDef",
     "DeleteCustomMetadataRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    "DescribeActivitiesRequestRequestTypeDef",
-    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
-    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
-    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
-    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
-    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
-    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestRequestTypeDef",
-    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeRootFoldersRequestRequestTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "LongRangeTypeTypeDef",
     "SearchPrincipalTypeTypeDef",
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserStorageMetadataTypeDef",
+    "DateRangeTypeTypeDef",
+    "DescribeActivitiesRequestRequestTypeDef",
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
-    "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
     "UserTypeDef",
+    "FiltersTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
-    "SearchResourcesRequestRequestTypeDef",
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
+    "SearchResourcesRequestRequestTypeDef",
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "ActivityTypeDef",
     "ResponseItemTypeDef",
     "CreateCommentResponseTypeDef",
     "DescribeCommentsResponseTypeDef",
     "DescribeActivitiesResponseTypeDef",
     "SearchResourcesResponseTypeDef",
 )
@@ -183,39 +185,54 @@
     "_OptionalAbortDocumentVersionUploadRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class AbortDocumentVersionUploadRequestRequestTypeDef(
     _RequiredAbortDocumentVersionUploadRequestRequestTypeDef,
     _OptionalAbortDocumentVersionUploadRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredActivateUserRequestRequestTypeDef = TypedDict(
     "_RequiredActivateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalActivateUserRequestRequestTypeDef = TypedDict(
     "_OptionalActivateUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class ActivateUserRequestRequestTypeDef(
     _RequiredActivateUserRequestRequestTypeDef, _OptionalActivateUserRequestRequestTypeDef
 ):
     pass
 
+
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
 UserMetadataTypeDef = TypedDict(
     "UserMetadataTypeDef",
     {
         "Id": str,
         "Username": str,
         "GivenName": str,
         "Surname": str,
@@ -271,19 +288,21 @@
         "ThreadId": str,
         "Visibility": CommentVisibilityTypeType,
         "NotifyCollaborators": bool,
     },
     total=False,
 )
 
+
 class CreateCommentRequestRequestTypeDef(
     _RequiredCreateCommentRequestRequestTypeDef, _OptionalCreateCommentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCustomMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
         "CustomMetadata": Mapping[str, str],
     },
 )
@@ -292,20 +311,22 @@
     {
         "AuthenticationToken": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class CreateCustomMetadataRequestRequestTypeDef(
     _RequiredCreateCustomMetadataRequestRequestTypeDef,
     _OptionalCreateCustomMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFolderRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFolderRequestRequestTypeDef",
     {
         "ParentFolderId": str,
     },
 )
 _OptionalCreateFolderRequestRequestTypeDef = TypedDict(
@@ -313,19 +334,21 @@
     {
         "AuthenticationToken": str,
         "Name": str,
     },
     total=False,
 )
 
+
 class CreateFolderRequestRequestTypeDef(
     _RequiredCreateFolderRequestRequestTypeDef, _OptionalCreateFolderRequestRequestTypeDef
 ):
     pass
 
+
 FolderMetadataTypeDef = TypedDict(
     "FolderMetadataTypeDef",
     {
         "Id": str,
         "Name": str,
         "CreatorId": str,
         "ParentFolderId": str,
@@ -351,19 +374,21 @@
     "_OptionalCreateLabelsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class CreateLabelsRequestRequestTypeDef(
     _RequiredCreateLabelsRequestRequestTypeDef, _OptionalCreateLabelsRequestRequestTypeDef
 ):
     pass
 
+
 CreateNotificationSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateNotificationSubscriptionRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Endpoint": str,
         "Protocol": SubscriptionProtocolTypeType,
         "SubscriptionType": Literal["ALL"],
@@ -385,42 +410,36 @@
     {
         "StorageAllocatedInBytes": int,
         "StorageType": StorageTypeType,
     },
     total=False,
 )
 
-DateRangeTypeTypeDef = TypedDict(
-    "DateRangeTypeTypeDef",
-    {
-        "StartValue": Union[datetime, str],
-        "EndValue": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeactivateUserRequestRequestTypeDef = TypedDict(
     "_RequiredDeactivateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalDeactivateUserRequestRequestTypeDef = TypedDict(
     "_OptionalDeactivateUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeactivateUserRequestRequestTypeDef(
     _RequiredDeactivateUserRequestRequestTypeDef, _OptionalDeactivateUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteCommentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCommentRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
         "CommentId": str,
     },
@@ -429,19 +448,21 @@
     "_OptionalDeleteCommentRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeleteCommentRequestRequestTypeDef(
     _RequiredDeleteCommentRequestRequestTypeDef, _OptionalDeleteCommentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteCustomMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDeleteCustomMetadataRequestRequestTypeDef = TypedDict(
@@ -451,39 +472,43 @@
         "VersionId": str,
         "Keys": Sequence[str],
         "DeleteAll": bool,
     },
     total=False,
 )
 
+
 class DeleteCustomMetadataRequestRequestTypeDef(
     _RequiredDeleteCustomMetadataRequestRequestTypeDef,
     _OptionalDeleteCustomMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDeleteDocumentRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDocumentRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteDocumentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDocumentVersionRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
         "DeletePriorVersions": bool,
     },
@@ -492,59 +517,65 @@
     "_OptionalDeleteDocumentVersionRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeleteDocumentVersionRequestRequestTypeDef(
     _RequiredDeleteDocumentVersionRequestRequestTypeDef,
     _OptionalDeleteDocumentVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDeleteFolderContentsRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFolderContentsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeleteFolderContentsRequestRequestTypeDef(
     _RequiredDeleteFolderContentsRequestRequestTypeDef,
     _OptionalDeleteFolderContentsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFolderRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFolderRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDeleteFolderRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFolderRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeleteFolderRequestRequestTypeDef(
     _RequiredDeleteFolderRequestRequestTypeDef, _OptionalDeleteFolderRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLabelsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDeleteLabelsRequestRequestTypeDef = TypedDict(
@@ -553,19 +584,21 @@
         "AuthenticationToken": str,
         "Labels": Sequence[str],
         "DeleteAll": bool,
     },
     total=False,
 )
 
+
 class DeleteLabelsRequestRequestTypeDef(
     _RequiredDeleteLabelsRequestRequestTypeDef, _OptionalDeleteLabelsRequestRequestTypeDef
 ):
     pass
 
+
 DeleteNotificationSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     {
         "SubscriptionId": str,
         "OrganizationId": str,
     },
 )
@@ -580,74 +613,31 @@
     "_OptionalDeleteUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
-DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeActivitiesRequestRequestTypeDef = TypedDict(
-    "DescribeActivitiesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
 
-_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "DocumentId": str,
-        "VersionId": str,
-    },
-)
-_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AuthenticationToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
-    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -657,41 +647,20 @@
         "AuthenticationToken": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeCommentsRequestRequestTypeDef(
     _RequiredDescribeCommentsRequestRequestTypeDef, _OptionalDescribeCommentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Include": str,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
-    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
@@ -703,20 +672,22 @@
         "Limit": int,
         "Include": str,
         "Fields": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentVersionsRequestRequestTypeDef(
     _RequiredDescribeDocumentVersionsRequestRequestTypeDef,
     _OptionalDescribeDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 DocumentVersionMetadataTypeDef = TypedDict(
     "DocumentVersionMetadataTypeDef",
     {
         "Id": str,
         "Name": str,
         "ContentType": str,
         "Size": int,
@@ -729,39 +700,14 @@
         "CreatorId": str,
         "Thumbnail": Dict[DocumentThumbnailTypeType, str],
         "Source": Dict[DocumentSourceTypeType, str],
     },
     total=False,
 )
 
-_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "FolderId": str,
-    },
-)
-_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Sort": ResourceSortTypeType,
-        "Order": OrderTypeType,
-        "Type": FolderContentTypeType,
-        "Include": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
-    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDescribeFolderContentsRequestRequestTypeDef = TypedDict(
@@ -774,41 +720,21 @@
         "Marker": str,
         "Type": FolderContentTypeType,
         "Include": str,
     },
     total=False,
 )
 
+
 class DescribeFolderContentsRequestRequestTypeDef(
     _RequiredDescribeFolderContentsRequestRequestTypeDef,
     _OptionalDescribeFolderContentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "SearchQuery": str,
-    },
-)
-_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
-    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeGroupsRequestRequestTypeDef",
     {
         "SearchQuery": str,
     },
 )
@@ -819,48 +745,30 @@
         "OrganizationId": str,
         "Marker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeGroupsRequestRequestTypeDef(
     _RequiredDescribeGroupsRequestRequestTypeDef, _OptionalDescribeGroupsRequestRequestTypeDef
 ):
     pass
 
+
 GroupMetadataTypeDef = TypedDict(
     "GroupMetadataTypeDef",
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
-_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
-    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -868,41 +776,21 @@
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeNotificationSubscriptionsRequestRequestTypeDef(
     _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef,
     _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PrincipalId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
-    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourcePermissionsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
@@ -913,39 +801,21 @@
         "PrincipalId": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeResourcePermissionsRequestRequestTypeDef(
     _RequiredDescribeResourcePermissionsRequestRequestTypeDef,
     _OptionalDescribeResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-    },
-)
-_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
-    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeRootFoldersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRootFoldersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
@@ -954,35 +824,21 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeRootFoldersRequestRequestTypeDef(
     _RequiredDescribeRootFoldersRequestRequestTypeDef,
     _OptionalDescribeRootFoldersRequestRequestTypeDef,
 ):
     pass
 
-DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "UserIds": str,
-        "Query": str,
-        "Include": UserFilterTypeType,
-        "Order": OrderTypeType,
-        "Sort": UserSortTypeType,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "OrganizationId": str,
         "UserIds": str,
@@ -993,21 +849,14 @@
         "Marker": str,
         "Limit": int,
         "Fields": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LongRangeTypeTypeDef = TypedDict(
     "LongRangeTypeTypeDef",
     {
         "StartValue": int,
         "EndValue": int,
     },
     total=False,
@@ -1023,19 +872,21 @@
     "_OptionalSearchPrincipalTypeTypeDef",
     {
         "Roles": Sequence[PrincipalRoleTypeType],
     },
     total=False,
 )
 
+
 class SearchPrincipalTypeTypeDef(
     _RequiredSearchPrincipalTypeTypeDef, _OptionalSearchPrincipalTypeTypeDef
 ):
     pass
 
+
 GetCurrentUserRequestRequestTypeDef = TypedDict(
     "GetCurrentUserRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 
@@ -1052,19 +903,21 @@
         "Limit": int,
         "Fields": str,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetDocumentPathRequestRequestTypeDef(
     _RequiredGetDocumentPathRequestRequestTypeDef, _OptionalGetDocumentPathRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -1072,19 +925,21 @@
     {
         "AuthenticationToken": str,
         "IncludeCustomMetadata": bool,
     },
     total=False,
 )
 
+
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetDocumentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentVersionRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -1094,20 +949,22 @@
         "AuthenticationToken": str,
         "Fields": str,
         "IncludeCustomMetadata": bool,
     },
     total=False,
 )
 
+
 class GetDocumentVersionRequestRequestTypeDef(
     _RequiredGetDocumentVersionRequestRequestTypeDef,
     _OptionalGetDocumentVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetFolderPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetFolderPathRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalGetFolderPathRequestRequestTypeDef = TypedDict(
@@ -1117,19 +974,21 @@
         "Limit": int,
         "Fields": str,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetFolderPathRequestRequestTypeDef(
     _RequiredGetFolderPathRequestRequestTypeDef, _OptionalGetFolderPathRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetFolderRequestRequestTypeDef = TypedDict(
     "_RequiredGetFolderRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalGetFolderRequestRequestTypeDef = TypedDict(
@@ -1137,65 +996,42 @@
     {
         "AuthenticationToken": str,
         "IncludeCustomMetadata": bool,
     },
     total=False,
 )
 
+
 class GetFolderRequestRequestTypeDef(
     _RequiredGetFolderRequestRequestTypeDef, _OptionalGetFolderRequestRequestTypeDef
 ):
     pass
 
+
 GetResourcesRequestRequestTypeDef = TypedDict(
     "GetResourcesRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "UserId": str,
         "CollectionType": Literal["SHARED_WITH_ME"],
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Id": str,
-        "Name": str,
-        "ContentCreatedTimestamp": Union[datetime, str],
-        "ContentModifiedTimestamp": Union[datetime, str],
-        "ContentType": str,
-        "DocumentSizeInBytes": int,
-        "ParentFolderId": str,
-    },
-    total=False,
-)
-
 UploadMetadataTypeDef = TypedDict(
     "UploadMetadataTypeDef",
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
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
 PermissionInfoTypeDef = TypedDict(
     "PermissionInfoTypeDef",
     {
         "Role": RoleTypeType,
         "Type": RolePermissionTypeType,
     },
     total=False,
@@ -1211,20 +1047,22 @@
     "_OptionalRemoveAllResourcePermissionsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class RemoveAllResourcePermissionsRequestRequestTypeDef(
     _RequiredRemoveAllResourcePermissionsRequestRequestTypeDef,
     _OptionalRemoveAllResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRemoveResourcePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveResourcePermissionRequestRequestTypeDef",
     {
         "ResourceId": str,
         "PrincipalId": str,
     },
 )
@@ -1233,60 +1071,53 @@
     {
         "AuthenticationToken": str,
         "PrincipalType": PrincipalTypeType,
     },
     total=False,
 )
 
+
 class RemoveResourcePermissionRequestRequestTypeDef(
     _RequiredRemoveResourcePermissionRequestRequestTypeDef,
     _OptionalRemoveResourcePermissionRequestRequestTypeDef,
 ):
     pass
 
+
 ResourcePathComponentTypeDef = TypedDict(
     "ResourcePathComponentTypeDef",
     {
         "Id": str,
         "Name": str,
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
 _RequiredRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_OptionalRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class RestoreDocumentVersionsRequestRequestTypeDef(
     _RequiredRestoreDocumentVersionsRequestRequestTypeDef,
     _OptionalRestoreDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 SearchSortResultTypeDef = TypedDict(
     "SearchSortResultTypeDef",
     {
         "Field": OrderByFieldTypeType,
         "Order": SortOrderType,
     },
     total=False,
@@ -1305,19 +1136,21 @@
         "Name": str,
         "ParentFolderId": str,
         "ResourceState": ResourceStateTypeType,
     },
     total=False,
 )
 
+
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDocumentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentVersionRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -1326,20 +1159,22 @@
     {
         "AuthenticationToken": str,
         "VersionStatus": Literal["ACTIVE"],
     },
     total=False,
 )
 
+
 class UpdateDocumentVersionRequestRequestTypeDef(
     _RequiredUpdateDocumentVersionRequestRequestTypeDef,
     _OptionalUpdateDocumentVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFolderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFolderRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalUpdateFolderRequestRequestTypeDef = TypedDict(
@@ -1349,19 +1184,28 @@
         "Name": str,
         "ParentFolderId": str,
         "ResourceState": ResourceStateTypeType,
     },
     total=False,
 )
 
+
 class UpdateFolderRequestRequestTypeDef(
     _RequiredUpdateFolderRequestRequestTypeDef, _OptionalUpdateFolderRequestRequestTypeDef
 ):
     pass
 
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResourceMetadataTypeDef = TypedDict(
     "ResourceMetadataTypeDef",
     {
         "Type": ResourceTypeType,
         "Name": str,
         "OriginalName": str,
         "Id": str,
@@ -1384,68 +1228,70 @@
     {
         "AuthenticationToken": str,
         "NotificationOptions": NotificationOptionsTypeDef,
     },
     total=False,
 )
 
+
 class AddResourcePermissionsRequestRequestTypeDef(
     _RequiredAddResourcePermissionsRequestRequestTypeDef,
     _OptionalAddResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 AddResourcePermissionsResponseTypeDef = TypedDict(
     "AddResourcePermissionsResponseTypeDef",
     {
         "ShareResults": List[ShareResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFolderResponseTypeDef = TypedDict(
     "CreateFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRootFoldersResponseTypeDef = TypedDict(
     "DescribeRootFoldersResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderResponseTypeDef = TypedDict(
     "GetFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNotificationSubscriptionResponseTypeDef = TypedDict(
     "CreateNotificationSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationSubscriptionsResponseTypeDef = TypedDict(
     "DescribeNotificationSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "Username": str,
@@ -1462,19 +1308,21 @@
         "TimeZoneId": str,
         "StorageRule": StorageRuleTypeTypeDef,
         "AuthenticationToken": str,
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
@@ -1488,34 +1336,277 @@
         "TimeZoneId": str,
         "Locale": LocaleTypeType,
         "GrantPoweruserPrivileges": BooleanEnumTypeType,
     },
     total=False,
 )
 
+
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+
 UserStorageMetadataTypeDef = TypedDict(
     "UserStorageMetadataTypeDef",
     {
         "StorageUtilizedInBytes": int,
         "StorageRule": StorageRuleTypeTypeDef,
     },
     total=False,
 )
 
+DateRangeTypeTypeDef = TypedDict(
+    "DateRangeTypeTypeDef",
+    {
+        "StartValue": TimestampTypeDef,
+        "EndValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DescribeActivitiesRequestRequestTypeDef = TypedDict(
+    "DescribeActivitiesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "Limit": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Id": str,
+        "Name": str,
+        "ContentCreatedTimestamp": TimestampTypeDef,
+        "ContentModifiedTimestamp": TimestampTypeDef,
+        "ContentType": str,
+        "DocumentSizeInBytes": int,
+        "ParentFolderId": str,
+    },
+    total=False,
+)
+
+DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "DocumentId": str,
+        "VersionId": str,
+    },
+)
+_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
+    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Include": str,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
+    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "FolderId": str,
+    },
+)
+_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Sort": ResourceSortTypeType,
+        "Order": OrderTypeType,
+        "Type": FolderContentTypeType,
+        "Include": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
+    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "SearchQuery": str,
+    },
+)
+_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
+    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
+    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PrincipalId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
+    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+    },
+)
+_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
+    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+):
+    pass
+
+
+DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "UserIds": str,
+        "Query": str,
+        "Include": UserFilterTypeType,
+        "Order": OrderTypeType,
+        "Sort": UserSortTypeType,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeDocumentVersionsResponseTypeDef = TypedDict(
     "DescribeDocumentVersionsResponseTypeDef",
     {
         "DocumentVersions": List[DocumentVersionMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Id": str,
@@ -1531,53 +1622,36 @@
 )
 
 GetDocumentVersionResponseTypeDef = TypedDict(
     "GetDocumentVersionResponseTypeDef",
     {
         "Metadata": DocumentVersionMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGroupsResponseTypeDef = TypedDict(
     "DescribeGroupsResponseTypeDef",
     {
         "Groups": List[GroupMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParticipantsTypeDef = TypedDict(
     "ParticipantsTypeDef",
     {
         "Users": List[UserMetadataTypeDef],
         "Groups": List[GroupMetadataTypeDef],
     },
     total=False,
 )
 
-FiltersTypeDef = TypedDict(
-    "FiltersTypeDef",
-    {
-        "TextLocales": Sequence[LanguageCodeTypeType],
-        "ContentCategories": Sequence[ContentCategoryTypeType],
-        "ResourceTypes": Sequence[SearchResourceTypeType],
-        "Labels": Sequence[str],
-        "Principals": Sequence[SearchPrincipalTypeTypeDef],
-        "AncestorIds": Sequence[str],
-        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
-        "SizeRange": LongRangeTypeTypeDef,
-        "CreatedRange": DateRangeTypeTypeDef,
-        "ModifiedRange": DateRangeTypeTypeDef,
-    },
-    total=False,
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "Id": str,
         "Type": PrincipalTypeType,
         "Roles": List[PermissionInfoTypeDef],
     },
@@ -1610,113 +1684,99 @@
         "TimeZoneId": str,
         "Locale": LocaleTypeType,
         "Storage": UserStorageMetadataTypeDef,
     },
     total=False,
 )
 
+FiltersTypeDef = TypedDict(
+    "FiltersTypeDef",
+    {
+        "TextLocales": Sequence[LanguageCodeTypeType],
+        "ContentCategories": Sequence[ContentCategoryTypeType],
+        "ResourceTypes": Sequence[SearchResourceTypeType],
+        "Labels": Sequence[str],
+        "Principals": Sequence[SearchPrincipalTypeTypeDef],
+        "AncestorIds": Sequence[str],
+        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
+        "SizeRange": LongRangeTypeTypeDef,
+        "CreatedRange": DateRangeTypeTypeDef,
+        "ModifiedRange": DateRangeTypeTypeDef,
+    },
+    total=False,
+)
+
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentResponseTypeDef = TypedDict(
     "GetDocumentResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesResponseTypeDef = TypedDict(
     "GetResourcesResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateDocumentVersionUploadResponseTypeDef = TypedDict(
     "InitiateDocumentVersionUploadResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SearchResourcesRequestRequestTypeDef = TypedDict(
-    "SearchResourcesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentPathResponseTypeDef = TypedDict(
     "GetDocumentPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderPathResponseTypeDef = TypedDict(
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentMetadataTypeDef = TypedDict(
     "CommentMetadataTypeDef",
     {
         "CommentId": str,
@@ -1746,49 +1806,82 @@
         "Status": CommentStatusTypeType,
         "Visibility": CommentVisibilityTypeType,
         "RecipientId": str,
     },
     total=False,
 )
 
+
 class CommentTypeDef(_RequiredCommentTypeDef, _OptionalCommentTypeDef):
     pass
 
+
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "TotalNumberOfUsers": int,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCurrentUserResponseTypeDef = TypedDict(
     "GetCurrentUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchResourcesRequestRequestTypeDef = TypedDict(
+    "SearchResourcesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "Limit": int,
+        "Marker": str,
     },
+    total=False,
+)
+
+SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
         "TimeStamp": datetime,
@@ -1816,37 +1909,37 @@
     total=False,
 )
 
 CreateCommentResponseTypeDef = TypedDict(
     "CreateCommentResponseTypeDef",
     {
         "Comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCommentsResponseTypeDef = TypedDict(
     "DescribeCommentsResponseTypeDef",
     {
         "Comments": List[CommentTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeActivitiesResponseTypeDef = TypedDict(
     "DescribeActivitiesResponseTypeDef",
     {
         "UserActivities": List[ActivityTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "Items": List[ResponseItemTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/PKG-INFO` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workdocs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore workdocs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore workdocs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-workdocs"></a>
 
 # types-aiobotocore-workdocs
 
 [![PyPI - types-aiobotocore-workdocs](https://img.shields.io/pypi/v/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-workdocs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-workdocs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-workdocs?color=blue)](https://pypistats.org/packages/types-aiobotocore-workdocs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-workdocs)](https://pepy.tech/project/types-aiobotocore-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WorkDocs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [types-aiobotocore-workdocs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs/).
 
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
@@ -383,137 +382,138 @@
 )
 
 
 def check_value(value: ActivityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_workdocs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
     FolderMetadataTypeDef,
     CreateLabelsRequestRequestTypeDef,
     CreateNotificationSubscriptionRequestRequestTypeDef,
     SubscriptionTypeDef,
     StorageRuleTypeTypeDef,
-    DateRangeTypeTypeDef,
+    TimestampTypeDef,
     DeactivateUserRequestRequestTypeDef,
     DeleteCommentRequestRequestTypeDef,
     DeleteCustomMetadataRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
-    DescribeActivitiesRequestRequestTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCommentsRequestRequestTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
-    InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
+    DateRangeTypeTypeDef,
+    DescribeActivitiesRequestRequestTypeDef,
+    InitiateDocumentVersionUploadRequestRequestTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
-    FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
     UserTypeDef,
+    FiltersTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
-    SearchResourcesRequestRequestTypeDef,
-    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
+    SearchResourcesRequestRequestTypeDef,
+    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     ActivityTypeDef,
     ResponseItemTypeDef,
     CreateCommentResponseTypeDef,
     DescribeCommentsResponseTypeDef,
     DescribeActivitiesResponseTypeDef,
     SearchResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> AbortDocumentVersionUploadRequestRequestTypeDef:
+def get_value() -> AbortDocumentVersionUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-workdocs-2.5.2/types_aiobotocore_workdocs.egg-info/SOURCES.txt` & `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


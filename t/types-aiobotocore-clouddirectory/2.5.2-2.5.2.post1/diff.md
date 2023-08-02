# Comparing `tmp/types-aiobotocore-clouddirectory-2.5.2.tar.gz` & `tmp/types-aiobotocore-clouddirectory-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-clouddirectory-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-clouddirectory-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
```

## Comparing `types-aiobotocore-clouddirectory-2.5.2.tar` & `types-aiobotocore-clouddirectory-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.313821 types-aiobotocore-clouddirectory-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-07-08 01:43:21.309821 types-aiobotocore-clouddirectory-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.313821 types-aiobotocore-clouddirectory-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.305821 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59759 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59665 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25363 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-08 01:26:53.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86520 2023-07-08 01:26:55.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86393 2023-07-08 01:26:54.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:52.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.309821 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:21.000000 types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25249 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:34:21.000000 types-aiobotocore-clouddirectory-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59814 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59720 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25325 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25304 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    90540 2023-08-02 14:34:25.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90408 2023-08-02 14:34:23.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:22.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.929637 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:59.000000 types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/LICENSE` & `types-aiobotocore-clouddirectory-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2/PKG-INFO` & `types-aiobotocore-clouddirectory-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-clouddirectory
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore clouddirectory type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore clouddirectory type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-clouddirectory"></a>
 
 # types-aiobotocore-clouddirectory
 
 [![PyPI - types-aiobotocore-clouddirectory](https://img.shields.io/pypi/v/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-clouddirectory?color=blue)](https://pypistats.org/packages/types-aiobotocore-clouddirectory)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-clouddirectory)](https://pepy.tech/project/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudDirectory 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [types-aiobotocore-clouddirectory docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/).
 
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
@@ -401,121 +400,82 @@
 )
 
 
 def check_value(value: BatchReadExceptionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_clouddirectory.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
+    ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
-    TypedAttributeValueTypeDef,
+    TypedAttributeValueOutputTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
+    BlobTypeDef,
     CreateDirectoryRequestRequestTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
-    EnableDirectoryResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
-    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
-    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -531,124 +491,177 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
     BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    GetObjectInformationResponseTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DeleteDirectoryResponseTypeDef,
+    DeleteSchemaResponseTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDirectoryResponseTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PublishSchemaResponseTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
-    AttributeKeyAndValueTypeDef,
-    AttributeNameAndValueTypeDef,
-    LinkAttributeActionTypeDef,
-    ObjectAttributeActionTypeDef,
-    TypedAttributeValueRangeTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
-    FacetAttributeDefinitionTypeDef,
-    TypedLinkAttributeDefinitionTypeDef,
+    FacetAttributeDefinitionOutputTypeDef,
+    TypedLinkAttributeDefinitionOutputTypeDef,
     GetFacetResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
+    TypedAttributeValueTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
-    CreateObjectRequestRequestTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
-    AttachTypedLinkRequestRequestTypeDef,
-    BatchAttachTypedLinkTypeDef,
-    TypedLinkSpecifierTypeDef,
-    LinkAttributeUpdateTypeDef,
-    ObjectAttributeUpdateTypeDef,
-    ObjectAttributeRangeTypeDef,
-    TypedLinkAttributeRangeTypeDef,
-    FacetAttributeTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
+    FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
-    TypedLinkFacetAttributeUpdateTypeDef,
-    TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
+    AttributeKeyAndValueTypeDef,
+    AttributeNameAndValueTypeDef,
+    FacetAttributeDefinitionTypeDef,
+    LinkAttributeActionTypeDef,
+    ObjectAttributeActionTypeDef,
+    TypedAttributeValueRangeTypeDef,
+    TypedLinkAttributeDefinitionTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
-    BatchDetachTypedLinkTypeDef,
-    BatchGetLinkAttributesTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
-    DetachTypedLinkRequestRequestTypeDef,
-    GetLinkAttributesRequestRequestTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    ListFacetAttributesResponseTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    AttributeNameAndValueUnionTypeDef,
+    BatchAttachTypedLinkTypeDef,
+    TypedLinkSpecifierTypeDef,
+    FacetAttributeTypeDef,
+    LinkAttributeUpdateTypeDef,
+    ObjectAttributeUpdateTypeDef,
+    ObjectAttributeRangeTypeDef,
+    TypedLinkAttributeRangeTypeDef,
+    TypedLinkFacetAttributeUpdateTypeDef,
+    TypedLinkFacetTypeDef,
+    BatchWriteOperationResponseTypeDef,
+    BatchReadSuccessfulResponseTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    CreateObjectRequestRequestTypeDef,
+    AttachTypedLinkRequestRequestTypeDef,
+    BatchDetachTypedLinkTypeDef,
+    BatchGetLinkAttributesTypeDef,
+    DetachTypedLinkRequestRequestTypeDef,
+    GetLinkAttributesRequestRequestTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
+    FacetAttributeUnionTypeDef,
+    FacetAttributeUpdateTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
-    CreateFacetRequestRequestTypeDef,
-    FacetAttributeUpdateTypeDef,
-    ListFacetAttributesResponseTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
-    BatchWriteOperationResponseTypeDef,
-    BatchReadSuccessfulResponseTypeDef,
-    BatchWriteOperationTypeDef,
-    BatchReadOperationTypeDef,
-    UpdateFacetRequestRequestTypeDef,
     BatchWriteResponseTypeDef,
     BatchReadOperationResponseTypeDef,
+    CreateFacetRequestRequestTypeDef,
+    UpdateFacetRequestRequestTypeDef,
+    BatchWriteOperationTypeDef,
+    BatchReadOperationTypeDef,
+    BatchReadResponseTypeDef,
     BatchWriteRequestRequestTypeDef,
     BatchReadRequestRequestTypeDef,
-    BatchReadResponseTypeDef,
 )
 
 
-def get_structure() -> ObjectReferenceTypeDef:
+def get_value() -> ObjectReferenceTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/README.md` & `types-aiobotocore-clouddirectory-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-clouddirectory"></a>
 
 # types-aiobotocore-clouddirectory
 
 [![PyPI - types-aiobotocore-clouddirectory](https://img.shields.io/pypi/v/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-clouddirectory?color=blue)](https://pypistats.org/packages/types-aiobotocore-clouddirectory)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-clouddirectory)](https://pepy.tech/project/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudDirectory 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [types-aiobotocore-clouddirectory docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/).
 
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
@@ -368,121 +368,82 @@
 )
 
 
 def check_value(value: BatchReadExceptionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_clouddirectory.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
+    ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
-    TypedAttributeValueTypeDef,
+    TypedAttributeValueOutputTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
+    BlobTypeDef,
     CreateDirectoryRequestRequestTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
-    EnableDirectoryResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
-    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
-    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -498,124 +459,177 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
     BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    GetObjectInformationResponseTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DeleteDirectoryResponseTypeDef,
+    DeleteSchemaResponseTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDirectoryResponseTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PublishSchemaResponseTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
-    AttributeKeyAndValueTypeDef,
-    AttributeNameAndValueTypeDef,
-    LinkAttributeActionTypeDef,
-    ObjectAttributeActionTypeDef,
-    TypedAttributeValueRangeTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
-    FacetAttributeDefinitionTypeDef,
-    TypedLinkAttributeDefinitionTypeDef,
+    FacetAttributeDefinitionOutputTypeDef,
+    TypedLinkAttributeDefinitionOutputTypeDef,
     GetFacetResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
+    TypedAttributeValueTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
-    CreateObjectRequestRequestTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
-    AttachTypedLinkRequestRequestTypeDef,
-    BatchAttachTypedLinkTypeDef,
-    TypedLinkSpecifierTypeDef,
-    LinkAttributeUpdateTypeDef,
-    ObjectAttributeUpdateTypeDef,
-    ObjectAttributeRangeTypeDef,
-    TypedLinkAttributeRangeTypeDef,
-    FacetAttributeTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
+    FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
-    TypedLinkFacetAttributeUpdateTypeDef,
-    TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
+    AttributeKeyAndValueTypeDef,
+    AttributeNameAndValueTypeDef,
+    FacetAttributeDefinitionTypeDef,
+    LinkAttributeActionTypeDef,
+    ObjectAttributeActionTypeDef,
+    TypedAttributeValueRangeTypeDef,
+    TypedLinkAttributeDefinitionTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
-    BatchDetachTypedLinkTypeDef,
-    BatchGetLinkAttributesTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
-    DetachTypedLinkRequestRequestTypeDef,
-    GetLinkAttributesRequestRequestTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    ListFacetAttributesResponseTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    AttributeNameAndValueUnionTypeDef,
+    BatchAttachTypedLinkTypeDef,
+    TypedLinkSpecifierTypeDef,
+    FacetAttributeTypeDef,
+    LinkAttributeUpdateTypeDef,
+    ObjectAttributeUpdateTypeDef,
+    ObjectAttributeRangeTypeDef,
+    TypedLinkAttributeRangeTypeDef,
+    TypedLinkFacetAttributeUpdateTypeDef,
+    TypedLinkFacetTypeDef,
+    BatchWriteOperationResponseTypeDef,
+    BatchReadSuccessfulResponseTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    CreateObjectRequestRequestTypeDef,
+    AttachTypedLinkRequestRequestTypeDef,
+    BatchDetachTypedLinkTypeDef,
+    BatchGetLinkAttributesTypeDef,
+    DetachTypedLinkRequestRequestTypeDef,
+    GetLinkAttributesRequestRequestTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
+    FacetAttributeUnionTypeDef,
+    FacetAttributeUpdateTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
-    CreateFacetRequestRequestTypeDef,
-    FacetAttributeUpdateTypeDef,
-    ListFacetAttributesResponseTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
-    BatchWriteOperationResponseTypeDef,
-    BatchReadSuccessfulResponseTypeDef,
-    BatchWriteOperationTypeDef,
-    BatchReadOperationTypeDef,
-    UpdateFacetRequestRequestTypeDef,
     BatchWriteResponseTypeDef,
     BatchReadOperationResponseTypeDef,
+    CreateFacetRequestRequestTypeDef,
+    UpdateFacetRequestRequestTypeDef,
+    BatchWriteOperationTypeDef,
+    BatchReadOperationTypeDef,
+    BatchReadResponseTypeDef,
     BatchWriteRequestRequestTypeDef,
     BatchReadRequestRequestTypeDef,
-    BatchReadResponseTypeDef,
 )
 
 
-def get_structure() -> ObjectReferenceTypeDef:
+def get_value() -> ObjectReferenceTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/setup.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-clouddirectory",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with"
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
-    keywords="aiobotocore clouddirectory type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore clouddirectory type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_clouddirectory": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/"
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__init__.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/__main__.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudDirectory 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudDirectory 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
-    AttributeKeyAndValueTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
     AttributeKeyTypeDef,
-    AttributeNameAndValueTypeDef,
+    AttributeNameAndValueUnionTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateObjectResponseTypeDef,
@@ -61,15 +61,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeUnionTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     GetObjectInformationResponseTypeDef,
@@ -104,15 +104,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    TypedLinkSpecifierTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -190,15 +190,15 @@
 
     async def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#add_facet_to_object)
         """
@@ -260,15 +260,15 @@
     async def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueTypeDef]
+        Attributes: Sequence[AttributeNameAndValueUnionTypeDef]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_typed_link)
         """
@@ -324,15 +324,15 @@
         """
 
     async def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[FacetAttributeTypeDef] = ...,
+        Attributes: Sequence[FacetAttributeUnionTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -356,15 +356,15 @@
         """
 
     async def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -466,15 +466,15 @@
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_policy)
         """
 
     async def detach_typed_link(
-        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierTypeDef
+        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_typed_link)
         """
@@ -536,15 +536,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_facet)
         """
 
     async def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -957,15 +957,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_facet)
         """
 
     async def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_link_attributes)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/client.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
-    AttributeKeyAndValueTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
     AttributeKeyTypeDef,
-    AttributeNameAndValueTypeDef,
+    AttributeNameAndValueUnionTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateObjectResponseTypeDef,
@@ -61,15 +61,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeUnionTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     GetObjectInformationResponseTypeDef,
@@ -104,15 +104,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    TypedLinkSpecifierTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -185,15 +185,15 @@
         """
     async def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#add_facet_to_object)
         """
@@ -250,15 +250,15 @@
     async def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[AttributeNameAndValueTypeDef]
+        Attributes: Sequence[AttributeNameAndValueUnionTypeDef]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#attach_typed_link)
         """
@@ -308,15 +308,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_directory)
         """
     async def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[FacetAttributeTypeDef] = ...,
+        Attributes: Sequence[FacetAttributeUnionTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -338,15 +338,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#create_index)
         """
     async def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[AttributeKeyAndValueTypeDef] = ...,
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -437,15 +437,15 @@
         """
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_policy)
         """
     async def detach_typed_link(
-        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierTypeDef
+        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#detach_typed_link)
         """
@@ -500,15 +500,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#get_facet)
         """
     async def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -889,15 +889,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_facet)
         """
     async def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: TypedLinkSpecifierTypeDef,
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/client/#update_link_attributes)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/literals.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 
@@ -150,75 +150,75 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 
 class ListDevelopmentSchemaArnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevelopmentSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
         """
 
 
 class ListDirectoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdirectoriespaginator)
     """
 
     def paginate(
-        self, *, state: DirectoryStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, state: DirectoryStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDirectoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdirectoriespaginator)
         """
 
 
 class ListFacetAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetattributespaginator)
         """
 
 
 class ListFacetNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetnamespaginator)
         """
 
 
@@ -232,15 +232,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIncomingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 
@@ -253,30 +253,30 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIndexResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listindexpaginator)
         """
 
 
 class ListManagedSchemaArnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listmanagedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listmanagedschemaarnspaginator)
         """
 
 
@@ -289,15 +289,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 
@@ -308,15 +308,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 
@@ -328,15 +328,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 
@@ -350,15 +350,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOutgoingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 
@@ -370,75 +370,75 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 
 class ListPublishedSchemaArnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpublishedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPublishedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpublishedschemaarnspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTypedLinkFacetAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypedLinkFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
         """
 
 
 class ListTypedLinkFacetNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypedLinkFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
         """
 
 
@@ -449,13 +449,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/paginator.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         SchemaArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAppliedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAppliedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listappliedschemaarnspaginator)
         """
 
 class ListAttachedIndicesPaginator(AioPaginator):
@@ -146,71 +146,71 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         TargetReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListAttachedIndices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listattachedindicespaginator)
         """
 
 class ListDevelopmentSchemaArnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevelopmentSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDevelopmentSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdevelopmentschemaarnspaginator)
         """
 
 class ListDirectoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdirectoriespaginator)
     """
 
     def paginate(
-        self, *, state: DirectoryStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, state: DirectoryStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDirectoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listdirectoriespaginator)
         """
 
 class ListFacetAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetattributespaginator)
         """
 
 class ListFacetNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListFacetNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listfacetnamespaginator)
         """
 
 class ListIncomingTypedLinksPaginator(AioPaginator):
@@ -223,15 +223,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIncomingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIncomingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listincomingtypedlinkspaginator)
         """
 
 class ListIndexPaginator(AioPaginator):
@@ -243,29 +243,29 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         IndexReference: ObjectReferenceTypeDef,
         RangesOnIndexedValues: Sequence[ObjectAttributeRangeTypeDef] = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIndexResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListIndex.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listindexpaginator)
         """
 
 class ListManagedSchemaArnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listmanagedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListManagedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listmanagedschemaarnspaginator)
         """
 
 class ListObjectAttributesPaginator(AioPaginator):
@@ -277,15 +277,15 @@
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
         FacetFilter: SchemaFacetTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectattributespaginator)
         """
 
 class ListObjectParentPathsPaginator(AioPaginator):
@@ -295,15 +295,15 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectParentPathsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectParentPaths.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectparentpathspaginator)
         """
 
 class ListObjectPoliciesPaginator(AioPaginator):
@@ -314,15 +314,15 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListObjectPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListObjectPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listobjectpoliciespaginator)
         """
 
 class ListOutgoingTypedLinksPaginator(AioPaginator):
@@ -335,15 +335,15 @@
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
         FilterAttributeRanges: Sequence[TypedLinkAttributeRangeTypeDef] = ...,
         FilterTypedLink: TypedLinkSchemaAndFacetNameTypeDef = ...,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOutgoingTypedLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListOutgoingTypedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listoutgoingtypedlinkspaginator)
         """
 
 class ListPolicyAttachmentsPaginator(AioPaginator):
@@ -354,71 +354,71 @@
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         PolicyReference: ObjectReferenceTypeDef,
         ConsistencyLevel: ConsistencyLevelType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPolicyAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpolicyattachmentspaginator)
         """
 
 class ListPublishedSchemaArnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpublishedschemaarnspaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPublishedSchemaArnsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListPublishedSchemaArns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listpublishedschemaarnspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTypedLinkFacetAttributesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypedLinkFacetAttributesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetAttributes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetattributespaginator)
         """
 
 class ListTypedLinkFacetNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
     """
 
     def paginate(
-        self, *, SchemaArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SchemaArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypedLinkFacetNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.ListTypedLinkFacetNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#listtypedlinkfacetnamespaginator)
         """
 
 class LookupPolicyPaginator(AioPaginator):
@@ -428,13 +428,13 @@
     """
 
     def paginate(
         self,
         *,
         DirectoryArn: str,
         ObjectReference: ObjectReferenceTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[LookupPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Paginator.LookupPolicy.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/paginators/#lookuppolicypaginator)
         """
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.py` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_clouddirectory.type_defs import ObjectReferenceTypeDef
 
-    data: ObjectReferenceTypeDef = {...}
+    data: ObjectReferenceTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -31,114 +31,74 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
-    "ApplySchemaResponseTypeDef",
-    "AttachObjectResponseTypeDef",
-    "AttachToIndexResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
-    "TypedAttributeValueTypeDef",
+    "TypedAttributeValueOutputTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
+    "BlobTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
-    "CreateDirectoryResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateObjectResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResponseTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
-    "DeleteSchemaResponseTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
-    "DetachFromIndexResponseTypeDef",
-    "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
-    "DisableDirectoryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
-    "EnableDirectoryResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
-    "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
-    "GetSchemaAsJsonResponseTypeDef",
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAppliedSchemaArnsRequestRequestTypeDef",
-    "ListAppliedSchemaArnsResponseTypeDef",
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListDirectoriesRequestRequestTypeDef",
-    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetAttributesRequestRequestTypeDef",
-    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
     "ListFacetNamesRequestRequestTypeDef",
-    "ListFacetNamesResponseTypeDef",
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
     "ListManagedSchemaArnsRequestRequestTypeDef",
-    "ListManagedSchemaArnsResponseTypeDef",
-    "ListObjectChildrenResponseTypeDef",
-    "ListObjectPoliciesResponseTypeDef",
-    "ListPolicyAttachmentsResponseTypeDef",
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
-    "ListPublishedSchemaArnsResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
-    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
-    "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
-    "PutSchemaFromJsonResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
-    "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
-    "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
-    "UpgradePublishedSchemaResponseTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
     "BatchAttachObjectTypeDef",
     "BatchAttachPolicyTypeDef",
     "BatchAttachToIndexTypeDef",
     "BatchDeleteObjectTypeDef",
@@ -154,120 +114,173 @@
     "BatchListPolicyAttachmentsTypeDef",
     "BatchLookupPolicyTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DetachFromIndexRequestRequestTypeDef",
     "DetachObjectRequestRequestTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "GetObjectInformationRequestRequestTypeDef",
-    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListAttachedIndicesRequestRequestTypeDef",
     "ListObjectChildrenRequestRequestTypeDef",
-    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     "ListObjectParentPathsRequestRequestTypeDef",
     "ListObjectParentsRequestRequestTypeDef",
-    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
-    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
-    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
     "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "GetObjectInformationResponseTypeDef",
-    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
+    "ApplySchemaResponseTypeDef",
+    "AttachObjectResponseTypeDef",
+    "AttachToIndexResponseTypeDef",
+    "CreateDirectoryResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateObjectResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DeleteDirectoryResponseTypeDef",
+    "DeleteSchemaResponseTypeDef",
+    "DetachFromIndexResponseTypeDef",
+    "DetachObjectResponseTypeDef",
+    "DisableDirectoryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDirectoryResponseTypeDef",
+    "GetAppliedSchemaVersionResponseTypeDef",
+    "GetObjectInformationResponseTypeDef",
+    "GetSchemaAsJsonResponseTypeDef",
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    "ListAppliedSchemaArnsResponseTypeDef",
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    "ListFacetNamesResponseTypeDef",
+    "ListManagedSchemaArnsResponseTypeDef",
+    "ListObjectChildrenResponseTypeDef",
+    "ListObjectPoliciesResponseTypeDef",
+    "ListPolicyAttachmentsResponseTypeDef",
+    "ListPublishedSchemaArnsResponseTypeDef",
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    "PublishSchemaResponseTypeDef",
+    "PutSchemaFromJsonResponseTypeDef",
+    "UpdateObjectAttributesResponseTypeDef",
+    "UpdateSchemaResponseTypeDef",
+    "UpgradeAppliedSchemaResponseTypeDef",
+    "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
-    "AttributeKeyAndValueTypeDef",
-    "AttributeNameAndValueTypeDef",
-    "LinkAttributeActionTypeDef",
-    "ObjectAttributeActionTypeDef",
-    "TypedAttributeValueRangeTypeDef",
+    "AttributeKeyAndValueOutputTypeDef",
+    "AttributeNameAndValueOutputTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
-    "FacetAttributeDefinitionTypeDef",
-    "TypedLinkAttributeDefinitionTypeDef",
+    "FacetAttributeDefinitionOutputTypeDef",
+    "TypedLinkAttributeDefinitionOutputTypeDef",
     "GetFacetResponseTypeDef",
+    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "BatchAddFacetToObjectTypeDef",
-    "BatchCreateObjectTypeDef",
+    "TypedAttributeValueTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
-    "CreateObjectRequestRequestTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
-    "AttachTypedLinkRequestRequestTypeDef",
-    "BatchAttachTypedLinkTypeDef",
-    "TypedLinkSpecifierTypeDef",
-    "LinkAttributeUpdateTypeDef",
-    "ObjectAttributeUpdateTypeDef",
-    "ObjectAttributeRangeTypeDef",
-    "TypedLinkAttributeRangeTypeDef",
-    "FacetAttributeTypeDef",
+    "TypedLinkSpecifierOutputTypeDef",
+    "FacetAttributeOutputTypeDef",
     "ListTypedLinkFacetAttributesResponseTypeDef",
-    "TypedLinkFacetAttributeUpdateTypeDef",
-    "TypedLinkFacetTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
+    "AttributeKeyAndValueTypeDef",
+    "AttributeNameAndValueTypeDef",
+    "FacetAttributeDefinitionTypeDef",
+    "LinkAttributeActionTypeDef",
+    "ObjectAttributeActionTypeDef",
+    "TypedAttributeValueRangeTypeDef",
+    "TypedLinkAttributeDefinitionTypeDef",
     "BatchListAttachedIndicesResponseTypeDef",
     "BatchListIndexResponseTypeDef",
     "ListAttachedIndicesResponseTypeDef",
     "ListIndexResponseTypeDef",
     "AttachTypedLinkResponseTypeDef",
     "BatchAttachTypedLinkResponseTypeDef",
-    "BatchDetachTypedLinkTypeDef",
-    "BatchGetLinkAttributesTypeDef",
     "BatchListIncomingTypedLinksResponseTypeDef",
     "BatchListOutgoingTypedLinksResponseTypeDef",
-    "DetachTypedLinkRequestRequestTypeDef",
-    "GetLinkAttributesRequestRequestTypeDef",
     "ListIncomingTypedLinksResponseTypeDef",
     "ListOutgoingTypedLinksResponseTypeDef",
+    "ListFacetAttributesResponseTypeDef",
+    "AttributeKeyAndValueUnionTypeDef",
+    "BatchAddFacetToObjectTypeDef",
+    "BatchCreateObjectTypeDef",
+    "AttributeNameAndValueUnionTypeDef",
+    "BatchAttachTypedLinkTypeDef",
+    "TypedLinkSpecifierTypeDef",
+    "FacetAttributeTypeDef",
+    "LinkAttributeUpdateTypeDef",
+    "ObjectAttributeUpdateTypeDef",
+    "ObjectAttributeRangeTypeDef",
+    "TypedLinkAttributeRangeTypeDef",
+    "TypedLinkFacetAttributeUpdateTypeDef",
+    "TypedLinkFacetTypeDef",
+    "BatchWriteOperationResponseTypeDef",
+    "BatchReadSuccessfulResponseTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
+    "CreateObjectRequestRequestTypeDef",
+    "AttachTypedLinkRequestRequestTypeDef",
+    "BatchDetachTypedLinkTypeDef",
+    "BatchGetLinkAttributesTypeDef",
+    "DetachTypedLinkRequestRequestTypeDef",
+    "GetLinkAttributesRequestRequestTypeDef",
+    "TypedLinkSpecifierUnionTypeDef",
+    "FacetAttributeUnionTypeDef",
+    "FacetAttributeUpdateTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
     "BatchListIncomingTypedLinksTypeDef",
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
-    "CreateFacetRequestRequestTypeDef",
-    "FacetAttributeUpdateTypeDef",
-    "ListFacetAttributesResponseTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
-    "BatchWriteOperationResponseTypeDef",
-    "BatchReadSuccessfulResponseTypeDef",
-    "BatchWriteOperationTypeDef",
-    "BatchReadOperationTypeDef",
-    "UpdateFacetRequestRequestTypeDef",
     "BatchWriteResponseTypeDef",
     "BatchReadOperationResponseTypeDef",
+    "CreateFacetRequestRequestTypeDef",
+    "UpdateFacetRequestRequestTypeDef",
+    "BatchWriteOperationTypeDef",
+    "BatchReadOperationTypeDef",
+    "BatchReadResponseTypeDef",
     "BatchWriteRequestRequestTypeDef",
     "BatchReadRequestRequestTypeDef",
-    "BatchReadResponseTypeDef",
 )
 
 ObjectReferenceTypeDef = TypedDict(
     "ObjectReferenceTypeDef",
     {
         "Selector": str,
     },
@@ -287,36 +300,22 @@
     "ApplySchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
 
-ApplySchemaResponseTypeDef = TypedDict(
-    "ApplySchemaResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachObjectResponseTypeDef = TypedDict(
-    "AttachObjectResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachToIndexResponseTypeDef = TypedDict(
-    "AttachToIndexResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TypedLinkSchemaAndFacetNameTypeDef = TypedDict(
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
@@ -329,22 +328,22 @@
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
 )
 
-TypedAttributeValueTypeDef = TypedDict(
-    "TypedAttributeValueTypeDef",
+TypedAttributeValueOutputTypeDef = TypedDict(
+    "TypedAttributeValueOutputTypeDef",
     {
         "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
+        "BinaryValue": bytes,
         "BooleanValue": bool,
         "NumberValue": str,
-        "DatetimeValue": Union[datetime, str],
+        "DatetimeValue": datetime,
     },
     total=False,
 )
 
 BatchAttachObjectResponseTypeDef = TypedDict(
     "BatchAttachObjectResponseTypeDef",
     {
@@ -451,79 +450,37 @@
     "BatchUpdateObjectAttributesResponseTypeDef",
     {
         "ObjectIdentifier": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateDirectoryRequestRequestTypeDef = TypedDict(
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
 
-CreateDirectoryResponseTypeDef = TypedDict(
-    "CreateDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "Name": str,
-        "ObjectIdentifier": str,
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateObjectResponseTypeDef = TypedDict(
-    "CreateObjectResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSchemaRequestRequestTypeDef = TypedDict(
     "CreateSchemaRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DeleteDirectoryResponseTypeDef = TypedDict(
-    "DeleteDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFacetRequestRequestTypeDef = TypedDict(
     "DeleteFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -531,46 +488,22 @@
 DeleteSchemaRequestRequestTypeDef = TypedDict(
     "DeleteSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-DetachFromIndexResponseTypeDef = TypedDict(
-    "DetachFromIndexResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DetachObjectResponseTypeDef = TypedDict(
-    "DetachObjectResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DirectoryTypeDef = TypedDict(
     "DirectoryTypeDef",
     {
         "Name": str,
         "DirectoryArn": str,
         "State": DirectoryStateType,
         "CreationDateTime": datetime,
@@ -581,42 +514,28 @@
 DisableDirectoryRequestRequestTypeDef = TypedDict(
     "DisableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DisableDirectoryResponseTypeDef = TypedDict(
-    "DisableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
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
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-EnableDirectoryResponseTypeDef = TypedDict(
-    "EnableDirectoryResponseTypeDef",
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
     {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": RuleTypeType,
+        "Parameters": Dict[str, str],
     },
+    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
@@ -645,22 +564,14 @@
 GetAppliedSchemaVersionRequestRequestTypeDef = TypedDict(
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetAppliedSchemaVersionResponseTypeDef = TypedDict(
-    "GetAppliedSchemaVersionResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDirectoryRequestRequestTypeDef = TypedDict(
     "GetDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
@@ -675,62 +586,32 @@
 GetSchemaAsJsonRequestRequestTypeDef = TypedDict(
     "GetSchemaAsJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetSchemaAsJsonResponseTypeDef = TypedDict(
-    "GetSchemaAsJsonResponseTypeDef",
-    {
-        "Name": str,
-        "Document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTypedLinkFacetInformationRequestRequestTypeDef = TypedDict(
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    {
-        "IdentityAttributeOrder": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-    },
-)
-_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
-    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppliedSchemaArnsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 _OptionalListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
@@ -739,99 +620,39 @@
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAppliedSchemaArnsRequestRequestTypeDef(
     _RequiredListAppliedSchemaArnsRequestRequestTypeDef,
     _OptionalListAppliedSchemaArnsRequestRequestTypeDef,
 ):
     pass
 
-
-ListAppliedSchemaArnsResponseTypeDef = TypedDict(
-    "ListAppliedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevelopmentSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    {
-        "state": DirectoryStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDirectoriesRequestRequestTypeDef = TypedDict(
     "ListDirectoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "state": DirectoryStateType,
     },
     total=False,
 )
 
-_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
-    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -840,44 +661,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFacetAttributesRequestRequestTypeDef(
     _RequiredListFacetAttributesRequestRequestTypeDef,
     _OptionalListFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
-    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListFacetNamesRequestRequestTypeDef = TypedDict(
@@ -885,135 +682,39 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListFacetNamesRequestRequestTypeDef(
     _RequiredListFacetNamesRequestRequestTypeDef, _OptionalListFacetNamesRequestRequestTypeDef
 ):
     pass
 
-
-ListFacetNamesResponseTypeDef = TypedDict(
-    "ListFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListManagedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListManagedSchemaArnsResponseTypeDef = TypedDict(
-    "ListManagedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectChildrenResponseTypeDef = TypedDict(
-    "ListObjectChildrenResponseTypeDef",
-    {
-        "Children": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectPoliciesResponseTypeDef = TypedDict(
-    "ListObjectPoliciesResponseTypeDef",
-    {
-        "AttachedPolicyIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyAttachmentsResponseTypeDef = TypedDict(
-    "ListPolicyAttachmentsResponseTypeDef",
-    {
-        "ObjectIdentifiers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPublishedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListPublishedSchemaArnsResponseTypeDef = TypedDict(
-    "ListPublishedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1021,54 +722,29 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
-    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -1077,44 +753,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTypedLinkFacetAttributesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
-    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 _OptionalListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
@@ -1122,41 +774,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTypedLinkFacetNamesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetNamesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetNamesRequestRequestTypeDef,
 ):
     pass
 
-
-ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
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
 PolicyAttachmentTypeDef = TypedDict(
     "PolicyAttachmentTypeDef",
     {
         "PolicyId": str,
         "ObjectIdentifier": str,
         "PolicyType": str,
     },
@@ -1175,88 +806,44 @@
     {
         "MinorVersion": str,
         "Name": str,
     },
     total=False,
 )
 
-
 class PublishSchemaRequestRequestTypeDef(
     _RequiredPublishSchemaRequestRequestTypeDef, _OptionalPublishSchemaRequestRequestTypeDef
 ):
     pass
 
-
-PublishSchemaResponseTypeDef = TypedDict(
-    "PublishSchemaResponseTypeDef",
-    {
-        "PublishedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutSchemaFromJsonRequestRequestTypeDef = TypedDict(
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
-PutSchemaFromJsonResponseTypeDef = TypedDict(
-    "PutSchemaFromJsonResponseTypeDef",
-    {
-        "Arn": str,
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
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateObjectAttributesResponseTypeDef = TypedDict(
-    "UpdateObjectAttributesResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSchemaRequestRequestTypeDef = TypedDict(
     "UpdateSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradeAppliedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
@@ -1264,31 +851,20 @@
     "_OptionalUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class UpgradeAppliedSchemaRequestRequestTypeDef(
     _RequiredUpgradeAppliedSchemaRequestRequestTypeDef,
     _OptionalUpgradeAppliedSchemaRequestRequestTypeDef,
 ):
     pass
 
-
-UpgradeAppliedSchemaResponseTypeDef = TypedDict(
-    "UpgradeAppliedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradePublishedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DevelopmentSchemaArn": str,
         "PublishedSchemaArn": str,
         "MinorVersion": str,
     },
@@ -1297,30 +873,20 @@
     "_OptionalUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class UpgradePublishedSchemaRequestRequestTypeDef(
     _RequiredUpgradePublishedSchemaRequestRequestTypeDef,
     _OptionalUpgradePublishedSchemaRequestRequestTypeDef,
 ):
     pass
 
-
-UpgradePublishedSchemaResponseTypeDef = TypedDict(
-    "UpgradePublishedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachObjectRequestRequestTypeDef = TypedDict(
     "AttachObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ParentReference": ObjectReferenceTypeDef,
         "ChildReference": ObjectReferenceTypeDef,
         "LinkName": str,
@@ -1396,21 +962,19 @@
     "_OptionalBatchDetachObjectTypeDef",
     {
         "BatchReferenceName": str,
     },
     total=False,
 )
 
-
 class BatchDetachObjectTypeDef(
     _RequiredBatchDetachObjectTypeDef, _OptionalBatchDetachObjectTypeDef
 ):
     pass
 
-
 BatchDetachPolicyTypeDef = TypedDict(
     "BatchDetachPolicyTypeDef",
     {
         "PolicyReference": ObjectReferenceTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1433,21 +997,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListAttachedIndicesTypeDef(
     _RequiredBatchListAttachedIndicesTypeDef, _OptionalBatchListAttachedIndicesTypeDef
 ):
     pass
 
-
 _RequiredBatchListObjectChildrenTypeDef = TypedDict(
     "_RequiredBatchListObjectChildrenTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectChildrenTypeDef = TypedDict(
@@ -1455,21 +1017,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListObjectChildrenTypeDef(
     _RequiredBatchListObjectChildrenTypeDef, _OptionalBatchListObjectChildrenTypeDef
 ):
     pass
 
-
 _RequiredBatchListObjectParentPathsTypeDef = TypedDict(
     "_RequiredBatchListObjectParentPathsTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectParentPathsTypeDef = TypedDict(
@@ -1477,21 +1037,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListObjectParentPathsTypeDef(
     _RequiredBatchListObjectParentPathsTypeDef, _OptionalBatchListObjectParentPathsTypeDef
 ):
     pass
 
-
 _RequiredBatchListObjectParentsTypeDef = TypedDict(
     "_RequiredBatchListObjectParentsTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectParentsTypeDef = TypedDict(
@@ -1499,21 +1057,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListObjectParentsTypeDef(
     _RequiredBatchListObjectParentsTypeDef, _OptionalBatchListObjectParentsTypeDef
 ):
     pass
 
-
 _RequiredBatchListObjectPoliciesTypeDef = TypedDict(
     "_RequiredBatchListObjectPoliciesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectPoliciesTypeDef = TypedDict(
@@ -1521,21 +1077,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListObjectPoliciesTypeDef(
     _RequiredBatchListObjectPoliciesTypeDef, _OptionalBatchListObjectPoliciesTypeDef
 ):
     pass
 
-
 _RequiredBatchListPolicyAttachmentsTypeDef = TypedDict(
     "_RequiredBatchListPolicyAttachmentsTypeDef",
     {
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListPolicyAttachmentsTypeDef = TypedDict(
@@ -1543,21 +1097,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListPolicyAttachmentsTypeDef(
     _RequiredBatchListPolicyAttachmentsTypeDef, _OptionalBatchListPolicyAttachmentsTypeDef
 ):
     pass
 
-
 _RequiredBatchLookupPolicyTypeDef = TypedDict(
     "_RequiredBatchLookupPolicyTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchLookupPolicyTypeDef = TypedDict(
@@ -1565,21 +1117,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchLookupPolicyTypeDef(
     _RequiredBatchLookupPolicyTypeDef, _OptionalBatchLookupPolicyTypeDef
 ):
     pass
 
-
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1622,46 +1172,20 @@
     "_OptionalGetObjectInformationRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class GetObjectInformationRequestRequestTypeDef(
     _RequiredGetObjectInformationRequestRequestTypeDef,
     _OptionalGetObjectInformationRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "TargetReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
-    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedIndicesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedIndicesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TargetReference": ObjectReferenceTypeDef,
     },
 )
@@ -1671,22 +1195,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListAttachedIndicesRequestRequestTypeDef(
     _RequiredListAttachedIndicesRequestRequestTypeDef,
     _OptionalListAttachedIndicesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListObjectChildrenRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectChildrenRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1696,45 +1218,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListObjectChildrenRequestRequestTypeDef(
     _RequiredListObjectChildrenRequestRequestTypeDef,
     _OptionalListObjectChildrenRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
-    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectParentPathsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentPathsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1743,22 +1240,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListObjectParentPathsRequestRequestTypeDef(
     _RequiredListObjectParentPathsRequestRequestTypeDef,
     _OptionalListObjectParentPathsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListObjectParentsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1769,45 +1264,19 @@
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
         "IncludeAllLinksToEachParent": bool,
     },
     total=False,
 )
 
-
 class ListObjectParentsRequestRequestTypeDef(
     _RequiredListObjectParentsRequestRequestTypeDef, _OptionalListObjectParentsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
-    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListObjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectPoliciesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1817,46 +1286,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListObjectPoliciesRequestRequestTypeDef(
     _RequiredListObjectPoliciesRequestRequestTypeDef,
     _OptionalListObjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "PolicyReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
-    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyAttachmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyAttachmentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
@@ -1866,45 +1309,20 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListPolicyAttachmentsRequestRequestTypeDef(
     _RequiredListPolicyAttachmentsRequestRequestTypeDef,
     _OptionalListPolicyAttachmentsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class LookupPolicyRequestLookupPolicyPaginateTypeDef(
-    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
-    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
-):
-    pass
-
-
 _RequiredLookupPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredLookupPolicyRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1913,21 +1331,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class LookupPolicyRequestRequestTypeDef(
     _RequiredLookupPolicyRequestRequestTypeDef, _OptionalLookupPolicyRequestRequestTypeDef
 ):
     pass
 
-
 BatchGetObjectAttributesTypeDef = TypedDict(
     "BatchGetObjectAttributesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
         "SchemaFacet": SchemaFacetTypeDef,
         "AttributeNames": Sequence[str],
     },
@@ -1954,21 +1370,19 @@
         "NextToken": str,
         "MaxResults": int,
         "FacetFilter": SchemaFacetTypeDef,
     },
     total=False,
 )
 
-
 class BatchListObjectAttributesTypeDef(
     _RequiredBatchListObjectAttributesTypeDef, _OptionalBatchListObjectAttributesTypeDef
 ):
     pass
 
-
 BatchRemoveFacetFromObjectTypeDef = TypedDict(
     "BatchRemoveFacetFromObjectTypeDef",
     {
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1986,88 +1400,329 @@
     "_OptionalGetObjectAttributesRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestRequestTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectAttributesRequestRequestTypeDef(
+    _RequiredListObjectAttributesRequestRequestTypeDef,
+    _OptionalListObjectAttributesRequestRequestTypeDef,
+):
+    pass
+
+RemoveFacetFromObjectRequestRequestTypeDef = TypedDict(
+    "RemoveFacetFromObjectRequestRequestTypeDef",
+    {
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+
+ApplySchemaResponseTypeDef = TypedDict(
+    "ApplySchemaResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachObjectResponseTypeDef = TypedDict(
+    "AttachObjectResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachToIndexResponseTypeDef = TypedDict(
+    "AttachToIndexResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResponseTypeDef = TypedDict(
+    "CreateDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "Name": str,
+        "ObjectIdentifier": str,
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateObjectResponseTypeDef = TypedDict(
+    "CreateObjectResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResponseTypeDef = TypedDict(
+    "DeleteDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachFromIndexResponseTypeDef = TypedDict(
+    "DetachFromIndexResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachObjectResponseTypeDef = TypedDict(
+    "DetachObjectResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDirectoryResponseTypeDef = TypedDict(
+    "DisableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
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
+EnableDirectoryResponseTypeDef = TypedDict(
+    "EnableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppliedSchemaVersionResponseTypeDef = TypedDict(
+    "GetAppliedSchemaVersionResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetObjectInformationResponseTypeDef = TypedDict(
     "GetObjectInformationResponseTypeDef",
     {
         "SchemaFacets": List[SchemaFacetTypeDef],
         "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+GetSchemaAsJsonResponseTypeDef = TypedDict(
+    "GetSchemaAsJsonResponseTypeDef",
     {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "Name": str,
+        "Document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+
+GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
+    "GetTypedLinkFacetInformationResponseTypeDef",
     {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "IdentityAttributeOrder": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListAppliedSchemaArnsResponseTypeDef = TypedDict(
+    "ListAppliedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
-    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-):
-    pass
+ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListFacetNamesResponseTypeDef = TypedDict(
+    "ListFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestRequestTypeDef",
+ListManagedSchemaArnsResponseTypeDef = TypedDict(
+    "ListManagedSchemaArnsResponseTypeDef",
     {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListObjectAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestRequestTypeDef",
+
+ListObjectChildrenResponseTypeDef = TypedDict(
+    "ListObjectChildrenResponseTypeDef",
     {
+        "Children": Dict[str, str],
         "NextToken": str,
-        "MaxResults": int,
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListObjectPoliciesResponseTypeDef = TypedDict(
+    "ListObjectPoliciesResponseTypeDef",
+    {
+        "AttachedPolicyIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListObjectAttributesRequestRequestTypeDef(
-    _RequiredListObjectAttributesRequestRequestTypeDef,
-    _OptionalListObjectAttributesRequestRequestTypeDef,
-):
-    pass
+ListPolicyAttachmentsResponseTypeDef = TypedDict(
+    "ListPolicyAttachmentsResponseTypeDef",
+    {
+        "ObjectIdentifiers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListPublishedSchemaArnsResponseTypeDef = TypedDict(
+    "ListPublishedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RemoveFacetFromObjectRequestRequestTypeDef = TypedDict(
-    "RemoveFacetFromObjectRequestRequestTypeDef",
+ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishSchemaResponseTypeDef = TypedDict(
+    "PublishSchemaResponseTypeDef",
     {
+        "PublishedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaFromJsonResponseTypeDef = TypedDict(
+    "PutSchemaFromJsonResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateObjectAttributesResponseTypeDef = TypedDict(
+    "UpdateObjectAttributesResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradeAppliedSchemaResponseTypeDef = TypedDict(
+    "UpgradeAppliedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
         "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradePublishedSchemaResponseTypeDef = TypedDict(
+    "UpgradePublishedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
@@ -2080,19 +1735,17 @@
         "ParentReference": ObjectReferenceTypeDef,
         "LinkName": str,
         "BatchReferenceName": str,
     },
     total=False,
 )
 
-
 class BatchCreateIndexTypeDef(_RequiredBatchCreateIndexTypeDef, _OptionalBatchCreateIndexTypeDef):
     pass
 
-
 _RequiredCreateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIndexRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
         "IsUnique": bool,
     },
@@ -2102,93 +1755,50 @@
     {
         "ParentReference": ObjectReferenceTypeDef,
         "LinkName": str,
     },
     total=False,
 )
 
-
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
-
-AttributeKeyAndValueTypeDef = TypedDict(
-    "AttributeKeyAndValueTypeDef",
+AttributeKeyAndValueOutputTypeDef = TypedDict(
+    "AttributeKeyAndValueOutputTypeDef",
     {
         "Key": AttributeKeyTypeDef,
-        "Value": TypedAttributeValueTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
     },
 )
 
-AttributeNameAndValueTypeDef = TypedDict(
-    "AttributeNameAndValueTypeDef",
+AttributeNameAndValueOutputTypeDef = TypedDict(
+    "AttributeNameAndValueOutputTypeDef",
     {
         "AttributeName": str,
-        "Value": TypedAttributeValueTypeDef,
-    },
-)
-
-LinkAttributeActionTypeDef = TypedDict(
-    "LinkAttributeActionTypeDef",
-    {
-        "AttributeActionType": UpdateActionTypeType,
-        "AttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-ObjectAttributeActionTypeDef = TypedDict(
-    "ObjectAttributeActionTypeDef",
-    {
-        "ObjectAttributeActionType": UpdateActionTypeType,
-        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
-    "_RequiredTypedAttributeValueRangeTypeDef",
-    {
-        "StartMode": RangeModeType,
-        "EndMode": RangeModeType,
-    },
-)
-_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
-    "_OptionalTypedAttributeValueRangeTypeDef",
-    {
-        "StartValue": TypedAttributeValueTypeDef,
-        "EndValue": TypedAttributeValueTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
     },
-    total=False,
 )
 
-
-class TypedAttributeValueRangeTypeDef(
-    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
-):
-    pass
-
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
 ListObjectParentPathsResponseTypeDef = TypedDict(
     "ListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchListObjectParentsResponseTypeDef = TypedDict(
     "BatchListObjectParentsResponseTypeDef",
     {
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
@@ -2199,267 +1809,765 @@
 
 ListObjectParentsResponseTypeDef = TypedDict(
     "ListObjectParentsResponseTypeDef",
     {
         "Parents": Dict[str, str],
         "NextToken": str,
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDirectoryResponseTypeDef = TypedDict(
     "GetDirectoryResponseTypeDef",
     {
         "Directory": DirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDirectoriesResponseTypeDef = TypedDict(
     "ListDirectoriesResponseTypeDef",
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredFacetAttributeDefinitionTypeDef",
+_RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionOutputTypeDef",
     {
         "Type": FacetAttributeTypeType,
     },
 )
-_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalFacetAttributeDefinitionTypeDef",
+_OptionalFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionOutputTypeDef",
     {
-        "DefaultValue": TypedAttributeValueTypeDef,
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
         "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
+        "Rules": Dict[str, RuleOutputTypeDef],
     },
     total=False,
 )
 
-
-class FacetAttributeDefinitionTypeDef(
-    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
+class FacetAttributeDefinitionOutputTypeDef(
+    _RequiredFacetAttributeDefinitionOutputTypeDef, _OptionalFacetAttributeDefinitionOutputTypeDef
 ):
     pass
 
-
-_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeDefinitionTypeDef",
+_RequiredTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionOutputTypeDef",
     {
         "Name": str,
         "Type": FacetAttributeTypeType,
         "RequiredBehavior": RequiredAttributeBehaviorType,
     },
 )
-_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeDefinitionTypeDef",
+_OptionalTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionOutputTypeDef",
     {
-        "DefaultValue": TypedAttributeValueTypeDef,
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
         "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
+        "Rules": Dict[str, RuleOutputTypeDef],
     },
     total=False,
 )
 
-
-class TypedLinkAttributeDefinitionTypeDef(
-    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
+class TypedLinkAttributeDefinitionOutputTypeDef(
+    _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
+    _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
 ):
     pass
 
-
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryArn": str,
+    },
+)
+_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
+    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "DirectoryArn": str,
+        "TargetReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PolicyToPathTypeDef = TypedDict(
-    "PolicyToPathTypeDef",
+class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
+    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+):
+    pass
+
+ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     {
-        "Path": str,
-        "Policies": List[PolicyAttachmentTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredAddFacetToObjectRequestRequestTypeDef",
+ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "state": DirectoryStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalAddFacetToObjectRequestRequestTypeDef",
+
+_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
+    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+):
+    pass
+
+_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class AddFacetToObjectRequestRequestTypeDef(
-    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
+    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
 ):
     pass
 
+ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-BatchAddFacetToObjectTypeDef = TypedDict(
-    "BatchAddFacetToObjectTypeDef",
+_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
+_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredBatchCreateObjectTypeDef = TypedDict(
-    "_RequiredBatchCreateObjectTypeDef",
+class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
+    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+):
+    pass
+
+_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     {
-        "SchemaFacet": Sequence[SchemaFacetTypeDef],
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalBatchCreateObjectTypeDef = TypedDict(
-    "_OptionalBatchCreateObjectTypeDef",
+_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     {
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
-        "BatchReferenceName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
+    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+):
+    pass
 
-class BatchCreateObjectTypeDef(
-    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
+    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
 ):
     pass
 
+_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "PolicyReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-BatchGetLinkAttributesResponseTypeDef = TypedDict(
-    "BatchGetLinkAttributesResponseTypeDef",
+class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
+    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+):
+    pass
+
+ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-BatchGetObjectAttributesResponseTypeDef = TypedDict(
-    "BatchGetObjectAttributesResponseTypeDef",
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-BatchListObjectAttributesResponseTypeDef = TypedDict(
-    "BatchListObjectAttributesResponseTypeDef",
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "NextToken": str,
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateObjectRequestRequestTypeDef",
+class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
+    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+        "SchemaArn": str,
     },
 )
-_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateObjectRequestRequestTypeDef",
+_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
+    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+):
+    pass
 
-class CreateObjectRequestRequestTypeDef(
-    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class LookupPolicyRequestLookupPolicyPaginateTypeDef(
+    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
+    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+PolicyToPathTypeDef = TypedDict(
+    "PolicyToPathTypeDef",
+    {
+        "Path": str,
+        "Policies": List[PolicyAttachmentTypeDef],
+    },
+    total=False,
+)
+
+TypedAttributeValueTypeDef = TypedDict(
+    "TypedAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "BooleanValue": bool,
+        "NumberValue": str,
+        "DatetimeValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+BatchGetLinkAttributesResponseTypeDef = TypedDict(
+    "BatchGetLinkAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+    },
+    total=False,
+)
+
+BatchGetObjectAttributesResponseTypeDef = TypedDict(
+    "BatchGetObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+    },
+    total=False,
+)
+
+BatchListObjectAttributesResponseTypeDef = TypedDict(
+    "BatchListObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
 
 GetLinkAttributesResponseTypeDef = TypedDict(
     "GetLinkAttributesResponseTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesResponseTypeDef = TypedDict(
     "GetObjectAttributesResponseTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IndexAttachmentTypeDef = TypedDict(
     "IndexAttachmentTypeDef",
     {
-        "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
+        "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
         "ObjectIdentifier": str,
     },
     total=False,
 )
 
 ListObjectAttributesResponseTypeDef = TypedDict(
     "ListObjectAttributesResponseTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttachTypedLinkRequestRequestTypeDef = TypedDict(
-    "AttachTypedLinkRequestRequestTypeDef",
+TypedLinkSpecifierOutputTypeDef = TypedDict(
+    "TypedLinkSpecifierOutputTypeDef",
     {
-        "DirectoryArn": str,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
+    },
+)
+
+_RequiredFacetAttributeOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalFacetAttributeOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeOutputTypeDef",
+    {
+        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+    total=False,
+)
+
+class FacetAttributeOutputTypeDef(
+    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
+):
+    pass
+
+ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchLookupPolicyResponseTypeDef = TypedDict(
+    "BatchLookupPolicyResponseTypeDef",
+    {
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+LookupPolicyResponseTypeDef = TypedDict(
+    "LookupPolicyResponseTypeDef",
+    {
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttributeKeyAndValueTypeDef = TypedDict(
+    "AttributeKeyAndValueTypeDef",
+    {
+        "Key": AttributeKeyTypeDef,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+AttributeNameAndValueTypeDef = TypedDict(
+    "AttributeNameAndValueTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionTypeDef",
+    {
+        "Type": FacetAttributeTypeType,
+    },
+)
+_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
+    },
+    total=False,
+)
+
+class FacetAttributeDefinitionTypeDef(
+    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
+):
+    pass
+
+LinkAttributeActionTypeDef = TypedDict(
+    "LinkAttributeActionTypeDef",
+    {
+        "AttributeActionType": UpdateActionTypeType,
+        "AttributeUpdateValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+ObjectAttributeActionTypeDef = TypedDict(
+    "ObjectAttributeActionTypeDef",
+    {
+        "ObjectAttributeActionType": UpdateActionTypeType,
+        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
+    "_RequiredTypedAttributeValueRangeTypeDef",
+    {
+        "StartMode": RangeModeType,
+        "EndMode": RangeModeType,
+    },
+)
+_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
+    "_OptionalTypedAttributeValueRangeTypeDef",
+    {
+        "StartValue": TypedAttributeValueTypeDef,
+        "EndValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+class TypedAttributeValueRangeTypeDef(
+    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
+):
+    pass
+
+_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionTypeDef",
+    {
+        "Name": str,
+        "Type": FacetAttributeTypeType,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+)
+_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
+    },
+    total=False,
+)
+
+class TypedLinkAttributeDefinitionTypeDef(
+    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
+):
+    pass
+
+BatchListAttachedIndicesResponseTypeDef = TypedDict(
+    "BatchListAttachedIndicesResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+BatchListIndexResponseTypeDef = TypedDict(
+    "BatchListIndexResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListAttachedIndicesResponseTypeDef = TypedDict(
+    "ListAttachedIndicesResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndexResponseTypeDef = TypedDict(
+    "ListIndexResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachTypedLinkResponseTypeDef = TypedDict(
+    "AttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchAttachTypedLinkResponseTypeDef = TypedDict(
+    "BatchAttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+    },
+    total=False,
+)
+
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AttributeKeyAndValueUnionTypeDef = Union[
+    AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef
+]
+BatchAddFacetToObjectTypeDef = TypedDict(
+    "BatchAddFacetToObjectTypeDef",
+    {
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+
+_RequiredBatchCreateObjectTypeDef = TypedDict(
+    "_RequiredBatchCreateObjectTypeDef",
+    {
+        "SchemaFacet": Sequence[SchemaFacetTypeDef],
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+    },
+)
+_OptionalBatchCreateObjectTypeDef = TypedDict(
+    "_OptionalBatchCreateObjectTypeDef",
+    {
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+        "BatchReferenceName": str,
+    },
+    total=False,
+)
+
+class BatchCreateObjectTypeDef(
+    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+):
+    pass
+
+AttributeNameAndValueUnionTypeDef = Union[
+    AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef
+]
 BatchAttachTypedLinkTypeDef = TypedDict(
     "BatchAttachTypedLinkTypeDef",
     {
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "Attributes": Sequence[AttributeNameAndValueTypeDef],
@@ -2468,18 +2576,37 @@
 
 TypedLinkSpecifierTypeDef = TypedDict(
     "TypedLinkSpecifierTypeDef",
     {
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": List[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
+    },
+)
+
+_RequiredFacetAttributeTypeDef = TypedDict(
+    "_RequiredFacetAttributeTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalFacetAttributeTypeDef = TypedDict(
+    "_OptionalFacetAttributeTypeDef",
+    {
+        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
     },
+    total=False,
 )
 
+class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
+    pass
+
 LinkAttributeUpdateTypeDef = TypedDict(
     "LinkAttributeUpdateTypeDef",
     {
         "AttributeKey": AttributeKeyTypeDef,
         "AttributeAction": LinkAttributeActionTypeDef,
     },
     total=False,
@@ -2513,51 +2640,19 @@
     "_OptionalTypedLinkAttributeRangeTypeDef",
     {
         "AttributeName": str,
     },
     total=False,
 )
 
-
 class TypedLinkAttributeRangeTypeDef(
     _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
 ):
     pass
 
-
-_RequiredFacetAttributeTypeDef = TypedDict(
-    "_RequiredFacetAttributeTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalFacetAttributeTypeDef = TypedDict(
-    "_OptionalFacetAttributeTypeDef",
-    {
-        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-    total=False,
-)
-
-
-class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
-    pass
-
-
-ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetAttributesResponseTypeDef",
-    {
-        "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
         "Action": UpdateActionTypeType,
     },
 )
@@ -2567,82 +2662,109 @@
     {
         "Name": str,
         "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
         "IdentityAttributeOrder": Sequence[str],
     },
 )
 
-BatchLookupPolicyResponseTypeDef = TypedDict(
-    "BatchLookupPolicyResponseTypeDef",
+BatchWriteOperationResponseTypeDef = TypedDict(
+    "BatchWriteOperationResponseTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
+        "CreateObject": BatchCreateObjectResponseTypeDef,
+        "AttachObject": BatchAttachObjectResponseTypeDef,
+        "DetachObject": BatchDetachObjectResponseTypeDef,
+        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
+        "DeleteObject": Dict[str, Any],
+        "AddFacetToObject": Dict[str, Any],
+        "RemoveFacetFromObject": Dict[str, Any],
+        "AttachPolicy": Dict[str, Any],
+        "DetachPolicy": Dict[str, Any],
+        "CreateIndex": BatchCreateIndexResponseTypeDef,
+        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
+        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
+        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
+        "DetachTypedLink": Dict[str, Any],
+        "UpdateLinkAttributes": Dict[str, Any],
     },
     total=False,
 )
 
-LookupPolicyResponseTypeDef = TypedDict(
-    "LookupPolicyResponseTypeDef",
+BatchReadSuccessfulResponseTypeDef = TypedDict(
+    "BatchReadSuccessfulResponseTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
+        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
+        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
+        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
+        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
+        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
+        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
+        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
+        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
+        "ListIndex": BatchListIndexResponseTypeDef,
+        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
+        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
+        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
+        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
     },
+    total=False,
 )
 
-BatchListAttachedIndicesResponseTypeDef = TypedDict(
-    "BatchListAttachedIndicesResponseTypeDef",
+_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
-    total=False,
 )
-
-BatchListIndexResponseTypeDef = TypedDict(
-    "BatchListIndexResponseTypeDef",
+_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
     },
     total=False,
 )
 
-ListAttachedIndicesResponseTypeDef = TypedDict(
-    "ListAttachedIndicesResponseTypeDef",
-    {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class AddFacetToObjectRequestRequestTypeDef(
+    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+):
+    pass
 
-ListIndexResponseTypeDef = TypedDict(
-    "ListIndexResponseTypeDef",
+_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryArn": str,
+        "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
-
-AttachTypedLinkResponseTypeDef = TypedDict(
-    "AttachTypedLinkResponseTypeDef",
+_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateObjectRequestRequestTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
     },
+    total=False,
 )
 
-BatchAttachTypedLinkResponseTypeDef = TypedDict(
-    "BatchAttachTypedLinkResponseTypeDef",
+class CreateObjectRequestRequestTypeDef(
+    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+):
+    pass
+
+AttachTypedLinkRequestRequestTypeDef = TypedDict(
+    "AttachTypedLinkRequestRequestTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "DirectoryArn": str,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueUnionTypeDef],
     },
-    total=False,
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
@@ -2652,32 +2774,14 @@
     "BatchGetLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
-    {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
-    {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DetachTypedLinkRequestRequestTypeDef = TypedDict(
     "DetachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
 )
@@ -2694,37 +2798,28 @@
     "_OptionalGetLinkAttributesRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
-
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
-    {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
+TypedLinkSpecifierUnionTypeDef = Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
+FacetAttributeUnionTypeDef = Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]
+FacetAttributeUpdateTypeDef = TypedDict(
+    "FacetAttributeUpdateTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attribute": FacetAttributeTypeDef,
+        "Action": UpdateActionTypeType,
     },
+    total=False,
 )
 
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
@@ -2769,44 +2864,40 @@
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class BatchListIndexTypeDef(_RequiredBatchListIndexTypeDef, _OptionalBatchListIndexTypeDef):
     pass
 
-
 _RequiredListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_RequiredListIndexRequestListIndexPaginateTypeDef",
     {
         "DirectoryArn": str,
         "IndexReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_OptionalListIndexRequestListIndexPaginateTypeDef",
     {
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListIndexRequestListIndexPaginateTypeDef(
     _RequiredListIndexRequestListIndexPaginateTypeDef,
     _OptionalListIndexRequestListIndexPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListIndexRequestRequestTypeDef = TypedDict(
     "_RequiredListIndexRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "IndexReference": ObjectReferenceTypeDef,
     },
 )
@@ -2817,21 +2908,19 @@
         "MaxResults": int,
         "NextToken": str,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListIndexRequestRequestTypeDef(
     _RequiredListIndexRequestRequestTypeDef, _OptionalListIndexRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchListIncomingTypedLinksTypeDef = TypedDict(
     "_RequiredBatchListIncomingTypedLinksTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListIncomingTypedLinksTypeDef = TypedDict(
@@ -2841,21 +2930,19 @@
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListIncomingTypedLinksTypeDef(
     _RequiredBatchListIncomingTypedLinksTypeDef, _OptionalBatchListIncomingTypedLinksTypeDef
 ):
     pass
 
-
 _RequiredBatchListOutgoingTypedLinksTypeDef = TypedDict(
     "_RequiredBatchListOutgoingTypedLinksTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListOutgoingTypedLinksTypeDef = TypedDict(
@@ -2865,47 +2952,43 @@
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class BatchListOutgoingTypedLinksTypeDef(
     _RequiredBatchListOutgoingTypedLinksTypeDef, _OptionalBatchListOutgoingTypedLinksTypeDef
 ):
     pass
 
-
 _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef(
     _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListIncomingTypedLinksRequestRequestTypeDef = TypedDict(
     "_RequiredListIncomingTypedLinksRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2917,48 +3000,44 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListIncomingTypedLinksRequestRequestTypeDef(
     _RequiredListIncomingTypedLinksRequestRequestTypeDef,
     _OptionalListIncomingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef(
     _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListOutgoingTypedLinksRequestRequestTypeDef = TypedDict(
     "_RequiredListOutgoingTypedLinksRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2970,125 +3049,98 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class ListOutgoingTypedLinksRequestRequestTypeDef(
     _RequiredListOutgoingTypedLinksRequestRequestTypeDef,
     _OptionalListOutgoingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFacetRequestRequestTypeDef",
+UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
+        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
+        "IdentityAttributeOrder": Sequence[str],
     },
 )
-_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFacetRequestRequestTypeDef",
+
+CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "CreateTypedLinkFacetRequestRequestTypeDef",
     {
-        "Attributes": Sequence[FacetAttributeTypeDef],
-        "ObjectType": ObjectTypeType,
-        "FacetStyle": FacetStyleType,
+        "SchemaArn": str,
+        "Facet": TypedLinkFacetTypeDef,
     },
-    total=False,
 )
 
-
-class CreateFacetRequestRequestTypeDef(
-    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
-):
-    pass
-
-
-FacetAttributeUpdateTypeDef = TypedDict(
-    "FacetAttributeUpdateTypeDef",
+BatchWriteResponseTypeDef = TypedDict(
+    "BatchWriteResponseTypeDef",
     {
-        "Attribute": FacetAttributeTypeDef,
-        "Action": UpdateActionTypeType,
+        "Responses": List[BatchWriteOperationResponseTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
+BatchReadOperationResponseTypeDef = TypedDict(
+    "BatchReadOperationResponseTypeDef",
     {
-        "Attributes": List[FacetAttributeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
+        "ExceptionResponse": BatchReadExceptionTypeDef,
     },
+    total=False,
 )
 
-UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "UpdateTypedLinkFacetRequestRequestTypeDef",
+_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
-        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
-        "IdentityAttributeOrder": Sequence[str],
     },
 )
-
-CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "CreateTypedLinkFacetRequestRequestTypeDef",
+_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFacetRequestRequestTypeDef",
     {
-        "SchemaArn": str,
-        "Facet": TypedLinkFacetTypeDef,
+        "Attributes": Sequence[FacetAttributeUnionTypeDef],
+        "ObjectType": ObjectTypeType,
+        "FacetStyle": FacetStyleType,
     },
+    total=False,
 )
 
-BatchWriteOperationResponseTypeDef = TypedDict(
-    "BatchWriteOperationResponseTypeDef",
+class CreateFacetRequestRequestTypeDef(
+    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFacetRequestRequestTypeDef",
     {
-        "CreateObject": BatchCreateObjectResponseTypeDef,
-        "AttachObject": BatchAttachObjectResponseTypeDef,
-        "DetachObject": BatchDetachObjectResponseTypeDef,
-        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
-        "DeleteObject": Dict[str, Any],
-        "AddFacetToObject": Dict[str, Any],
-        "RemoveFacetFromObject": Dict[str, Any],
-        "AttachPolicy": Dict[str, Any],
-        "DetachPolicy": Dict[str, Any],
-        "CreateIndex": BatchCreateIndexResponseTypeDef,
-        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
-        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
-        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
-        "DetachTypedLink": Dict[str, Any],
-        "UpdateLinkAttributes": Dict[str, Any],
+        "SchemaArn": str,
+        "Name": str,
     },
-    total=False,
 )
-
-BatchReadSuccessfulResponseTypeDef = TypedDict(
-    "BatchReadSuccessfulResponseTypeDef",
+_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFacetRequestRequestTypeDef",
     {
-        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
-        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
-        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
-        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
-        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
-        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
-        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
-        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
-        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
-        "ListIndex": BatchListIndexResponseTypeDef,
-        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
-        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
-        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
-        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
+        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
+        "ObjectType": ObjectTypeType,
     },
     total=False,
 )
 
+class UpdateFacetRequestRequestTypeDef(
+    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
+):
+    pass
+
 BatchWriteOperationTypeDef = TypedDict(
     "BatchWriteOperationTypeDef",
     {
         "CreateObject": BatchCreateObjectTypeDef,
         "AttachObject": BatchAttachObjectTypeDef,
         "DetachObject": BatchDetachObjectTypeDef,
         "UpdateObjectAttributes": BatchUpdateObjectAttributesTypeDef,
@@ -3124,52 +3176,20 @@
         "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksTypeDef,
         "ListIncomingTypedLinks": BatchListIncomingTypedLinksTypeDef,
         "GetLinkAttributes": BatchGetLinkAttributesTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFacetRequestRequestTypeDef",
-    {
-        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
-        "ObjectType": ObjectTypeType,
-    },
-    total=False,
-)
-
-
-class UpdateFacetRequestRequestTypeDef(
-    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
-):
-    pass
-
-
-BatchWriteResponseTypeDef = TypedDict(
-    "BatchWriteResponseTypeDef",
-    {
-        "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchReadOperationResponseTypeDef = TypedDict(
-    "BatchReadOperationResponseTypeDef",
+BatchReadResponseTypeDef = TypedDict(
+    "BatchReadResponseTypeDef",
     {
-        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
-        "ExceptionResponse": BatchReadExceptionTypeDef,
+        "Responses": List[BatchReadOperationResponseTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 BatchWriteRequestRequestTypeDef = TypedDict(
     "BatchWriteRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "Operations": Sequence[BatchWriteOperationTypeDef],
@@ -3187,21 +3207,11 @@
     "_OptionalBatchReadRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
-
 class BatchReadRequestRequestTypeDef(
     _RequiredBatchReadRequestRequestTypeDef, _OptionalBatchReadRequestRequestTypeDef
 ):
     pass
-
-
-BatchReadResponseTypeDef = TypedDict(
-    "BatchReadResponseTypeDef",
-    {
-        "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory/type_defs.pyi` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_clouddirectory.type_defs import ObjectReferenceTypeDef
 
-    data: ObjectReferenceTypeDef = {...}
+    data: ObjectReferenceTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -31,113 +31,75 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
-    "ApplySchemaResponseTypeDef",
-    "AttachObjectResponseTypeDef",
-    "AttachToIndexResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
-    "TypedAttributeValueTypeDef",
+    "TypedAttributeValueOutputTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
+    "BlobTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
-    "CreateDirectoryResponseTypeDef",
-    "CreateIndexResponseTypeDef",
-    "CreateObjectResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResponseTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
-    "DeleteSchemaResponseTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
-    "DetachFromIndexResponseTypeDef",
-    "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
-    "DisableDirectoryResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
-    "EnableDirectoryResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
-    "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
-    "GetSchemaAsJsonResponseTypeDef",
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAppliedSchemaArnsRequestRequestTypeDef",
-    "ListAppliedSchemaArnsResponseTypeDef",
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListDirectoriesRequestRequestTypeDef",
-    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetAttributesRequestRequestTypeDef",
-    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
     "ListFacetNamesRequestRequestTypeDef",
-    "ListFacetNamesResponseTypeDef",
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
     "ListManagedSchemaArnsRequestRequestTypeDef",
-    "ListManagedSchemaArnsResponseTypeDef",
-    "ListObjectChildrenResponseTypeDef",
-    "ListObjectPoliciesResponseTypeDef",
-    "ListPolicyAttachmentsResponseTypeDef",
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
-    "ListPublishedSchemaArnsResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
-    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
-    "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
-    "PutSchemaFromJsonResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
-    "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
-    "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
-    "UpgradePublishedSchemaResponseTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
     "BatchAttachObjectTypeDef",
     "BatchAttachPolicyTypeDef",
     "BatchAttachToIndexTypeDef",
     "BatchDeleteObjectTypeDef",
@@ -153,120 +115,173 @@
     "BatchListPolicyAttachmentsTypeDef",
     "BatchLookupPolicyTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DetachFromIndexRequestRequestTypeDef",
     "DetachObjectRequestRequestTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "GetObjectInformationRequestRequestTypeDef",
-    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListAttachedIndicesRequestRequestTypeDef",
     "ListObjectChildrenRequestRequestTypeDef",
-    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     "ListObjectParentPathsRequestRequestTypeDef",
     "ListObjectParentsRequestRequestTypeDef",
-    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
-    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
-    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
     "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "GetObjectInformationResponseTypeDef",
-    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
+    "ApplySchemaResponseTypeDef",
+    "AttachObjectResponseTypeDef",
+    "AttachToIndexResponseTypeDef",
+    "CreateDirectoryResponseTypeDef",
+    "CreateIndexResponseTypeDef",
+    "CreateObjectResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DeleteDirectoryResponseTypeDef",
+    "DeleteSchemaResponseTypeDef",
+    "DetachFromIndexResponseTypeDef",
+    "DetachObjectResponseTypeDef",
+    "DisableDirectoryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDirectoryResponseTypeDef",
+    "GetAppliedSchemaVersionResponseTypeDef",
+    "GetObjectInformationResponseTypeDef",
+    "GetSchemaAsJsonResponseTypeDef",
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    "ListAppliedSchemaArnsResponseTypeDef",
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    "ListFacetNamesResponseTypeDef",
+    "ListManagedSchemaArnsResponseTypeDef",
+    "ListObjectChildrenResponseTypeDef",
+    "ListObjectPoliciesResponseTypeDef",
+    "ListPolicyAttachmentsResponseTypeDef",
+    "ListPublishedSchemaArnsResponseTypeDef",
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    "PublishSchemaResponseTypeDef",
+    "PutSchemaFromJsonResponseTypeDef",
+    "UpdateObjectAttributesResponseTypeDef",
+    "UpdateSchemaResponseTypeDef",
+    "UpgradeAppliedSchemaResponseTypeDef",
+    "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
-    "AttributeKeyAndValueTypeDef",
-    "AttributeNameAndValueTypeDef",
-    "LinkAttributeActionTypeDef",
-    "ObjectAttributeActionTypeDef",
-    "TypedAttributeValueRangeTypeDef",
+    "AttributeKeyAndValueOutputTypeDef",
+    "AttributeNameAndValueOutputTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
-    "FacetAttributeDefinitionTypeDef",
-    "TypedLinkAttributeDefinitionTypeDef",
+    "FacetAttributeDefinitionOutputTypeDef",
+    "TypedLinkAttributeDefinitionOutputTypeDef",
     "GetFacetResponseTypeDef",
+    "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
+    "ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
+    "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "BatchAddFacetToObjectTypeDef",
-    "BatchCreateObjectTypeDef",
+    "TypedAttributeValueTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
-    "CreateObjectRequestRequestTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
-    "AttachTypedLinkRequestRequestTypeDef",
-    "BatchAttachTypedLinkTypeDef",
-    "TypedLinkSpecifierTypeDef",
-    "LinkAttributeUpdateTypeDef",
-    "ObjectAttributeUpdateTypeDef",
-    "ObjectAttributeRangeTypeDef",
-    "TypedLinkAttributeRangeTypeDef",
-    "FacetAttributeTypeDef",
+    "TypedLinkSpecifierOutputTypeDef",
+    "FacetAttributeOutputTypeDef",
     "ListTypedLinkFacetAttributesResponseTypeDef",
-    "TypedLinkFacetAttributeUpdateTypeDef",
-    "TypedLinkFacetTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
+    "AttributeKeyAndValueTypeDef",
+    "AttributeNameAndValueTypeDef",
+    "FacetAttributeDefinitionTypeDef",
+    "LinkAttributeActionTypeDef",
+    "ObjectAttributeActionTypeDef",
+    "TypedAttributeValueRangeTypeDef",
+    "TypedLinkAttributeDefinitionTypeDef",
     "BatchListAttachedIndicesResponseTypeDef",
     "BatchListIndexResponseTypeDef",
     "ListAttachedIndicesResponseTypeDef",
     "ListIndexResponseTypeDef",
     "AttachTypedLinkResponseTypeDef",
     "BatchAttachTypedLinkResponseTypeDef",
-    "BatchDetachTypedLinkTypeDef",
-    "BatchGetLinkAttributesTypeDef",
     "BatchListIncomingTypedLinksResponseTypeDef",
     "BatchListOutgoingTypedLinksResponseTypeDef",
-    "DetachTypedLinkRequestRequestTypeDef",
-    "GetLinkAttributesRequestRequestTypeDef",
     "ListIncomingTypedLinksResponseTypeDef",
     "ListOutgoingTypedLinksResponseTypeDef",
+    "ListFacetAttributesResponseTypeDef",
+    "AttributeKeyAndValueUnionTypeDef",
+    "BatchAddFacetToObjectTypeDef",
+    "BatchCreateObjectTypeDef",
+    "AttributeNameAndValueUnionTypeDef",
+    "BatchAttachTypedLinkTypeDef",
+    "TypedLinkSpecifierTypeDef",
+    "FacetAttributeTypeDef",
+    "LinkAttributeUpdateTypeDef",
+    "ObjectAttributeUpdateTypeDef",
+    "ObjectAttributeRangeTypeDef",
+    "TypedLinkAttributeRangeTypeDef",
+    "TypedLinkFacetAttributeUpdateTypeDef",
+    "TypedLinkFacetTypeDef",
+    "BatchWriteOperationResponseTypeDef",
+    "BatchReadSuccessfulResponseTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
+    "CreateObjectRequestRequestTypeDef",
+    "AttachTypedLinkRequestRequestTypeDef",
+    "BatchDetachTypedLinkTypeDef",
+    "BatchGetLinkAttributesTypeDef",
+    "DetachTypedLinkRequestRequestTypeDef",
+    "GetLinkAttributesRequestRequestTypeDef",
+    "TypedLinkSpecifierUnionTypeDef",
+    "FacetAttributeUnionTypeDef",
+    "FacetAttributeUpdateTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
     "BatchListIncomingTypedLinksTypeDef",
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
-    "CreateFacetRequestRequestTypeDef",
-    "FacetAttributeUpdateTypeDef",
-    "ListFacetAttributesResponseTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
-    "BatchWriteOperationResponseTypeDef",
-    "BatchReadSuccessfulResponseTypeDef",
-    "BatchWriteOperationTypeDef",
-    "BatchReadOperationTypeDef",
-    "UpdateFacetRequestRequestTypeDef",
     "BatchWriteResponseTypeDef",
     "BatchReadOperationResponseTypeDef",
+    "CreateFacetRequestRequestTypeDef",
+    "UpdateFacetRequestRequestTypeDef",
+    "BatchWriteOperationTypeDef",
+    "BatchReadOperationTypeDef",
+    "BatchReadResponseTypeDef",
     "BatchWriteRequestRequestTypeDef",
     "BatchReadRequestRequestTypeDef",
-    "BatchReadResponseTypeDef",
 )
 
 ObjectReferenceTypeDef = TypedDict(
     "ObjectReferenceTypeDef",
     {
         "Selector": str,
     },
@@ -286,36 +301,22 @@
     "ApplySchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
 
-ApplySchemaResponseTypeDef = TypedDict(
-    "ApplySchemaResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachObjectResponseTypeDef = TypedDict(
-    "AttachObjectResponseTypeDef",
-    {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AttachToIndexResponseTypeDef = TypedDict(
-    "AttachToIndexResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AttachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TypedLinkSchemaAndFacetNameTypeDef = TypedDict(
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
@@ -328,22 +329,22 @@
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
 )
 
-TypedAttributeValueTypeDef = TypedDict(
-    "TypedAttributeValueTypeDef",
+TypedAttributeValueOutputTypeDef = TypedDict(
+    "TypedAttributeValueOutputTypeDef",
     {
         "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
+        "BinaryValue": bytes,
         "BooleanValue": bool,
         "NumberValue": str,
-        "DatetimeValue": Union[datetime, str],
+        "DatetimeValue": datetime,
     },
     total=False,
 )
 
 BatchAttachObjectResponseTypeDef = TypedDict(
     "BatchAttachObjectResponseTypeDef",
     {
@@ -450,79 +451,37 @@
     "BatchUpdateObjectAttributesResponseTypeDef",
     {
         "ObjectIdentifier": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateDirectoryRequestRequestTypeDef = TypedDict(
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
 
-CreateDirectoryResponseTypeDef = TypedDict(
-    "CreateDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "Name": str,
-        "ObjectIdentifier": str,
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateIndexResponseTypeDef = TypedDict(
-    "CreateIndexResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateObjectResponseTypeDef = TypedDict(
-    "CreateObjectResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateSchemaRequestRequestTypeDef = TypedDict(
     "CreateSchemaRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DeleteDirectoryResponseTypeDef = TypedDict(
-    "DeleteDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFacetRequestRequestTypeDef = TypedDict(
     "DeleteFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -530,46 +489,22 @@
 DeleteSchemaRequestRequestTypeDef = TypedDict(
     "DeleteSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-DeleteSchemaResponseTypeDef = TypedDict(
-    "DeleteSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-DetachFromIndexResponseTypeDef = TypedDict(
-    "DetachFromIndexResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DetachObjectResponseTypeDef = TypedDict(
-    "DetachObjectResponseTypeDef",
-    {
-        "DetachedObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DirectoryTypeDef = TypedDict(
     "DirectoryTypeDef",
     {
         "Name": str,
         "DirectoryArn": str,
         "State": DirectoryStateType,
         "CreationDateTime": datetime,
@@ -580,42 +515,28 @@
 DisableDirectoryRequestRequestTypeDef = TypedDict(
     "DisableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-DisableDirectoryResponseTypeDef = TypedDict(
-    "DisableDirectoryResponseTypeDef",
-    {
-        "DirectoryArn": str,
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
 EnableDirectoryRequestRequestTypeDef = TypedDict(
     "EnableDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
-EnableDirectoryResponseTypeDef = TypedDict(
-    "EnableDirectoryResponseTypeDef",
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
     {
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": RuleTypeType,
+        "Parameters": Dict[str, str],
     },
+    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
@@ -644,22 +565,14 @@
 GetAppliedSchemaVersionRequestRequestTypeDef = TypedDict(
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetAppliedSchemaVersionResponseTypeDef = TypedDict(
-    "GetAppliedSchemaVersionResponseTypeDef",
-    {
-        "AppliedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDirectoryRequestRequestTypeDef = TypedDict(
     "GetDirectoryRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 
@@ -674,60 +587,32 @@
 GetSchemaAsJsonRequestRequestTypeDef = TypedDict(
     "GetSchemaAsJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
 
-GetSchemaAsJsonResponseTypeDef = TypedDict(
-    "GetSchemaAsJsonResponseTypeDef",
-    {
-        "Name": str,
-        "Document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTypedLinkFacetInformationRequestRequestTypeDef = TypedDict(
     "GetTypedLinkFacetInformationRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
-    "GetTypedLinkFacetInformationResponseTypeDef",
-    {
-        "IdentityAttributeOrder": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-    },
-)
-_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
-    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
-    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppliedSchemaArnsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
     },
 )
 _OptionalListAppliedSchemaArnsRequestRequestTypeDef = TypedDict(
@@ -736,95 +621,41 @@
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAppliedSchemaArnsRequestRequestTypeDef(
     _RequiredListAppliedSchemaArnsRequestRequestTypeDef,
     _OptionalListAppliedSchemaArnsRequestRequestTypeDef,
 ):
     pass
 
-ListAppliedSchemaArnsResponseTypeDef = TypedDict(
-    "ListAppliedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDevelopmentSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListDevelopmentSchemaArnsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
-    "ListDevelopmentSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
-    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
-    {
-        "state": DirectoryStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDirectoriesRequestRequestTypeDef = TypedDict(
     "ListDirectoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "state": DirectoryStateType,
     },
     total=False,
 )
 
-_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
-    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -833,39 +664,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListFacetAttributesRequestRequestTypeDef(
     _RequiredListFacetAttributesRequestRequestTypeDef,
     _OptionalListFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
-    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
-    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
-):
-    pass
 
 _RequiredListFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
@@ -874,131 +687,41 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListFacetNamesRequestRequestTypeDef(
     _RequiredListFacetNamesRequestRequestTypeDef, _OptionalListFacetNamesRequestRequestTypeDef
 ):
     pass
 
-ListFacetNamesResponseTypeDef = TypedDict(
-    "ListFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListManagedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListManagedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListManagedSchemaArnsResponseTypeDef = TypedDict(
-    "ListManagedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectChildrenResponseTypeDef = TypedDict(
-    "ListObjectChildrenResponseTypeDef",
-    {
-        "Children": Dict[str, str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListObjectPoliciesResponseTypeDef = TypedDict(
-    "ListObjectPoliciesResponseTypeDef",
-    {
-        "AttachedPolicyIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPolicyAttachmentsResponseTypeDef = TypedDict(
-    "ListPolicyAttachmentsResponseTypeDef",
-    {
-        "ObjectIdentifiers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
-    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPublishedSchemaArnsRequestRequestTypeDef = TypedDict(
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListPublishedSchemaArnsResponseTypeDef = TypedDict(
-    "ListPublishedSchemaArnsResponseTypeDef",
-    {
-        "SchemaArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1006,50 +729,31 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
-    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetAttributesRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -1058,39 +762,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTypedLinkFacetAttributesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetAttributesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetAttributesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "SchemaArn": str,
-    },
-)
-_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
-    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
-    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
-):
-    pass
 
 _RequiredListTypedLinkFacetNamesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypedLinkFacetNamesRequestRequestTypeDef",
     {
         "SchemaArn": str,
     },
 )
@@ -1099,38 +785,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTypedLinkFacetNamesRequestRequestTypeDef(
     _RequiredListTypedLinkFacetNamesRequestRequestTypeDef,
     _OptionalListTypedLinkFacetNamesRequestRequestTypeDef,
 ):
     pass
 
-ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetNamesResponseTypeDef",
-    {
-        "FacetNames": List[str],
-        "NextToken": str,
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
 
 PolicyAttachmentTypeDef = TypedDict(
     "PolicyAttachmentTypeDef",
     {
         "PolicyId": str,
         "ObjectIdentifier": str,
         "PolicyType": str,
@@ -1150,86 +819,46 @@
     {
         "MinorVersion": str,
         "Name": str,
     },
     total=False,
 )
 
+
 class PublishSchemaRequestRequestTypeDef(
     _RequiredPublishSchemaRequestRequestTypeDef, _OptionalPublishSchemaRequestRequestTypeDef
 ):
     pass
 
-PublishSchemaResponseTypeDef = TypedDict(
-    "PublishSchemaResponseTypeDef",
-    {
-        "PublishedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PutSchemaFromJsonRequestRequestTypeDef = TypedDict(
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
-PutSchemaFromJsonResponseTypeDef = TypedDict(
-    "PutSchemaFromJsonResponseTypeDef",
-    {
-        "Arn": str,
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
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateObjectAttributesResponseTypeDef = TypedDict(
-    "UpdateObjectAttributesResponseTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSchemaRequestRequestTypeDef = TypedDict(
     "UpdateSchemaRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 
-UpdateSchemaResponseTypeDef = TypedDict(
-    "UpdateSchemaResponseTypeDef",
-    {
-        "SchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpgradeAppliedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "PublishedSchemaArn": str,
         "DirectoryArn": str,
     },
 )
@@ -1237,28 +866,21 @@
     "_OptionalUpgradeAppliedSchemaRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class UpgradeAppliedSchemaRequestRequestTypeDef(
     _RequiredUpgradeAppliedSchemaRequestRequestTypeDef,
     _OptionalUpgradeAppliedSchemaRequestRequestTypeDef,
 ):
     pass
 
-UpgradeAppliedSchemaResponseTypeDef = TypedDict(
-    "UpgradeAppliedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "DirectoryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpgradePublishedSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DevelopmentSchemaArn": str,
         "PublishedSchemaArn": str,
         "MinorVersion": str,
@@ -1268,27 +890,21 @@
     "_OptionalUpgradePublishedSchemaRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class UpgradePublishedSchemaRequestRequestTypeDef(
     _RequiredUpgradePublishedSchemaRequestRequestTypeDef,
     _OptionalUpgradePublishedSchemaRequestRequestTypeDef,
 ):
     pass
 
-UpgradePublishedSchemaResponseTypeDef = TypedDict(
-    "UpgradePublishedSchemaResponseTypeDef",
-    {
-        "UpgradedSchemaArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AttachObjectRequestRequestTypeDef = TypedDict(
     "AttachObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ParentReference": ObjectReferenceTypeDef,
         "ChildReference": ObjectReferenceTypeDef,
@@ -1365,19 +981,21 @@
     "_OptionalBatchDetachObjectTypeDef",
     {
         "BatchReferenceName": str,
     },
     total=False,
 )
 
+
 class BatchDetachObjectTypeDef(
     _RequiredBatchDetachObjectTypeDef, _OptionalBatchDetachObjectTypeDef
 ):
     pass
 
+
 BatchDetachPolicyTypeDef = TypedDict(
     "BatchDetachPolicyTypeDef",
     {
         "PolicyReference": ObjectReferenceTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1400,19 +1018,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListAttachedIndicesTypeDef(
     _RequiredBatchListAttachedIndicesTypeDef, _OptionalBatchListAttachedIndicesTypeDef
 ):
     pass
 
+
 _RequiredBatchListObjectChildrenTypeDef = TypedDict(
     "_RequiredBatchListObjectChildrenTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectChildrenTypeDef = TypedDict(
@@ -1420,19 +1040,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListObjectChildrenTypeDef(
     _RequiredBatchListObjectChildrenTypeDef, _OptionalBatchListObjectChildrenTypeDef
 ):
     pass
 
+
 _RequiredBatchListObjectParentPathsTypeDef = TypedDict(
     "_RequiredBatchListObjectParentPathsTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectParentPathsTypeDef = TypedDict(
@@ -1440,19 +1062,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListObjectParentPathsTypeDef(
     _RequiredBatchListObjectParentPathsTypeDef, _OptionalBatchListObjectParentPathsTypeDef
 ):
     pass
 
+
 _RequiredBatchListObjectParentsTypeDef = TypedDict(
     "_RequiredBatchListObjectParentsTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectParentsTypeDef = TypedDict(
@@ -1460,19 +1084,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListObjectParentsTypeDef(
     _RequiredBatchListObjectParentsTypeDef, _OptionalBatchListObjectParentsTypeDef
 ):
     pass
 
+
 _RequiredBatchListObjectPoliciesTypeDef = TypedDict(
     "_RequiredBatchListObjectPoliciesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectPoliciesTypeDef = TypedDict(
@@ -1480,19 +1106,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListObjectPoliciesTypeDef(
     _RequiredBatchListObjectPoliciesTypeDef, _OptionalBatchListObjectPoliciesTypeDef
 ):
     pass
 
+
 _RequiredBatchListPolicyAttachmentsTypeDef = TypedDict(
     "_RequiredBatchListPolicyAttachmentsTypeDef",
     {
         "PolicyReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListPolicyAttachmentsTypeDef = TypedDict(
@@ -1500,19 +1128,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListPolicyAttachmentsTypeDef(
     _RequiredBatchListPolicyAttachmentsTypeDef, _OptionalBatchListPolicyAttachmentsTypeDef
 ):
     pass
 
+
 _RequiredBatchLookupPolicyTypeDef = TypedDict(
     "_RequiredBatchLookupPolicyTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchLookupPolicyTypeDef = TypedDict(
@@ -1520,19 +1150,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchLookupPolicyTypeDef(
     _RequiredBatchLookupPolicyTypeDef, _OptionalBatchLookupPolicyTypeDef
 ):
     pass
 
+
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1575,41 +1207,21 @@
     "_OptionalGetObjectInformationRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class GetObjectInformationRequestRequestTypeDef(
     _RequiredGetObjectInformationRequestRequestTypeDef,
     _OptionalGetObjectInformationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "TargetReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
-    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
-):
-    pass
 
 _RequiredListAttachedIndicesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedIndicesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TargetReference": ObjectReferenceTypeDef,
     },
@@ -1620,20 +1232,22 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListAttachedIndicesRequestRequestTypeDef(
     _RequiredListAttachedIndicesRequestRequestTypeDef,
     _OptionalListAttachedIndicesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListObjectChildrenRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectChildrenRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1643,40 +1257,21 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListObjectChildrenRequestRequestTypeDef(
     _RequiredListObjectChildrenRequestRequestTypeDef,
     _OptionalListObjectChildrenRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
-    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
-    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
-):
-    pass
 
 _RequiredListObjectParentPathsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentPathsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
@@ -1686,20 +1281,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListObjectParentPathsRequestRequestTypeDef(
     _RequiredListObjectParentPathsRequestRequestTypeDef,
     _OptionalListObjectParentPathsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListObjectParentsRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectParentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1710,40 +1307,20 @@
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
         "IncludeAllLinksToEachParent": bool,
     },
     total=False,
 )
 
+
 class ListObjectParentsRequestRequestTypeDef(
     _RequiredListObjectParentsRequestRequestTypeDef, _OptionalListObjectParentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
-    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
-):
-    pass
 
 _RequiredListObjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectPoliciesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
@@ -1754,41 +1331,21 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListObjectPoliciesRequestRequestTypeDef(
     _RequiredListObjectPoliciesRequestRequestTypeDef,
     _OptionalListObjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "PolicyReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
-    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
-):
-    pass
 
 _RequiredListPolicyAttachmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyAttachmentsRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "PolicyReference": ObjectReferenceTypeDef,
     },
@@ -1799,40 +1356,21 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListPolicyAttachmentsRequestRequestTypeDef(
     _RequiredListPolicyAttachmentsRequestRequestTypeDef,
     _OptionalListPolicyAttachmentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
-    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class LookupPolicyRequestLookupPolicyPaginateTypeDef(
-    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
-    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
-):
-    pass
 
 _RequiredLookupPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredLookupPolicyRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
@@ -1842,19 +1380,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class LookupPolicyRequestRequestTypeDef(
     _RequiredLookupPolicyRequestRequestTypeDef, _OptionalLookupPolicyRequestRequestTypeDef
 ):
     pass
 
+
 BatchGetObjectAttributesTypeDef = TypedDict(
     "BatchGetObjectAttributesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
         "SchemaFacet": SchemaFacetTypeDef,
         "AttributeNames": Sequence[str],
     },
@@ -1881,19 +1421,21 @@
         "NextToken": str,
         "MaxResults": int,
         "FacetFilter": SchemaFacetTypeDef,
     },
     total=False,
 )
 
+
 class BatchListObjectAttributesTypeDef(
     _RequiredBatchListObjectAttributesTypeDef, _OptionalBatchListObjectAttributesTypeDef
 ):
     pass
 
+
 BatchRemoveFacetFromObjectTypeDef = TypedDict(
     "BatchRemoveFacetFromObjectTypeDef",
     {
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1911,51 +1453,21 @@
     "_OptionalGetObjectAttributesRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "DirectoryArn": str,
-        "ObjectReference": ObjectReferenceTypeDef,
-    },
-)
-_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
-    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
-    {
-        "ConsistencyLevel": ConsistencyLevelType,
-        "FacetFilter": SchemaFacetTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
-    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
-):
-    pass
 
 _RequiredListObjectAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredListObjectAttributesRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
@@ -1967,29 +1479,310 @@
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
         "FacetFilter": SchemaFacetTypeDef,
     },
     total=False,
 )
 
+
 class ListObjectAttributesRequestRequestTypeDef(
     _RequiredListObjectAttributesRequestRequestTypeDef,
     _OptionalListObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 RemoveFacetFromObjectRequestRequestTypeDef = TypedDict(
     "RemoveFacetFromObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
+ApplySchemaResponseTypeDef = TypedDict(
+    "ApplySchemaResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachObjectResponseTypeDef = TypedDict(
+    "AttachObjectResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachToIndexResponseTypeDef = TypedDict(
+    "AttachToIndexResponseTypeDef",
+    {
+        "AttachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResponseTypeDef = TypedDict(
+    "CreateDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "Name": str,
+        "ObjectIdentifier": str,
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexResponseTypeDef = TypedDict(
+    "CreateIndexResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateObjectResponseTypeDef = TypedDict(
+    "CreateObjectResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResponseTypeDef = TypedDict(
+    "DeleteDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSchemaResponseTypeDef = TypedDict(
+    "DeleteSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachFromIndexResponseTypeDef = TypedDict(
+    "DetachFromIndexResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachObjectResponseTypeDef = TypedDict(
+    "DetachObjectResponseTypeDef",
+    {
+        "DetachedObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDirectoryResponseTypeDef = TypedDict(
+    "DisableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
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
+EnableDirectoryResponseTypeDef = TypedDict(
+    "EnableDirectoryResponseTypeDef",
+    {
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppliedSchemaVersionResponseTypeDef = TypedDict(
+    "GetAppliedSchemaVersionResponseTypeDef",
+    {
+        "AppliedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSchemaAsJsonResponseTypeDef = TypedDict(
+    "GetSchemaAsJsonResponseTypeDef",
+    {
+        "Name": str,
+        "Document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTypedLinkFacetInformationResponseTypeDef = TypedDict(
+    "GetTypedLinkFacetInformationResponseTypeDef",
+    {
+        "IdentityAttributeOrder": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppliedSchemaArnsResponseTypeDef = TypedDict(
+    "ListAppliedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDevelopmentSchemaArnsResponseTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFacetNamesResponseTypeDef = TypedDict(
+    "ListFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedSchemaArnsResponseTypeDef = TypedDict(
+    "ListManagedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectChildrenResponseTypeDef = TypedDict(
+    "ListObjectChildrenResponseTypeDef",
+    {
+        "Children": Dict[str, str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectPoliciesResponseTypeDef = TypedDict(
+    "ListObjectPoliciesResponseTypeDef",
+    {
+        "AttachedPolicyIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyAttachmentsResponseTypeDef = TypedDict(
+    "ListPolicyAttachmentsResponseTypeDef",
+    {
+        "ObjectIdentifiers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPublishedSchemaArnsResponseTypeDef = TypedDict(
+    "ListPublishedSchemaArnsResponseTypeDef",
+    {
+        "SchemaArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypedLinkFacetNamesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetNamesResponseTypeDef",
+    {
+        "FacetNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishSchemaResponseTypeDef = TypedDict(
+    "PublishSchemaResponseTypeDef",
+    {
+        "PublishedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaFromJsonResponseTypeDef = TypedDict(
+    "PutSchemaFromJsonResponseTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateObjectAttributesResponseTypeDef = TypedDict(
+    "UpdateObjectAttributesResponseTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSchemaResponseTypeDef = TypedDict(
+    "UpdateSchemaResponseTypeDef",
+    {
+        "SchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradeAppliedSchemaResponseTypeDef = TypedDict(
+    "UpgradeAppliedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "DirectoryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpgradePublishedSchemaResponseTypeDef = TypedDict(
+    "UpgradePublishedSchemaResponseTypeDef",
+    {
+        "UpgradedSchemaArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
         "IsUnique": bool,
     },
 )
@@ -1999,17 +1792,19 @@
         "ParentReference": ObjectReferenceTypeDef,
         "LinkName": str,
         "BatchReferenceName": str,
     },
     total=False,
 )
 
+
 class BatchCreateIndexTypeDef(_RequiredBatchCreateIndexTypeDef, _OptionalBatchCreateIndexTypeDef):
     pass
 
+
 _RequiredCreateIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIndexRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
         "IsUnique": bool,
     },
@@ -2019,73 +1814,36 @@
     {
         "ParentReference": ObjectReferenceTypeDef,
         "LinkName": str,
     },
     total=False,
 )
 
+
 class CreateIndexRequestRequestTypeDef(
     _RequiredCreateIndexRequestRequestTypeDef, _OptionalCreateIndexRequestRequestTypeDef
 ):
     pass
 
-AttributeKeyAndValueTypeDef = TypedDict(
-    "AttributeKeyAndValueTypeDef",
+
+AttributeKeyAndValueOutputTypeDef = TypedDict(
+    "AttributeKeyAndValueOutputTypeDef",
     {
         "Key": AttributeKeyTypeDef,
-        "Value": TypedAttributeValueTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
     },
 )
 
-AttributeNameAndValueTypeDef = TypedDict(
-    "AttributeNameAndValueTypeDef",
+AttributeNameAndValueOutputTypeDef = TypedDict(
+    "AttributeNameAndValueOutputTypeDef",
     {
         "AttributeName": str,
-        "Value": TypedAttributeValueTypeDef,
-    },
-)
-
-LinkAttributeActionTypeDef = TypedDict(
-    "LinkAttributeActionTypeDef",
-    {
-        "AttributeActionType": UpdateActionTypeType,
-        "AttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-ObjectAttributeActionTypeDef = TypedDict(
-    "ObjectAttributeActionTypeDef",
-    {
-        "ObjectAttributeActionType": UpdateActionTypeType,
-        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
-    "_RequiredTypedAttributeValueRangeTypeDef",
-    {
-        "StartMode": RangeModeType,
-        "EndMode": RangeModeType,
+        "Value": TypedAttributeValueOutputTypeDef,
     },
 )
-_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
-    "_OptionalTypedAttributeValueRangeTypeDef",
-    {
-        "StartValue": TypedAttributeValueTypeDef,
-        "EndValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-class TypedAttributeValueRangeTypeDef(
-    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
-):
-    pass
 
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
@@ -2093,15 +1851,15 @@
 )
 
 ListObjectParentPathsResponseTypeDef = TypedDict(
     "ListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchListObjectParentsResponseTypeDef = TypedDict(
     "BatchListObjectParentsResponseTypeDef",
     {
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
@@ -2112,257 +1870,803 @@
 
 ListObjectParentsResponseTypeDef = TypedDict(
     "ListObjectParentsResponseTypeDef",
     {
         "Parents": Dict[str, str],
         "NextToken": str,
         "ParentLinks": List[ObjectIdentifierAndLinkNameTupleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDirectoryResponseTypeDef = TypedDict(
     "GetDirectoryResponseTypeDef",
     {
         "Directory": DirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDirectoriesResponseTypeDef = TypedDict(
     "ListDirectoriesResponseTypeDef",
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredFacetAttributeDefinitionTypeDef",
+_RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionOutputTypeDef",
     {
         "Type": FacetAttributeTypeType,
     },
 )
-_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalFacetAttributeDefinitionTypeDef",
+_OptionalFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionOutputTypeDef",
     {
-        "DefaultValue": TypedAttributeValueTypeDef,
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
         "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
+        "Rules": Dict[str, RuleOutputTypeDef],
     },
     total=False,
 )
 
-class FacetAttributeDefinitionTypeDef(
-    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
+
+class FacetAttributeDefinitionOutputTypeDef(
+    _RequiredFacetAttributeDefinitionOutputTypeDef, _OptionalFacetAttributeDefinitionOutputTypeDef
 ):
     pass
 
-_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeDefinitionTypeDef",
+
+_RequiredTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionOutputTypeDef",
     {
         "Name": str,
         "Type": FacetAttributeTypeType,
         "RequiredBehavior": RequiredAttributeBehaviorType,
     },
 )
-_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeDefinitionTypeDef",
+_OptionalTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionOutputTypeDef",
     {
-        "DefaultValue": TypedAttributeValueTypeDef,
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
         "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
+        "Rules": Dict[str, RuleOutputTypeDef],
     },
     total=False,
 )
 
-class TypedLinkAttributeDefinitionTypeDef(
-    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
+
+class TypedLinkAttributeDefinitionOutputTypeDef(
+    _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
+    _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
 ):
     pass
 
+
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryArn": str,
     },
 )
+_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef = TypedDict(
+    "_OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+
+class ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef(
+    _RequiredListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    _OptionalListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "DirectoryArn": str,
+        "TargetReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
+    {
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PolicyToPathTypeDef = TypedDict(
-    "PolicyToPathTypeDef",
+
+class ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef(
+    _RequiredListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    _OptionalListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+):
+    pass
+
+
+ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef = TypedDict(
+    "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     {
-        "Path": str,
-        "Policies": List[PolicyAttachmentTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredAddFacetToObjectRequestRequestTypeDef",
+ListDirectoriesRequestListDirectoriesPaginateTypeDef = TypedDict(
+    "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
+    {
+        "state": DirectoryStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFacetAttributesRequestListFacetAttributesPaginateTypeDef(
+    _RequiredListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    _OptionalListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFacetNamesRequestListFacetNamesPaginateTypeDef(
+    _RequiredListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    _OptionalListFacetNamesRequestListFacetNamesPaginateTypeDef,
+):
+    pass
+
+
+ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
         "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalAddFacetToObjectRequestRequestTypeDef",
+_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ConsistencyLevel": ConsistencyLevelType,
+        "FacetFilter": SchemaFacetTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class AddFacetToObjectRequestRequestTypeDef(
-    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+
+class ListObjectAttributesRequestListObjectAttributesPaginateTypeDef(
+    _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    _OptionalListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
 ):
     pass
 
-BatchAddFacetToObjectTypeDef = TypedDict(
-    "BatchAddFacetToObjectTypeDef",
+
+_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
     {
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
+_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef = TypedDict(
+    "_OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredBatchCreateObjectTypeDef = TypedDict(
-    "_RequiredBatchCreateObjectTypeDef",
+
+class ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef(
+    _RequiredListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    _OptionalListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     {
-        "SchemaFacet": Sequence[SchemaFacetTypeDef],
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "DirectoryArn": str,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalBatchCreateObjectTypeDef = TypedDict(
-    "_OptionalBatchCreateObjectTypeDef",
+_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     {
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
-        "BatchReferenceName": str,
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class BatchCreateObjectTypeDef(
-    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+
+class ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef(
+    _RequiredListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    _OptionalListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
 ):
     pass
 
-BatchGetLinkAttributesResponseTypeDef = TypedDict(
-    "BatchGetLinkAttributesResponseTypeDef",
+
+_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
+    {
+        "DirectoryArn": str,
+        "PolicyReference": ObjectReferenceTypeDef,
+    },
+)
+_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "ConsistencyLevel": ConsistencyLevelType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-BatchGetObjectAttributesResponseTypeDef = TypedDict(
-    "BatchGetObjectAttributesResponseTypeDef",
+
+class ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef(
+    _RequiredListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    _OptionalListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+):
+    pass
+
+
+ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef = TypedDict(
+    "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "SchemaArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-BatchListObjectAttributesResponseTypeDef = TypedDict(
-    "BatchListObjectAttributesResponseTypeDef",
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "NextToken": str,
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateObjectRequestRequestTypeDef",
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+        "Name": str,
+    },
+)
+_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef(
+    _RequiredListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    _OptionalListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "SchemaArn": str,
+    },
+)
+_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef = TypedDict(
+    "_OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef(
+    _RequiredListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    _OptionalListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef",
     {
         "DirectoryArn": str,
-        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateObjectRequestRequestTypeDef",
+_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef = TypedDict(
+    "_OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef",
     {
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateObjectRequestRequestTypeDef(
-    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+
+class LookupPolicyRequestLookupPolicyPaginateTypeDef(
+    _RequiredLookupPolicyRequestLookupPolicyPaginateTypeDef,
+    _OptionalLookupPolicyRequestLookupPolicyPaginateTypeDef,
 ):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+PolicyToPathTypeDef = TypedDict(
+    "PolicyToPathTypeDef",
+    {
+        "Path": str,
+        "Policies": List[PolicyAttachmentTypeDef],
+    },
+    total=False,
+)
+
+TypedAttributeValueTypeDef = TypedDict(
+    "TypedAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "BooleanValue": bool,
+        "NumberValue": str,
+        "DatetimeValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+BatchGetLinkAttributesResponseTypeDef = TypedDict(
+    "BatchGetLinkAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+    },
+    total=False,
+)
+
+BatchGetObjectAttributesResponseTypeDef = TypedDict(
+    "BatchGetObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+    },
+    total=False,
+)
+
+BatchListObjectAttributesResponseTypeDef = TypedDict(
+    "BatchListObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
 GetLinkAttributesResponseTypeDef = TypedDict(
     "GetLinkAttributesResponseTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetObjectAttributesResponseTypeDef = TypedDict(
     "GetObjectAttributesResponseTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IndexAttachmentTypeDef = TypedDict(
     "IndexAttachmentTypeDef",
     {
-        "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
+        "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
         "ObjectIdentifier": str,
     },
     total=False,
 )
 
 ListObjectAttributesResponseTypeDef = TypedDict(
     "ListObjectAttributesResponseTypeDef",
     {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttachTypedLinkRequestRequestTypeDef = TypedDict(
-    "AttachTypedLinkRequestRequestTypeDef",
+TypedLinkSpecifierOutputTypeDef = TypedDict(
+    "TypedLinkSpecifierOutputTypeDef",
     {
-        "DirectoryArn": str,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
+    },
+)
+
+_RequiredFacetAttributeOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalFacetAttributeOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeOutputTypeDef",
+    {
+        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+    total=False,
+)
+
+
+class FacetAttributeOutputTypeDef(
+    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
+):
+    pass
+
+
+ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchLookupPolicyResponseTypeDef = TypedDict(
+    "BatchLookupPolicyResponseTypeDef",
+    {
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+LookupPolicyResponseTypeDef = TypedDict(
+    "LookupPolicyResponseTypeDef",
+    {
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttributeKeyAndValueTypeDef = TypedDict(
+    "AttributeKeyAndValueTypeDef",
+    {
+        "Key": AttributeKeyTypeDef,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+AttributeNameAndValueTypeDef = TypedDict(
+    "AttributeNameAndValueTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionTypeDef",
+    {
+        "Type": FacetAttributeTypeType,
+    },
+)
+_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
+    },
+    total=False,
+)
+
+
+class FacetAttributeDefinitionTypeDef(
+    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
+):
+    pass
+
+
+LinkAttributeActionTypeDef = TypedDict(
+    "LinkAttributeActionTypeDef",
+    {
+        "AttributeActionType": UpdateActionTypeType,
+        "AttributeUpdateValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+ObjectAttributeActionTypeDef = TypedDict(
+    "ObjectAttributeActionTypeDef",
+    {
+        "ObjectAttributeActionType": UpdateActionTypeType,
+        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
+    "_RequiredTypedAttributeValueRangeTypeDef",
+    {
+        "StartMode": RangeModeType,
+        "EndMode": RangeModeType,
+    },
+)
+_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
+    "_OptionalTypedAttributeValueRangeTypeDef",
+    {
+        "StartValue": TypedAttributeValueTypeDef,
+        "EndValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+
+class TypedAttributeValueRangeTypeDef(
+    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
+):
+    pass
+
+
+_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionTypeDef",
+    {
+        "Name": str,
+        "Type": FacetAttributeTypeType,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+)
+_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
+    },
+    total=False,
+)
+
+
+class TypedLinkAttributeDefinitionTypeDef(
+    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
+):
+    pass
+
+
+BatchListAttachedIndicesResponseTypeDef = TypedDict(
+    "BatchListAttachedIndicesResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+BatchListIndexResponseTypeDef = TypedDict(
+    "BatchListIndexResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListAttachedIndicesResponseTypeDef = TypedDict(
+    "ListAttachedIndicesResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListIndexResponseTypeDef = TypedDict(
+    "ListIndexResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachTypedLinkResponseTypeDef = TypedDict(
+    "AttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchAttachTypedLinkResponseTypeDef = TypedDict(
+    "BatchAttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+    },
+    total=False,
+)
+
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttributeKeyAndValueUnionTypeDef = Union[
+    AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef
+]
+BatchAddFacetToObjectTypeDef = TypedDict(
+    "BatchAddFacetToObjectTypeDef",
+    {
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
+    },
+)
+
+_RequiredBatchCreateObjectTypeDef = TypedDict(
+    "_RequiredBatchCreateObjectTypeDef",
+    {
+        "SchemaFacet": Sequence[SchemaFacetTypeDef],
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+    },
+)
+_OptionalBatchCreateObjectTypeDef = TypedDict(
+    "_OptionalBatchCreateObjectTypeDef",
+    {
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+        "BatchReferenceName": str,
+    },
+    total=False,
+)
+
+
+class BatchCreateObjectTypeDef(
+    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+):
+    pass
+
+
+AttributeNameAndValueUnionTypeDef = Union[
+    AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef
+]
 BatchAttachTypedLinkTypeDef = TypedDict(
     "BatchAttachTypedLinkTypeDef",
     {
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "Attributes": Sequence[AttributeNameAndValueTypeDef],
@@ -2371,18 +2675,39 @@
 
 TypedLinkSpecifierTypeDef = TypedDict(
     "TypedLinkSpecifierTypeDef",
     {
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": List[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
     },
 )
 
+_RequiredFacetAttributeTypeDef = TypedDict(
+    "_RequiredFacetAttributeTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalFacetAttributeTypeDef = TypedDict(
+    "_OptionalFacetAttributeTypeDef",
+    {
+        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+    total=False,
+)
+
+
+class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
+    pass
+
+
 LinkAttributeUpdateTypeDef = TypedDict(
     "LinkAttributeUpdateTypeDef",
     {
         "AttributeKey": AttributeKeyTypeDef,
         "AttributeAction": LinkAttributeActionTypeDef,
     },
     total=False,
@@ -2416,46 +2741,20 @@
     "_OptionalTypedLinkAttributeRangeTypeDef",
     {
         "AttributeName": str,
     },
     total=False,
 )
 
+
 class TypedLinkAttributeRangeTypeDef(
     _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
 ):
     pass
 
-_RequiredFacetAttributeTypeDef = TypedDict(
-    "_RequiredFacetAttributeTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalFacetAttributeTypeDef = TypedDict(
-    "_OptionalFacetAttributeTypeDef",
-    {
-        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-    total=False,
-)
-
-class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
-    pass
-
-ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetAttributesResponseTypeDef",
-    {
-        "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
         "Action": UpdateActionTypeType,
     },
@@ -2466,82 +2765,113 @@
     {
         "Name": str,
         "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
         "IdentityAttributeOrder": Sequence[str],
     },
 )
 
-BatchLookupPolicyResponseTypeDef = TypedDict(
-    "BatchLookupPolicyResponseTypeDef",
+BatchWriteOperationResponseTypeDef = TypedDict(
+    "BatchWriteOperationResponseTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
+        "CreateObject": BatchCreateObjectResponseTypeDef,
+        "AttachObject": BatchAttachObjectResponseTypeDef,
+        "DetachObject": BatchDetachObjectResponseTypeDef,
+        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
+        "DeleteObject": Dict[str, Any],
+        "AddFacetToObject": Dict[str, Any],
+        "RemoveFacetFromObject": Dict[str, Any],
+        "AttachPolicy": Dict[str, Any],
+        "DetachPolicy": Dict[str, Any],
+        "CreateIndex": BatchCreateIndexResponseTypeDef,
+        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
+        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
+        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
+        "DetachTypedLink": Dict[str, Any],
+        "UpdateLinkAttributes": Dict[str, Any],
     },
     total=False,
 )
 
-LookupPolicyResponseTypeDef = TypedDict(
-    "LookupPolicyResponseTypeDef",
+BatchReadSuccessfulResponseTypeDef = TypedDict(
+    "BatchReadSuccessfulResponseTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
+        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
+        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
+        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
+        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
+        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
+        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
+        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
+        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
+        "ListIndex": BatchListIndexResponseTypeDef,
+        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
+        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
+        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
+        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
     },
+    total=False,
 )
 
-BatchListAttachedIndicesResponseTypeDef = TypedDict(
-    "BatchListAttachedIndicesResponseTypeDef",
+_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
-    total=False,
 )
-
-BatchListIndexResponseTypeDef = TypedDict(
-    "BatchListIndexResponseTypeDef",
+_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
     },
     total=False,
 )
 
-ListAttachedIndicesResponseTypeDef = TypedDict(
-    "ListAttachedIndicesResponseTypeDef",
-    {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-ListIndexResponseTypeDef = TypedDict(
-    "ListIndexResponseTypeDef",
+class AddFacetToObjectRequestRequestTypeDef(
+    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateObjectRequestRequestTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryArn": str,
+        "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
-
-AttachTypedLinkResponseTypeDef = TypedDict(
-    "AttachTypedLinkResponseTypeDef",
+_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateObjectRequestRequestTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
     },
+    total=False,
 )
 
-BatchAttachTypedLinkResponseTypeDef = TypedDict(
-    "BatchAttachTypedLinkResponseTypeDef",
+
+class CreateObjectRequestRequestTypeDef(
+    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+):
+    pass
+
+
+AttachTypedLinkRequestRequestTypeDef = TypedDict(
+    "AttachTypedLinkRequestRequestTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "DirectoryArn": str,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueUnionTypeDef],
     },
-    total=False,
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
@@ -2551,32 +2881,14 @@
     "BatchGetLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
-    {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
-    {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DetachTypedLinkRequestRequestTypeDef = TypedDict(
     "DetachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
     },
 )
@@ -2593,35 +2905,30 @@
     "_OptionalGetLinkAttributesRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
-    {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
+TypedLinkSpecifierUnionTypeDef = Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
+FacetAttributeUnionTypeDef = Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]
+FacetAttributeUpdateTypeDef = TypedDict(
+    "FacetAttributeUpdateTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Attribute": FacetAttributeTypeDef,
+        "Action": UpdateActionTypeType,
     },
+    total=False,
 )
 
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
@@ -2666,40 +2973,44 @@
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class BatchListIndexTypeDef(_RequiredBatchListIndexTypeDef, _OptionalBatchListIndexTypeDef):
     pass
 
+
 _RequiredListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_RequiredListIndexRequestListIndexPaginateTypeDef",
     {
         "DirectoryArn": str,
         "IndexReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalListIndexRequestListIndexPaginateTypeDef = TypedDict(
     "_OptionalListIndexRequestListIndexPaginateTypeDef",
     {
         "RangesOnIndexedValues": Sequence[ObjectAttributeRangeTypeDef],
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListIndexRequestListIndexPaginateTypeDef(
     _RequiredListIndexRequestListIndexPaginateTypeDef,
     _OptionalListIndexRequestListIndexPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListIndexRequestRequestTypeDef = TypedDict(
     "_RequiredListIndexRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "IndexReference": ObjectReferenceTypeDef,
     },
 )
@@ -2710,19 +3021,21 @@
         "MaxResults": int,
         "NextToken": str,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListIndexRequestRequestTypeDef(
     _RequiredListIndexRequestRequestTypeDef, _OptionalListIndexRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchListIncomingTypedLinksTypeDef = TypedDict(
     "_RequiredBatchListIncomingTypedLinksTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListIncomingTypedLinksTypeDef = TypedDict(
@@ -2732,19 +3045,21 @@
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListIncomingTypedLinksTypeDef(
     _RequiredBatchListIncomingTypedLinksTypeDef, _OptionalBatchListIncomingTypedLinksTypeDef
 ):
     pass
 
+
 _RequiredBatchListOutgoingTypedLinksTypeDef = TypedDict(
     "_RequiredBatchListOutgoingTypedLinksTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListOutgoingTypedLinksTypeDef = TypedDict(
@@ -2754,43 +3069,47 @@
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class BatchListOutgoingTypedLinksTypeDef(
     _RequiredBatchListOutgoingTypedLinksTypeDef, _OptionalBatchListOutgoingTypedLinksTypeDef
 ):
     pass
 
+
 _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef(
     _RequiredListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     _OptionalListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListIncomingTypedLinksRequestRequestTypeDef = TypedDict(
     "_RequiredListIncomingTypedLinksRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2802,44 +3121,48 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListIncomingTypedLinksRequestRequestTypeDef(
     _RequiredListIncomingTypedLinksRequestRequestTypeDef,
     _OptionalListIncomingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef = TypedDict(
     "_OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     {
         "FilterAttributeRanges": Sequence[TypedLinkAttributeRangeTypeDef],
         "FilterTypedLink": TypedLinkSchemaAndFacetNameTypeDef,
         "ConsistencyLevel": ConsistencyLevelType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef(
     _RequiredListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     _OptionalListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListOutgoingTypedLinksRequestRequestTypeDef = TypedDict(
     "_RequiredListOutgoingTypedLinksRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2851,121 +3174,104 @@
         "NextToken": str,
         "MaxResults": int,
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class ListOutgoingTypedLinksRequestRequestTypeDef(
     _RequiredListOutgoingTypedLinksRequestRequestTypeDef,
     _OptionalListOutgoingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFacetRequestRequestTypeDef",
+
+UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
+        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
+        "IdentityAttributeOrder": Sequence[str],
     },
 )
-_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFacetRequestRequestTypeDef",
+
+CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "CreateTypedLinkFacetRequestRequestTypeDef",
     {
-        "Attributes": Sequence[FacetAttributeTypeDef],
-        "ObjectType": ObjectTypeType,
-        "FacetStyle": FacetStyleType,
+        "SchemaArn": str,
+        "Facet": TypedLinkFacetTypeDef,
     },
-    total=False,
 )
 
-class CreateFacetRequestRequestTypeDef(
-    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
-):
-    pass
-
-FacetAttributeUpdateTypeDef = TypedDict(
-    "FacetAttributeUpdateTypeDef",
+BatchWriteResponseTypeDef = TypedDict(
+    "BatchWriteResponseTypeDef",
     {
-        "Attribute": FacetAttributeTypeDef,
-        "Action": UpdateActionTypeType,
+        "Responses": List[BatchWriteOperationResponseTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
+BatchReadOperationResponseTypeDef = TypedDict(
+    "BatchReadOperationResponseTypeDef",
     {
-        "Attributes": List[FacetAttributeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
+        "ExceptionResponse": BatchReadExceptionTypeDef,
     },
+    total=False,
 )
 
-UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "UpdateTypedLinkFacetRequestRequestTypeDef",
+_RequiredCreateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
-        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
-        "IdentityAttributeOrder": Sequence[str],
     },
 )
-
-CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "CreateTypedLinkFacetRequestRequestTypeDef",
+_OptionalCreateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFacetRequestRequestTypeDef",
     {
-        "SchemaArn": str,
-        "Facet": TypedLinkFacetTypeDef,
+        "Attributes": Sequence[FacetAttributeUnionTypeDef],
+        "ObjectType": ObjectTypeType,
+        "FacetStyle": FacetStyleType,
     },
+    total=False,
 )
 
-BatchWriteOperationResponseTypeDef = TypedDict(
-    "BatchWriteOperationResponseTypeDef",
+
+class CreateFacetRequestRequestTypeDef(
+    _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFacetRequestRequestTypeDef",
     {
-        "CreateObject": BatchCreateObjectResponseTypeDef,
-        "AttachObject": BatchAttachObjectResponseTypeDef,
-        "DetachObject": BatchDetachObjectResponseTypeDef,
-        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
-        "DeleteObject": Dict[str, Any],
-        "AddFacetToObject": Dict[str, Any],
-        "RemoveFacetFromObject": Dict[str, Any],
-        "AttachPolicy": Dict[str, Any],
-        "DetachPolicy": Dict[str, Any],
-        "CreateIndex": BatchCreateIndexResponseTypeDef,
-        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
-        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
-        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
-        "DetachTypedLink": Dict[str, Any],
-        "UpdateLinkAttributes": Dict[str, Any],
+        "SchemaArn": str,
+        "Name": str,
     },
-    total=False,
 )
-
-BatchReadSuccessfulResponseTypeDef = TypedDict(
-    "BatchReadSuccessfulResponseTypeDef",
+_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFacetRequestRequestTypeDef",
     {
-        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
-        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
-        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
-        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
-        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
-        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
-        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
-        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
-        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
-        "ListIndex": BatchListIndexResponseTypeDef,
-        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
-        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
-        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
-        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
+        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
+        "ObjectType": ObjectTypeType,
     },
     total=False,
 )
 
+
+class UpdateFacetRequestRequestTypeDef(
+    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
+):
+    pass
+
+
 BatchWriteOperationTypeDef = TypedDict(
     "BatchWriteOperationTypeDef",
     {
         "CreateObject": BatchCreateObjectTypeDef,
         "AttachObject": BatchAttachObjectTypeDef,
         "DetachObject": BatchDetachObjectTypeDef,
         "UpdateObjectAttributes": BatchUpdateObjectAttributesTypeDef,
@@ -3001,50 +3307,20 @@
         "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksTypeDef,
         "ListIncomingTypedLinks": BatchListIncomingTypedLinksTypeDef,
         "GetLinkAttributes": BatchGetLinkAttributesTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFacetRequestRequestTypeDef",
-    {
-        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
-        "ObjectType": ObjectTypeType,
-    },
-    total=False,
-)
-
-class UpdateFacetRequestRequestTypeDef(
-    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
-):
-    pass
-
-BatchWriteResponseTypeDef = TypedDict(
-    "BatchWriteResponseTypeDef",
-    {
-        "Responses": List[BatchWriteOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchReadOperationResponseTypeDef = TypedDict(
-    "BatchReadOperationResponseTypeDef",
+BatchReadResponseTypeDef = TypedDict(
+    "BatchReadResponseTypeDef",
     {
-        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
-        "ExceptionResponse": BatchReadExceptionTypeDef,
+        "Responses": List[BatchReadOperationResponseTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 BatchWriteRequestRequestTypeDef = TypedDict(
     "BatchWriteRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "Operations": Sequence[BatchWriteOperationTypeDef],
@@ -3062,19 +3338,12 @@
     "_OptionalBatchReadRequestRequestTypeDef",
     {
         "ConsistencyLevel": ConsistencyLevelType,
     },
     total=False,
 )
 
+
 class BatchReadRequestRequestTypeDef(
     _RequiredBatchReadRequestRequestTypeDef, _OptionalBatchReadRequestRequestTypeDef
 ):
     pass
-
-BatchReadResponseTypeDef = TypedDict(
-    "BatchReadResponseTypeDef",
-    {
-        "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/PKG-INFO` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-clouddirectory
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudDirectory 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore clouddirectory type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore clouddirectory type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-clouddirectory"></a>
 
 # types-aiobotocore-clouddirectory
 
 [![PyPI - types-aiobotocore-clouddirectory](https://img.shields.io/pypi/v/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-clouddirectory.svg?color=blue)](https://pypi.org/project/types-aiobotocore-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-clouddirectory?color=blue)](https://pypistats.org/packages/types-aiobotocore-clouddirectory)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-clouddirectory)](https://pepy.tech/project/types-aiobotocore-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudDirectory 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [types-aiobotocore-clouddirectory docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_clouddirectory/).
 
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
@@ -401,121 +400,82 @@
 )
 
 
 def check_value(value: BatchReadExceptionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_clouddirectory.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
-    ApplySchemaResponseTypeDef,
-    AttachObjectResponseTypeDef,
-    AttachToIndexResponseTypeDef,
+    ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
-    TypedAttributeValueTypeDef,
+    TypedAttributeValueOutputTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
+    BlobTypeDef,
     CreateDirectoryRequestRequestTypeDef,
-    CreateDirectoryResponseTypeDef,
-    CreateIndexResponseTypeDef,
-    CreateObjectResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResponseTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
-    DeleteSchemaResponseTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
-    DetachFromIndexResponseTypeDef,
-    DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
-    DisableDirectoryResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
-    EnableDirectoryResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
-    GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
-    GetSchemaAsJsonResponseTypeDef,
     GetTypedLinkFacetInformationRequestRequestTypeDef,
-    GetTypedLinkFacetInformationResponseTypeDef,
-    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppliedSchemaArnsRequestRequestTypeDef,
-    ListAppliedSchemaArnsResponseTypeDef,
-    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestRequestTypeDef,
-    ListDevelopmentSchemaArnsResponseTypeDef,
-    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListDirectoriesRequestRequestTypeDef,
-    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetAttributesRequestRequestTypeDef,
-    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
     ListFacetNamesRequestRequestTypeDef,
-    ListFacetNamesResponseTypeDef,
-    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
     ListManagedSchemaArnsRequestRequestTypeDef,
-    ListManagedSchemaArnsResponseTypeDef,
-    ListObjectChildrenResponseTypeDef,
-    ListObjectPoliciesResponseTypeDef,
-    ListPolicyAttachmentsResponseTypeDef,
-    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
-    ListPublishedSchemaArnsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
-    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
-    ListTypedLinkFacetNamesResponseTypeDef,
-    PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
-    PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
-    PutSchemaFromJsonResponseTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
-    UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
-    UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
-    UpgradePublishedSchemaResponseTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
     BatchAttachObjectTypeDef,
     BatchAttachPolicyTypeDef,
     BatchAttachToIndexTypeDef,
     BatchDeleteObjectTypeDef,
@@ -531,124 +491,177 @@
     BatchListPolicyAttachmentsTypeDef,
     BatchLookupPolicyTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DetachFromIndexRequestRequestTypeDef,
     DetachObjectRequestRequestTypeDef,
     DetachPolicyRequestRequestTypeDef,
     GetObjectInformationRequestRequestTypeDef,
-    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListAttachedIndicesRequestRequestTypeDef,
     ListObjectChildrenRequestRequestTypeDef,
-    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
     ListObjectParentPathsRequestRequestTypeDef,
     ListObjectParentsRequestRequestTypeDef,
-    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
-    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
-    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
     BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    GetObjectInformationResponseTypeDef,
-    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
+    ApplySchemaResponseTypeDef,
+    AttachObjectResponseTypeDef,
+    AttachToIndexResponseTypeDef,
+    CreateDirectoryResponseTypeDef,
+    CreateIndexResponseTypeDef,
+    CreateObjectResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DeleteDirectoryResponseTypeDef,
+    DeleteSchemaResponseTypeDef,
+    DetachFromIndexResponseTypeDef,
+    DetachObjectResponseTypeDef,
+    DisableDirectoryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDirectoryResponseTypeDef,
+    GetAppliedSchemaVersionResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
+    GetSchemaAsJsonResponseTypeDef,
+    GetTypedLinkFacetInformationResponseTypeDef,
+    ListAppliedSchemaArnsResponseTypeDef,
+    ListDevelopmentSchemaArnsResponseTypeDef,
+    ListFacetNamesResponseTypeDef,
+    ListManagedSchemaArnsResponseTypeDef,
+    ListObjectChildrenResponseTypeDef,
+    ListObjectPoliciesResponseTypeDef,
+    ListPolicyAttachmentsResponseTypeDef,
+    ListPublishedSchemaArnsResponseTypeDef,
+    ListTypedLinkFacetNamesResponseTypeDef,
+    PublishSchemaResponseTypeDef,
+    PutSchemaFromJsonResponseTypeDef,
+    UpdateObjectAttributesResponseTypeDef,
+    UpdateSchemaResponseTypeDef,
+    UpgradeAppliedSchemaResponseTypeDef,
+    UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
-    AttributeKeyAndValueTypeDef,
-    AttributeNameAndValueTypeDef,
-    LinkAttributeActionTypeDef,
-    ObjectAttributeActionTypeDef,
-    TypedAttributeValueRangeTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
-    FacetAttributeDefinitionTypeDef,
-    TypedLinkAttributeDefinitionTypeDef,
+    FacetAttributeDefinitionOutputTypeDef,
+    TypedLinkAttributeDefinitionOutputTypeDef,
     GetFacetResponseTypeDef,
+    ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
+    ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
+    ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
+    ListDirectoriesRequestListDirectoriesPaginateTypeDef,
+    ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
+    ListFacetNamesRequestListFacetNamesPaginateTypeDef,
+    ListManagedSchemaArnsRequestListManagedSchemaArnsPaginateTypeDef,
+    ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
+    ListObjectParentPathsRequestListObjectParentPathsPaginateTypeDef,
+    ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
+    ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
+    ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
+    ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
+    LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
+    TypedAttributeValueTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
-    CreateObjectRequestRequestTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
-    AttachTypedLinkRequestRequestTypeDef,
-    BatchAttachTypedLinkTypeDef,
-    TypedLinkSpecifierTypeDef,
-    LinkAttributeUpdateTypeDef,
-    ObjectAttributeUpdateTypeDef,
-    ObjectAttributeRangeTypeDef,
-    TypedLinkAttributeRangeTypeDef,
-    FacetAttributeTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
+    FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
-    TypedLinkFacetAttributeUpdateTypeDef,
-    TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
+    AttributeKeyAndValueTypeDef,
+    AttributeNameAndValueTypeDef,
+    FacetAttributeDefinitionTypeDef,
+    LinkAttributeActionTypeDef,
+    ObjectAttributeActionTypeDef,
+    TypedAttributeValueRangeTypeDef,
+    TypedLinkAttributeDefinitionTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
-    BatchDetachTypedLinkTypeDef,
-    BatchGetLinkAttributesTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
-    DetachTypedLinkRequestRequestTypeDef,
-    GetLinkAttributesRequestRequestTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    ListFacetAttributesResponseTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    AttributeNameAndValueUnionTypeDef,
+    BatchAttachTypedLinkTypeDef,
+    TypedLinkSpecifierTypeDef,
+    FacetAttributeTypeDef,
+    LinkAttributeUpdateTypeDef,
+    ObjectAttributeUpdateTypeDef,
+    ObjectAttributeRangeTypeDef,
+    TypedLinkAttributeRangeTypeDef,
+    TypedLinkFacetAttributeUpdateTypeDef,
+    TypedLinkFacetTypeDef,
+    BatchWriteOperationResponseTypeDef,
+    BatchReadSuccessfulResponseTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    CreateObjectRequestRequestTypeDef,
+    AttachTypedLinkRequestRequestTypeDef,
+    BatchDetachTypedLinkTypeDef,
+    BatchGetLinkAttributesTypeDef,
+    DetachTypedLinkRequestRequestTypeDef,
+    GetLinkAttributesRequestRequestTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
+    FacetAttributeUnionTypeDef,
+    FacetAttributeUpdateTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
-    CreateFacetRequestRequestTypeDef,
-    FacetAttributeUpdateTypeDef,
-    ListFacetAttributesResponseTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
-    BatchWriteOperationResponseTypeDef,
-    BatchReadSuccessfulResponseTypeDef,
-    BatchWriteOperationTypeDef,
-    BatchReadOperationTypeDef,
-    UpdateFacetRequestRequestTypeDef,
     BatchWriteResponseTypeDef,
     BatchReadOperationResponseTypeDef,
+    CreateFacetRequestRequestTypeDef,
+    UpdateFacetRequestRequestTypeDef,
+    BatchWriteOperationTypeDef,
+    BatchReadOperationTypeDef,
+    BatchReadResponseTypeDef,
     BatchWriteRequestRequestTypeDef,
     BatchReadRequestRequestTypeDef,
-    BatchReadResponseTypeDef,
 )
 
 
-def get_structure() -> ObjectReferenceTypeDef:
+def get_value() -> ObjectReferenceTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-clouddirectory-2.5.2/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt` & `types-aiobotocore-clouddirectory-2.5.2.post1/types_aiobotocore_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*


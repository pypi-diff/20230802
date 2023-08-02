# Comparing `tmp/types-aiobotocore-omics-2.5.2.tar.gz` & `tmp/types-aiobotocore-omics-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-omics-2.5.2.tar", last modified: Sat Jul  8 01:44:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-omics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:44 2023, max compression
```

## Comparing `types-aiobotocore-omics-2.5.2.tar` & `types-aiobotocore-omics-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:03.842623 types-aiobotocore-omics-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-08 01:44:03.842623 types-aiobotocore-omics-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28155 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:03.842623 types-aiobotocore-omics-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:03.842623 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64784 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    64670 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97569 2023-07-08 01:35:59.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97413 2023-07-08 01:35:58.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:54.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-08 01:35:55.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:03.842623 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-08 01:44:03.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-08 01:44:03.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:03.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:03.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:03.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:44:03.000000 types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.929506 types-aiobotocore-omics-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29782 2023-08-02 14:52:44.925506 types-aiobotocore-omics-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28272 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:44.929506 types-aiobotocore-omics-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.909506 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64693 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64579 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98055 2023-08-02 14:44:17.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97899 2023-08-02 14:44:14.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.925506 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29782 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-omics-2.5.2/LICENSE` & `types-aiobotocore-omics-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/PKG-INFO` & `types-aiobotocore-omics-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-omics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore omics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore omics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-omics"></a>
 
 # types-aiobotocore-omics
 
 [![PyPI - types-aiobotocore-omics](https://img.shields.io/pypi/v/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-omics?color=blue)](https://pypistats.org/packages/types-aiobotocore-omics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Omics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [types-aiobotocore-omics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/).
 
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
@@ -499,172 +498,166 @@
 )
 
 
 def check_value(value: AcceleratorsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_omics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_omics.type_defs import (
     AbortMultipartReadSetUploadRequestRequestTypeDef,
-    ActivateReadSetFilterTypeDef,
+    TimestampTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
     ReferenceItemTypeDef,
     SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    CompleteMultipartReadSetUploadResponseTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
-    CreateMultipartReadSetUploadResponseTypeDef,
     CreateRunGroupRequestRequestTypeDef,
-    CreateRunGroupResponseTypeDef,
     WorkflowParameterTypeDef,
-    CreateWorkflowResponseTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
-    DeleteAnnotationStoreResponseTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
-    DeleteVariantStoreResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportReadSetDetailTypeDef,
-    ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
     GetReadSetMetadataRequestRequestTypeDef,
     SequenceInformationTypeDef,
     GetReadSetRequestRequestTypeDef,
-    GetReadSetResponseTypeDef,
     GetReferenceImportJobRequestRequestTypeDef,
     ImportReferenceSourceItemTypeDef,
     GetReferenceMetadataRequestRequestTypeDef,
     GetReferenceRequestRequestTypeDef,
-    GetReferenceResponseTypeDef,
     GetReferenceStoreRequestRequestTypeDef,
     GetRunGroupRequestRequestTypeDef,
-    GetRunGroupResponseTypeDef,
     GetRunRequestRequestTypeDef,
-    GetRunResponseTypeDef,
     GetRunTaskRequestRequestTypeDef,
-    GetRunTaskResponseTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
     SourceFilesTypeDef,
-    ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
-    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
-    ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
-    ReadSetFilterTypeDef,
-    ReferenceStoreFilterTypeDef,
-    ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
-    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
-    ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
-    SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    PaginatorConfigTypeDef,
     ReadOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    StartAnnotationImportResponseTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
-    StartReadSetActivationJobResponseTypeDef,
-    StartReadSetExportJobResponseTypeDef,
-    StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
-    StartReferenceImportJobResponseTypeDef,
     StartRunRequestRequestTypeDef,
-    StartRunResponseTypeDef,
     VariantImportItemSourceTypeDef,
-    StartVariantImportResponseTypeDef,
+    TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
-    UploadReadSetPartRequestRequestTypeDef,
-    UploadReadSetPartResponseTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    ListReadSetActivationJobsRequestRequestTypeDef,
-    ListReadSetActivationJobsResponseTypeDef,
-    GetReadSetActivationJobResponseTypeDef,
-    ListAnnotationImportJobsResponseTypeDef,
-    CreateVariantStoreResponseTypeDef,
-    UpdateVariantStoreResponseTypeDef,
+    ActivateReadSetFilterTypeDef,
+    ExportReadSetFilterTypeDef,
+    ImportReadSetFilterTypeDef,
+    ImportReferenceFilterTypeDef,
+    ReadSetFilterTypeDef,
+    ReadSetUploadPartListFilterTypeDef,
+    ReferenceFilterTypeDef,
+    ReferenceStoreFilterTypeDef,
+    SequenceStoreFilterTypeDef,
     AnnotationStoreItemTypeDef,
     CreateReferenceStoreRequestRequestTypeDef,
-    CreateReferenceStoreResponseTypeDef,
     CreateSequenceStoreRequestRequestTypeDef,
-    CreateSequenceStoreResponseTypeDef,
     CreateVariantStoreRequestRequestTypeDef,
-    GetReferenceStoreResponseTypeDef,
-    GetSequenceStoreResponseTypeDef,
-    GetVariantStoreResponseTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    CompleteMultipartReadSetUploadResponseTypeDef,
+    CreateMultipartReadSetUploadResponseTypeDef,
+    CreateReferenceStoreResponseTypeDef,
+    CreateRunGroupResponseTypeDef,
+    CreateSequenceStoreResponseTypeDef,
+    CreateVariantStoreResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DeleteAnnotationStoreResponseTypeDef,
+    DeleteVariantStoreResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetReadSetActivationJobResponseTypeDef,
+    GetReadSetResponseTypeDef,
+    GetReferenceResponseTypeDef,
+    GetReferenceStoreResponseTypeDef,
+    GetRunGroupResponseTypeDef,
+    GetRunResponseTypeDef,
+    GetRunTaskResponseTypeDef,
+    GetSequenceStoreResponseTypeDef,
+    GetVariantStoreResponseTypeDef,
+    ListAnnotationImportJobsResponseTypeDef,
+    ListReadSetActivationJobsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartAnnotationImportResponseTypeDef,
+    StartReadSetActivationJobResponseTypeDef,
+    StartReadSetExportJobResponseTypeDef,
+    StartReadSetImportJobResponseTypeDef,
+    StartReferenceImportJobResponseTypeDef,
+    StartRunResponseTypeDef,
+    StartVariantImportResponseTypeDef,
+    UpdateVariantStoreResponseTypeDef,
+    UploadReadSetPartResponseTypeDef,
+    UploadReadSetPartRequestRequestTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef,
@@ -679,73 +672,84 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
-    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
+    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
+    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
+    ListRunTasksRequestListRunTasksPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
-    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
-    ListReadSetsRequestListReadSetsPaginateTypeDef,
-    ListReadSetsRequestRequestTypeDef,
-    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
-    ListReferenceStoresRequestRequestTypeDef,
-    ListReferencesRequestListReferencesPaginateTypeDef,
-    ListReferencesRequestRequestTypeDef,
     ListReferencesResponseTypeDef,
     ListRunGroupsResponseTypeDef,
     ListRunTasksResponseTypeDef,
     ListRunsResponseTypeDef,
-    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
-    ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TsvOptionsTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetActivationJobsRequestRequestTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestRequestTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestRequestTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestRequestTypeDef,
+    ListReadSetsRequestListReadSetsPaginateTypeDef,
+    ListReadSetsRequestRequestTypeDef,
+    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    ListReadSetUploadPartsRequestRequestTypeDef,
+    ListReferencesRequestListReferencesPaginateTypeDef,
+    ListReferencesRequestRequestTypeDef,
+    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
+    ListReferenceStoresRequestRequestTypeDef,
+    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
+    ListSequenceStoresRequestRequestTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
     FormatOptionsTypeDef,
-    CreateAnnotationStoreRequestRequestTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
+    CreateAnnotationStoreRequestRequestTypeDef,
+    StoreOptionsUnionTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
+def get_value() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-omics-2.5.2/README.md` & `types-aiobotocore-omics-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-omics"></a>
 
 # types-aiobotocore-omics
 
 [![PyPI - types-aiobotocore-omics](https://img.shields.io/pypi/v/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-omics?color=blue)](https://pypistats.org/packages/types-aiobotocore-omics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Omics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [types-aiobotocore-omics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/).
 
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
@@ -466,172 +466,166 @@
 )
 
 
 def check_value(value: AcceleratorsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_omics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_omics.type_defs import (
     AbortMultipartReadSetUploadRequestRequestTypeDef,
-    ActivateReadSetFilterTypeDef,
+    TimestampTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
     ReferenceItemTypeDef,
     SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    CompleteMultipartReadSetUploadResponseTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
-    CreateMultipartReadSetUploadResponseTypeDef,
     CreateRunGroupRequestRequestTypeDef,
-    CreateRunGroupResponseTypeDef,
     WorkflowParameterTypeDef,
-    CreateWorkflowResponseTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
-    DeleteAnnotationStoreResponseTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
-    DeleteVariantStoreResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportReadSetDetailTypeDef,
-    ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
     GetReadSetMetadataRequestRequestTypeDef,
     SequenceInformationTypeDef,
     GetReadSetRequestRequestTypeDef,
-    GetReadSetResponseTypeDef,
     GetReferenceImportJobRequestRequestTypeDef,
     ImportReferenceSourceItemTypeDef,
     GetReferenceMetadataRequestRequestTypeDef,
     GetReferenceRequestRequestTypeDef,
-    GetReferenceResponseTypeDef,
     GetReferenceStoreRequestRequestTypeDef,
     GetRunGroupRequestRequestTypeDef,
-    GetRunGroupResponseTypeDef,
     GetRunRequestRequestTypeDef,
-    GetRunResponseTypeDef,
     GetRunTaskRequestRequestTypeDef,
-    GetRunTaskResponseTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
     SourceFilesTypeDef,
-    ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
-    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
-    ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
-    ReadSetFilterTypeDef,
-    ReferenceStoreFilterTypeDef,
-    ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
-    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
-    ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
-    SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    PaginatorConfigTypeDef,
     ReadOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    StartAnnotationImportResponseTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
-    StartReadSetActivationJobResponseTypeDef,
-    StartReadSetExportJobResponseTypeDef,
-    StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
-    StartReferenceImportJobResponseTypeDef,
     StartRunRequestRequestTypeDef,
-    StartRunResponseTypeDef,
     VariantImportItemSourceTypeDef,
-    StartVariantImportResponseTypeDef,
+    TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
-    UploadReadSetPartRequestRequestTypeDef,
-    UploadReadSetPartResponseTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    ListReadSetActivationJobsRequestRequestTypeDef,
-    ListReadSetActivationJobsResponseTypeDef,
-    GetReadSetActivationJobResponseTypeDef,
-    ListAnnotationImportJobsResponseTypeDef,
-    CreateVariantStoreResponseTypeDef,
-    UpdateVariantStoreResponseTypeDef,
+    ActivateReadSetFilterTypeDef,
+    ExportReadSetFilterTypeDef,
+    ImportReadSetFilterTypeDef,
+    ImportReferenceFilterTypeDef,
+    ReadSetFilterTypeDef,
+    ReadSetUploadPartListFilterTypeDef,
+    ReferenceFilterTypeDef,
+    ReferenceStoreFilterTypeDef,
+    SequenceStoreFilterTypeDef,
     AnnotationStoreItemTypeDef,
     CreateReferenceStoreRequestRequestTypeDef,
-    CreateReferenceStoreResponseTypeDef,
     CreateSequenceStoreRequestRequestTypeDef,
-    CreateSequenceStoreResponseTypeDef,
     CreateVariantStoreRequestRequestTypeDef,
-    GetReferenceStoreResponseTypeDef,
-    GetSequenceStoreResponseTypeDef,
-    GetVariantStoreResponseTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    CompleteMultipartReadSetUploadResponseTypeDef,
+    CreateMultipartReadSetUploadResponseTypeDef,
+    CreateReferenceStoreResponseTypeDef,
+    CreateRunGroupResponseTypeDef,
+    CreateSequenceStoreResponseTypeDef,
+    CreateVariantStoreResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DeleteAnnotationStoreResponseTypeDef,
+    DeleteVariantStoreResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetReadSetActivationJobResponseTypeDef,
+    GetReadSetResponseTypeDef,
+    GetReferenceResponseTypeDef,
+    GetReferenceStoreResponseTypeDef,
+    GetRunGroupResponseTypeDef,
+    GetRunResponseTypeDef,
+    GetRunTaskResponseTypeDef,
+    GetSequenceStoreResponseTypeDef,
+    GetVariantStoreResponseTypeDef,
+    ListAnnotationImportJobsResponseTypeDef,
+    ListReadSetActivationJobsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartAnnotationImportResponseTypeDef,
+    StartReadSetActivationJobResponseTypeDef,
+    StartReadSetExportJobResponseTypeDef,
+    StartReadSetImportJobResponseTypeDef,
+    StartReferenceImportJobResponseTypeDef,
+    StartRunResponseTypeDef,
+    StartVariantImportResponseTypeDef,
+    UpdateVariantStoreResponseTypeDef,
+    UploadReadSetPartResponseTypeDef,
+    UploadReadSetPartRequestRequestTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef,
@@ -646,73 +640,84 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
-    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
+    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
+    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
+    ListRunTasksRequestListRunTasksPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
-    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
-    ListReadSetsRequestListReadSetsPaginateTypeDef,
-    ListReadSetsRequestRequestTypeDef,
-    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
-    ListReferenceStoresRequestRequestTypeDef,
-    ListReferencesRequestListReferencesPaginateTypeDef,
-    ListReferencesRequestRequestTypeDef,
     ListReferencesResponseTypeDef,
     ListRunGroupsResponseTypeDef,
     ListRunTasksResponseTypeDef,
     ListRunsResponseTypeDef,
-    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
-    ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TsvOptionsTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetActivationJobsRequestRequestTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestRequestTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestRequestTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestRequestTypeDef,
+    ListReadSetsRequestListReadSetsPaginateTypeDef,
+    ListReadSetsRequestRequestTypeDef,
+    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    ListReadSetUploadPartsRequestRequestTypeDef,
+    ListReferencesRequestListReferencesPaginateTypeDef,
+    ListReferencesRequestRequestTypeDef,
+    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
+    ListReferenceStoresRequestRequestTypeDef,
+    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
+    ListSequenceStoresRequestRequestTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
     FormatOptionsTypeDef,
-    CreateAnnotationStoreRequestRequestTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
+    CreateAnnotationStoreRequestRequestTypeDef,
+    StoreOptionsUnionTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
+def get_value() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-omics-2.5.2/setup.py` & `types-aiobotocore-omics-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-omics",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore omics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore omics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_omics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/"
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/__init__.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/__init__.pyi` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/__main__.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Omics 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Omics 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/client.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("omics") as client:
         client: OmicsClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     FileTypeType,
     ReadSetFileType,
     ReadSetPartSourceType,
     ReferenceFileType,
@@ -53,14 +52,15 @@
     ListVariantStoresPaginator,
     ListWorkflowsPaginator,
 )
 from .type_defs import (
     ActivateReadSetFilterTypeDef,
     AnnotationImportItemSourceTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    BlobTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
     CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
@@ -128,15 +128,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
-    StoreOptionsTypeDef,
+    StoreOptionsUnionTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
 from .waiter import (
@@ -284,15 +284,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsTypeDef = ...
+        storeOptions: StoreOptionsUnionTypeDef = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store)
         """
@@ -388,15 +388,15 @@
     async def create_workflow(
         self,
         *,
         requestId: str,
         name: str = ...,
         description: str = ...,
         engine: WorkflowEngineType = ...,
-        definitionZip: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        definitionZip: BlobTypeDef = ...,
         definitionUri: str = ...,
         main: str = ...,
         parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
         accelerators: Literal["GPU"] = ...
     ) -> CreateWorkflowResponseTypeDef:
@@ -1118,15 +1118,15 @@
     async def upload_read_set_part(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         partNumber: int,
-        payload: Union[str, bytes, IO[Any], StreamingBody]
+        payload: BlobTypeDef
     ) -> UploadReadSetPartResponseTypeDef:
         """
         This operation uploads a specific part of a read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#upload_read_set_part)
         """
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/client.pyi` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("omics") as client:
         client: OmicsClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     FileTypeType,
     ReadSetFileType,
     ReadSetPartSourceType,
     ReferenceFileType,
@@ -53,14 +52,15 @@
     ListVariantStoresPaginator,
     ListWorkflowsPaginator,
 )
 from .type_defs import (
     ActivateReadSetFilterTypeDef,
     AnnotationImportItemSourceTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    BlobTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
     CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
@@ -128,15 +128,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
-    StoreOptionsTypeDef,
+    StoreOptionsUnionTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
 from .waiter import (
@@ -271,15 +271,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsTypeDef = ...
+        storeOptions: StoreOptionsUnionTypeDef = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store)
         """
@@ -369,15 +369,15 @@
     async def create_workflow(
         self,
         *,
         requestId: str,
         name: str = ...,
         description: str = ...,
         engine: WorkflowEngineType = ...,
-        definitionZip: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        definitionZip: BlobTypeDef = ...,
         definitionUri: str = ...,
         main: str = ...,
         parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
         accelerators: Literal["GPU"] = ...
     ) -> CreateWorkflowResponseTypeDef:
@@ -1039,15 +1039,15 @@
     async def upload_read_set_part(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         partNumber: int,
-        payload: Union[str, bytes, IO[Any], StreamingBody]
+        payload: BlobTypeDef
     ) -> UploadReadSetPartResponseTypeDef:
         """
         This operation uploads a specific part of a read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#upload_read_set_part)
         """
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/literals.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/literals.pyi` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/paginator.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnnotationImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationimportjobspaginator)
         """
 
 
@@ -153,30 +153,30 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnnotationStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstorespaginator)
         """
 
 
 class ListMultipartReadSetUploadsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
     """
 
     def paginate(
-        self, *, sequenceStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sequenceStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMultipartReadSetUploadsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
         """
 
 
@@ -187,15 +187,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ActivateReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetActivationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetactivationjobspaginator)
         """
 
 
@@ -206,15 +206,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ExportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetexportjobspaginator)
         """
 
 
@@ -225,15 +225,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ImportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetimportjobspaginator)
         """
 
 
@@ -246,15 +246,15 @@
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         filter: ReadSetUploadPartListFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetUploadPartsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetuploadpartspaginator)
         """
 
 
@@ -265,15 +265,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetspaginator)
         """
 
 
@@ -284,15 +284,15 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ImportReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReferenceImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferenceimportjobspaginator)
         """
 
 
@@ -302,15 +302,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ReferenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReferenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
         """
 
 
@@ -321,30 +321,30 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencespaginator)
         """
 
 
 class ListRunGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
         """
 
 
@@ -355,15 +355,15 @@
     """
 
     def paginate(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listruntaskspaginator)
         """
 
 
@@ -375,15 +375,15 @@
 
     def paginate(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         status: RunStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrunspaginator)
         """
 
 
@@ -393,15 +393,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: SequenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSequenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
         """
 
 
@@ -412,15 +412,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVariantImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantimportjobspaginator)
         """
 
 
@@ -431,15 +431,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVariantStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantstorespaginator)
         """
 
 
@@ -450,13 +450,13 @@
     """
 
     def paginate(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/paginator.pyi` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnnotationImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationimportjobspaginator)
         """
 
 class ListAnnotationStoresPaginator(AioPaginator):
@@ -149,29 +149,29 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnnotationStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listannotationstorespaginator)
         """
 
 class ListMultipartReadSetUploadsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
     """
 
     def paginate(
-        self, *, sequenceStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sequenceStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMultipartReadSetUploadsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listmultipartreadsetuploadspaginator)
         """
 
 class ListReadSetActivationJobsPaginator(AioPaginator):
@@ -181,15 +181,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ActivateReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetActivationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetactivationjobspaginator)
         """
 
 class ListReadSetExportJobsPaginator(AioPaginator):
@@ -199,15 +199,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ExportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetexportjobspaginator)
         """
 
 class ListReadSetImportJobsPaginator(AioPaginator):
@@ -217,15 +217,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ImportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetimportjobspaginator)
         """
 
 class ListReadSetUploadPartsPaginator(AioPaginator):
@@ -237,15 +237,15 @@
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         filter: ReadSetUploadPartListFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetUploadPartsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetuploadpartspaginator)
         """
 
 class ListReadSetsPaginator(AioPaginator):
@@ -255,15 +255,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReadSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreadsetspaginator)
         """
 
 class ListReferenceImportJobsPaginator(AioPaginator):
@@ -273,15 +273,15 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ImportReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReferenceImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferenceimportjobspaginator)
         """
 
 class ListReferenceStoresPaginator(AioPaginator):
@@ -290,15 +290,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ReferenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReferenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencestorespaginator)
         """
 
 class ListReferencesPaginator(AioPaginator):
@@ -308,29 +308,29 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listreferencespaginator)
         """
 
 class ListRunGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrungroupspaginator)
         """
 
 class ListRunTasksPaginator(AioPaginator):
@@ -340,15 +340,15 @@
     """
 
     def paginate(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listruntaskspaginator)
         """
 
 class ListRunsPaginator(AioPaginator):
@@ -359,15 +359,15 @@
 
     def paginate(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         status: RunStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listrunspaginator)
         """
 
 class ListSequenceStoresPaginator(AioPaginator):
@@ -376,15 +376,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: SequenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSequenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listsequencestorespaginator)
         """
 
 class ListVariantImportJobsPaginator(AioPaginator):
@@ -394,15 +394,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVariantImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantimportjobspaginator)
         """
 
 class ListVariantStoresPaginator(AioPaginator):
@@ -412,15 +412,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVariantStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listvariantstorespaginator)
         """
 
 class ListWorkflowsPaginator(AioPaginator):
@@ -430,13 +430,13 @@
     """
 
     def paginate(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/type_defs.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_omics.type_defs import AbortMultipartReadSetUploadRequestRequestTypeDef
 
-    data: AbortMultipartReadSetUploadRequestRequestTypeDef = {...}
+    data: AbortMultipartReadSetUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -54,162 +54,156 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
-    "ActivateReadSetFilterTypeDef",
+    "TimestampTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
     "ReferenceItemTypeDef",
     "SseConfigTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
-    "CompleteMultipartReadSetUploadResponseTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
-    "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
-    "CreateRunGroupResponseTypeDef",
     "WorkflowParameterTypeDef",
-    "CreateWorkflowResponseTypeDef",
     "DeleteAnnotationStoreRequestRequestTypeDef",
-    "DeleteAnnotationStoreResponseTypeDef",
     "DeleteReferenceRequestRequestTypeDef",
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteSequenceStoreRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
-    "DeleteVariantStoreResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportReadSetDetailTypeDef",
-    "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
     "GetReadSetExportJobRequestRequestTypeDef",
     "GetReadSetImportJobRequestRequestTypeDef",
     "GetReadSetMetadataRequestRequestTypeDef",
     "SequenceInformationTypeDef",
     "GetReadSetRequestRequestTypeDef",
-    "GetReadSetResponseTypeDef",
     "GetReferenceImportJobRequestRequestTypeDef",
     "ImportReferenceSourceItemTypeDef",
     "GetReferenceMetadataRequestRequestTypeDef",
     "GetReferenceRequestRequestTypeDef",
-    "GetReferenceResponseTypeDef",
     "GetReferenceStoreRequestRequestTypeDef",
     "GetRunGroupRequestRequestTypeDef",
-    "GetRunGroupResponseTypeDef",
     "GetRunRequestRequestTypeDef",
-    "GetRunResponseTypeDef",
     "GetRunTaskRequestRequestTypeDef",
-    "GetRunTaskResponseTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
-    "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
     "SourceFilesTypeDef",
-    "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
-    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
-    "ReadSetUploadPartListFilterTypeDef",
     "ReadSetUploadPartListItemTypeDef",
-    "ReadSetFilterTypeDef",
-    "ReferenceStoreFilterTypeDef",
-    "ReferenceFilterTypeDef",
     "ReferenceListItemTypeDef",
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     "ListRunGroupsRequestRequestTypeDef",
     "RunGroupListItemTypeDef",
-    "ListRunTasksRequestListRunTasksPaginateTypeDef",
     "ListRunTasksRequestRequestTypeDef",
     "TaskListItemTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
     "RunListItemTypeDef",
-    "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
-    "PaginatorConfigTypeDef",
     "ReadOptionsTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartAnnotationImportResponseTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
-    "StartReadSetActivationJobResponseTypeDef",
-    "StartReadSetExportJobResponseTypeDef",
-    "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
-    "StartReferenceImportJobResponseTypeDef",
     "StartRunRequestRequestTypeDef",
-    "StartRunResponseTypeDef",
     "VariantImportItemSourceTypeDef",
-    "StartVariantImportResponseTypeDef",
+    "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
-    "UploadReadSetPartRequestRequestTypeDef",
-    "UploadReadSetPartResponseTypeDef",
-    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    "ListReadSetActivationJobsRequestRequestTypeDef",
-    "ListReadSetActivationJobsResponseTypeDef",
-    "GetReadSetActivationJobResponseTypeDef",
-    "ListAnnotationImportJobsResponseTypeDef",
-    "CreateVariantStoreResponseTypeDef",
-    "UpdateVariantStoreResponseTypeDef",
+    "ActivateReadSetFilterTypeDef",
+    "ExportReadSetFilterTypeDef",
+    "ImportReadSetFilterTypeDef",
+    "ImportReferenceFilterTypeDef",
+    "ReadSetFilterTypeDef",
+    "ReadSetUploadPartListFilterTypeDef",
+    "ReferenceFilterTypeDef",
+    "ReferenceStoreFilterTypeDef",
+    "SequenceStoreFilterTypeDef",
     "AnnotationStoreItemTypeDef",
     "CreateReferenceStoreRequestRequestTypeDef",
-    "CreateReferenceStoreResponseTypeDef",
     "CreateSequenceStoreRequestRequestTypeDef",
-    "CreateSequenceStoreResponseTypeDef",
     "CreateVariantStoreRequestRequestTypeDef",
-    "GetReferenceStoreResponseTypeDef",
-    "GetSequenceStoreResponseTypeDef",
-    "GetVariantStoreResponseTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
     "BatchDeleteReadSetResponseTypeDef",
+    "CompleteMultipartReadSetUploadResponseTypeDef",
+    "CreateMultipartReadSetUploadResponseTypeDef",
+    "CreateReferenceStoreResponseTypeDef",
+    "CreateRunGroupResponseTypeDef",
+    "CreateSequenceStoreResponseTypeDef",
+    "CreateVariantStoreResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "DeleteAnnotationStoreResponseTypeDef",
+    "DeleteVariantStoreResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetReadSetActivationJobResponseTypeDef",
+    "GetReadSetResponseTypeDef",
+    "GetReferenceResponseTypeDef",
+    "GetReferenceStoreResponseTypeDef",
+    "GetRunGroupResponseTypeDef",
+    "GetRunResponseTypeDef",
+    "GetRunTaskResponseTypeDef",
+    "GetSequenceStoreResponseTypeDef",
+    "GetVariantStoreResponseTypeDef",
+    "ListAnnotationImportJobsResponseTypeDef",
+    "ListReadSetActivationJobsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartAnnotationImportResponseTypeDef",
+    "StartReadSetActivationJobResponseTypeDef",
+    "StartReadSetExportJobResponseTypeDef",
+    "StartReadSetImportJobResponseTypeDef",
+    "StartReferenceImportJobResponseTypeDef",
+    "StartRunResponseTypeDef",
+    "StartVariantImportResponseTypeDef",
+    "UpdateVariantStoreResponseTypeDef",
+    "UploadReadSetPartResponseTypeDef",
+    "UploadReadSetPartRequestRequestTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
-    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef",
@@ -224,89 +218,91 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
     "StartReadSetImportJobSourceItemTypeDef",
-    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
+    "ListRunTasksRequestListRunTasksPaginateTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     "ListAnnotationStoresRequestRequestTypeDef",
     "ListMultipartReadSetUploadsResponseTypeDef",
-    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
-    "ListReadSetUploadPartsRequestRequestTypeDef",
     "ListReadSetUploadPartsResponseTypeDef",
-    "ListReadSetsRequestListReadSetsPaginateTypeDef",
-    "ListReadSetsRequestRequestTypeDef",
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
-    "ListReferenceStoresRequestRequestTypeDef",
-    "ListReferencesRequestListReferencesPaginateTypeDef",
-    "ListReferencesRequestRequestTypeDef",
     "ListReferencesResponseTypeDef",
     "ListRunGroupsResponseTypeDef",
     "ListRunTasksResponseTypeDef",
     "ListRunsResponseTypeDef",
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
-    "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TsvOptionsTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
+    "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
+    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    "ListReadSetActivationJobsRequestRequestTypeDef",
+    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    "ListReadSetExportJobsRequestRequestTypeDef",
+    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "ListReadSetImportJobsRequestRequestTypeDef",
+    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    "ListReferenceImportJobsRequestRequestTypeDef",
+    "ListReadSetsRequestListReadSetsPaginateTypeDef",
+    "ListReadSetsRequestRequestTypeDef",
+    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    "ListReadSetUploadPartsRequestRequestTypeDef",
+    "ListReferencesRequestListReferencesPaginateTypeDef",
+    "ListReferencesRequestRequestTypeDef",
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+    "ListReferenceStoresRequestRequestTypeDef",
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    "ListSequenceStoresRequestRequestTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
-    "CreateAnnotationStoreRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
+    "CreateAnnotationStoreRequestRequestTypeDef",
+    "StoreOptionsUnionTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
     },
 )
 
-ActivateReadSetFilterTypeDef = TypedDict(
-    "ActivateReadSetFilterTypeDef",
-    {
-        "status": ReadSetActivationJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredActivateReadSetJobItemTypeDef = TypedDict(
     "_RequiredActivateReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "status": ReadSetActivationJobStatusType,
         "creationTime": datetime,
@@ -432,14 +428,26 @@
     {
         "id": str,
         "code": str,
         "message": str,
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
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelAnnotationImportRequestRequestTypeDef = TypedDict(
     "CancelAnnotationImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -462,22 +470,14 @@
     {
         "partNumber": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
     },
 )
 
-CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CompleteMultipartReadSetUploadResponseTypeDef",
-    {
-        "readSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sourceFileType": FileTypeType,
         "subjectId": str,
         "sampleId": str,
@@ -500,32 +500,14 @@
 class CreateMultipartReadSetUploadRequestRequestTypeDef(
     _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef,
     _OptionalCreateMultipartReadSetUploadRequestRequestTypeDef,
 ):
     pass
 
 
-CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CreateMultipartReadSetUploadResponseTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "generatedFrom": str,
-        "referenceArn": str,
-        "name": str,
-        "description": str,
-        "tags": Dict[str, str],
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRunGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRunGroupRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateRunGroupRequestRequestTypeDef = TypedDict(
@@ -544,44 +526,23 @@
 
 class CreateRunGroupRequestRequestTypeDef(
     _RequiredCreateRunGroupRequestRequestTypeDef, _OptionalCreateRunGroupRequestRequestTypeDef
 ):
     pass
 
 
-CreateRunGroupResponseTypeDef = TypedDict(
-    "CreateRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowParameterTypeDef = TypedDict(
     "WorkflowParameterTypeDef",
     {
         "description": str,
         "optional": bool,
     },
     total=False,
 )
 
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAnnotationStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
@@ -596,22 +557,14 @@
 class DeleteAnnotationStoreRequestRequestTypeDef(
     _RequiredDeleteAnnotationStoreRequestRequestTypeDef,
     _OptionalDeleteAnnotationStoreRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteAnnotationStoreResponseTypeDef = TypedDict(
-    "DeleteAnnotationStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteReferenceRequestRequestTypeDef = TypedDict(
     "DeleteReferenceRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -662,36 +615,21 @@
 class DeleteVariantStoreRequestRequestTypeDef(
     _RequiredDeleteVariantStoreRequestRequestTypeDef,
     _OptionalDeleteVariantStoreRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteVariantStoreResponseTypeDef = TypedDict(
-    "DeleteVariantStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportReadSetDetailTypeDef = TypedDict(
     "_RequiredExportReadSetDetailTypeDef",
     {
         "id": str,
         "status": ReadSetExportJobItemStatusType,
     },
 )
@@ -706,24 +644,14 @@
 
 class ExportReadSetDetailTypeDef(
     _RequiredExportReadSetDetailTypeDef, _OptionalExportReadSetDetailTypeDef
 ):
     pass
 
 
-ExportReadSetFilterTypeDef = TypedDict(
-    "ExportReadSetFilterTypeDef",
-    {
-        "status": ReadSetExportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredExportReadSetJobDetailTypeDef = TypedDict(
     "_RequiredExportReadSetJobDetailTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
@@ -856,22 +784,14 @@
 
 class GetReadSetRequestRequestTypeDef(
     _RequiredGetReadSetRequestRequestTypeDef, _OptionalGetReadSetRequestRequestTypeDef
 ):
     pass
 
 
-GetReadSetResponseTypeDef = TypedDict(
-    "GetReadSetResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceImportJobRequestRequestTypeDef = TypedDict(
     "GetReferenceImportJobRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -929,52 +849,28 @@
 
 class GetReferenceRequestRequestTypeDef(
     _RequiredGetReferenceRequestRequestTypeDef, _OptionalGetReferenceRequestRequestTypeDef
 ):
     pass
 
 
-GetReferenceResponseTypeDef = TypedDict(
-    "GetReferenceResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceStoreRequestRequestTypeDef = TypedDict(
     "GetReferenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
 GetRunGroupRequestRequestTypeDef = TypedDict(
     "GetRunGroupRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetRunGroupResponseTypeDef = TypedDict(
-    "GetRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "maxCpus": int,
-        "maxRuns": int,
-        "maxDuration": int,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "maxGpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRunRequestRequestTypeDef = TypedDict(
     "_RequiredGetRunRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetRunRequestRequestTypeDef = TypedDict(
@@ -988,71 +884,22 @@
 
 class GetRunRequestRequestTypeDef(
     _RequiredGetRunRequestRequestTypeDef, _OptionalGetRunRequestRequestTypeDef
 ):
     pass
 
 
-GetRunResponseTypeDef = TypedDict(
-    "GetRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "workflowId": str,
-        "workflowType": WorkflowTypeType,
-        "runId": str,
-        "roleArn": str,
-        "name": str,
-        "runGroupId": str,
-        "priority": int,
-        "definition": str,
-        "digest": str,
-        "parameters": Dict[str, Any],
-        "storageCapacity": int,
-        "outputUri": str,
-        "logLevel": RunLogLevelType,
-        "resourceDigests": Dict[str, str],
-        "startedBy": str,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRunTaskRequestRequestTypeDef = TypedDict(
     "GetRunTaskRequestRequestTypeDef",
     {
         "id": str,
         "taskId": str,
     },
 )
 
-GetRunTaskResponseTypeDef = TypedDict(
-    "GetRunTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "status": TaskStatusType,
-        "name": str,
-        "cpus": int,
-        "memory": int,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "logStream": str,
-        "gpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSequenceStoreRequestRequestTypeDef = TypedDict(
     "GetSequenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1110,24 +957,14 @@
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-ImportReadSetFilterTypeDef = TypedDict(
-    "ImportReadSetFilterTypeDef",
-    {
-        "status": ReadSetImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReadSetJobItemTypeDef = TypedDict(
     "_RequiredImportReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
@@ -1164,24 +1001,14 @@
 )
 
 
 class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
     pass
 
 
-ImportReferenceFilterTypeDef = TypedDict(
-    "ImportReferenceFilterTypeDef",
-    {
-        "status": ReferenceImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReferenceJobItemTypeDef = TypedDict(
     "_RequiredImportReferenceJobItemTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
@@ -1208,44 +1035,32 @@
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
 )
 
-ListAnnotationStoresFilterTypeDef = TypedDict(
-    "ListAnnotationStoresFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StoreStatusType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+ListAnnotationStoresFilterTypeDef = TypedDict(
+    "ListAnnotationStoresFilterTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": StoreStatusType,
     },
     total=False,
 )
 
-
-class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
-    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartReadSetUploadsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
@@ -1291,23 +1106,14 @@
 
 class MultipartReadSetUploadListItemTypeDef(
     _RequiredMultipartReadSetUploadListItemTypeDef, _OptionalMultipartReadSetUploadListItemTypeDef
 ):
     pass
 
 
-ReadSetUploadPartListFilterTypeDef = TypedDict(
-    "ReadSetUploadPartListFilterTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReadSetUploadPartListItemTypeDef = TypedDict(
     "_RequiredReadSetUploadPartListItemTypeDef",
     {
         "partNumber": int,
         "partSize": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
@@ -1325,50 +1131,14 @@
 
 class ReadSetUploadPartListItemTypeDef(
     _RequiredReadSetUploadPartListItemTypeDef, _OptionalReadSetUploadPartListItemTypeDef
 ):
     pass
 
 
-ReadSetFilterTypeDef = TypedDict(
-    "ReadSetFilterTypeDef",
-    {
-        "name": str,
-        "status": ReadSetStatusType,
-        "referenceArn": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "sampleId": str,
-        "subjectId": str,
-        "generatedFrom": str,
-    },
-    total=False,
-)
-
-ReferenceStoreFilterTypeDef = TypedDict(
-    "ReferenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-ReferenceFilterTypeDef = TypedDict(
-    "ReferenceFilterTypeDef",
-    {
-        "name": str,
-        "md5": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReferenceListItemTypeDef = TypedDict(
     "_RequiredReferenceListItemTypeDef",
     {
         "id": str,
         "arn": str,
         "referenceStoreId": str,
         "md5": str,
@@ -1389,23 +1159,14 @@
 
 class ReferenceListItemTypeDef(
     _RequiredReferenceListItemTypeDef, _OptionalReferenceListItemTypeDef
 ):
     pass
 
 
-ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunGroupsRequestRequestTypeDef = TypedDict(
     "ListRunGroupsRequestRequestTypeDef",
     {
         "name": str,
         "startingToken": str,
         "maxResults": int,
     },
@@ -1423,37 +1184,14 @@
         "maxDuration": int,
         "creationTime": datetime,
         "maxGpus": int,
     },
     total=False,
 )
 
-_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRunTasksRequestListRunTasksPaginateTypeDef(
-    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
-    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRunTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListRunTasksRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalListRunTasksRequestRequestTypeDef = TypedDict(
@@ -1485,25 +1223,14 @@
         "startTime": datetime,
         "stopTime": datetime,
         "gpus": int,
     },
     total=False,
 )
 
-ListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "ListRunsRequestListRunsPaginateTypeDef",
-    {
-        "name": str,
-        "runGroupId": str,
-        "status": RunStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunsRequestRequestTypeDef = TypedDict(
     "ListRunsRequestRequestTypeDef",
     {
         "name": str,
         "runGroupId": str,
         "startingToken": str,
         "maxResults": int,
@@ -1525,39 +1252,21 @@
         "creationTime": datetime,
         "startTime": datetime,
         "stopTime": datetime,
     },
     total=False,
 )
 
-SequenceStoreFilterTypeDef = TypedDict(
-    "SequenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
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
 ListVariantImportJobsFilterTypeDef = TypedDict(
     "ListVariantImportJobsFilterTypeDef",
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
@@ -1595,24 +1304,14 @@
     "ListVariantStoresFilterTypeDef",
     {
         "status": StoreStatusType,
     },
     total=False,
 )
 
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "type": WorkflowTypeType,
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "type": WorkflowTypeType,
         "name": str,
         "startingToken": str,
         "maxResults": int,
@@ -1631,24 +1330,14 @@
         "digest": str,
         "creationTime": datetime,
         "metadata": Dict[str, str],
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
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
         "sep": str,
         "encoding": str,
         "quote": str,
         "quoteAll": bool,
@@ -1657,75 +1346,21 @@
         "comment": str,
         "header": bool,
         "lineSep": str,
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
-StartAnnotationImportResponseTypeDef = TypedDict(
-    "StartAnnotationImportResponseTypeDef",
-    {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartReadSetActivationJobSourceItemTypeDef = TypedDict(
     "StartReadSetActivationJobSourceItemTypeDef",
     {
         "readSetId": str,
     },
 )
 
-StartReadSetActivationJobResponseTypeDef = TypedDict(
-    "StartReadSetActivationJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartReadSetExportJobResponseTypeDef = TypedDict(
-    "StartReadSetExportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "destination": str,
-        "status": ReadSetExportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartReadSetImportJobResponseTypeDef = TypedDict(
-    "StartReadSetImportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "roleArn": str,
-        "status": ReadSetImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartReferenceImportJobSourceItemTypeDef = TypedDict(
     "_RequiredStartReferenceImportJobSourceItemTypeDef",
     {
         "sourceFile": str,
         "name": str,
     },
 )
@@ -1742,26 +1377,14 @@
 class StartReferenceImportJobSourceItemTypeDef(
     _RequiredStartReferenceImportJobSourceItemTypeDef,
     _OptionalStartReferenceImportJobSourceItemTypeDef,
 ):
     pass
 
 
-StartReferenceImportJobResponseTypeDef = TypedDict(
-    "StartReferenceImportJobResponseTypeDef",
-    {
-        "id": str,
-        "referenceStoreId": str,
-        "roleArn": str,
-        "status": ReferenceImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartRunRequestRequestTypeDef",
     {
         "roleArn": str,
         "requestId": str,
     },
 )
@@ -1786,38 +1409,29 @@
 
 class StartRunRequestRequestTypeDef(
     _RequiredStartRunRequestRequestTypeDef, _OptionalStartRunRequestRequestTypeDef
 ):
     pass
 
 
-StartRunResponseTypeDef = TypedDict(
-    "StartRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VariantImportItemSourceTypeDef = TypedDict(
     "VariantImportItemSourceTypeDef",
     {
         "source": str,
     },
 )
 
-StartVariantImportResponseTypeDef = TypedDict(
-    "StartVariantImportResponseTypeDef",
+TsvStoreOptionsOutputTypeDef = TypedDict(
+    "TsvStoreOptionsOutputTypeDef",
     {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "annotationType": AnnotationTypeType,
+        "formatToHeader": Dict[FormatToHeaderKeyType, str],
+        "schema": List[Dict[str, SchemaValueTypeType]],
     },
+    total=False,
 )
 
 TsvStoreOptionsTypeDef = TypedDict(
     "TsvStoreOptionsTypeDef",
     {
         "annotationType": AnnotationTypeType,
         "formatToHeader": Mapping[FormatToHeaderKeyType, str],
@@ -1929,136 +1543,107 @@
 
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-UploadReadSetPartRequestRequestTypeDef = TypedDict(
-    "UploadReadSetPartRequestRequestTypeDef",
+ActivateReadSetFilterTypeDef = TypedDict(
+    "ActivateReadSetFilterTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-        "partNumber": int,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "status": ReadSetActivationJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-UploadReadSetPartResponseTypeDef = TypedDict(
-    "UploadReadSetPartResponseTypeDef",
+ExportReadSetFilterTypeDef = TypedDict(
+    "ExportReadSetFilterTypeDef",
     {
-        "checksum": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": ReadSetExportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+ImportReadSetFilterTypeDef = TypedDict(
+    "ImportReadSetFilterTypeDef",
     {
-        "filter": ActivateReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": ReadSetImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-
-class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
-    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
+ImportReferenceFilterTypeDef = TypedDict(
+    "ImportReferenceFilterTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ActivateReadSetFilterTypeDef,
+        "status": ReferenceImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-
-class ListReadSetActivationJobsRequestRequestTypeDef(
-    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
-    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
-):
-    pass
-
-
-ListReadSetActivationJobsResponseTypeDef = TypedDict(
-    "ListReadSetActivationJobsResponseTypeDef",
+ReadSetFilterTypeDef = TypedDict(
+    "ReadSetFilterTypeDef",
     {
-        "nextToken": str,
-        "activationJobs": List[ActivateReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "status": ReadSetStatusType,
+        "referenceArn": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "sampleId": str,
+        "subjectId": str,
+        "generatedFrom": str,
     },
+    total=False,
 )
 
-GetReadSetActivationJobResponseTypeDef = TypedDict(
-    "GetReadSetActivationJobResponseTypeDef",
+ReadSetUploadPartListFilterTypeDef = TypedDict(
+    "ReadSetUploadPartListFilterTypeDef",
     {
-        "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "statusMessage": str,
-        "creationTime": datetime,
-        "completionTime": datetime,
-        "sources": List[ActivateReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-ListAnnotationImportJobsResponseTypeDef = TypedDict(
-    "ListAnnotationImportJobsResponseTypeDef",
+ReferenceFilterTypeDef = TypedDict(
+    "ReferenceFilterTypeDef",
     {
-        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "md5": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-CreateVariantStoreResponseTypeDef = TypedDict(
-    "CreateVariantStoreResponseTypeDef",
+ReferenceStoreFilterTypeDef = TypedDict(
+    "ReferenceStoreFilterTypeDef",
     {
-        "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
         "name": str,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-UpdateVariantStoreResponseTypeDef = TypedDict(
-    "UpdateVariantStoreResponseTypeDef",
+SequenceStoreFilterTypeDef = TypedDict(
+    "SequenceStoreFilterTypeDef",
     {
-        "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
         "name": str,
-        "description": str,
-        "creationTime": datetime,
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
 AnnotationStoreItemTypeDef = TypedDict(
     "AnnotationStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
@@ -2096,27 +1681,14 @@
 class CreateReferenceStoreRequestRequestTypeDef(
     _RequiredCreateReferenceStoreRequestRequestTypeDef,
     _OptionalCreateReferenceStoreRequestRequestTypeDef,
 ):
     pass
 
 
-CreateReferenceStoreResponseTypeDef = TypedDict(
-    "CreateReferenceStoreResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSequenceStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
@@ -2135,28 +1707,14 @@
 class CreateSequenceStoreRequestRequestTypeDef(
     _RequiredCreateSequenceStoreRequestRequestTypeDef,
     _OptionalCreateSequenceStoreRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSequenceStoreResponseTypeDef = TypedDict(
-    "CreateSequenceStoreResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVariantStoreRequestRequestTypeDef",
     {
         "reference": ReferenceItemTypeDef,
     },
 )
 _OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
@@ -2174,133 +1732,470 @@
 class CreateVariantStoreRequestRequestTypeDef(
     _RequiredCreateVariantStoreRequestRequestTypeDef,
     _OptionalCreateVariantStoreRequestRequestTypeDef,
 ):
     pass
 
 
-GetReferenceStoreResponseTypeDef = TypedDict(
-    "GetReferenceStoreResponseTypeDef",
+_RequiredReferenceStoreDetailTypeDef = TypedDict(
+    "_RequiredReferenceStoreDetailTypeDef",
     {
-        "id": str,
         "arn": str,
+        "id": str,
+        "creationTime": datetime,
+    },
+)
+_OptionalReferenceStoreDetailTypeDef = TypedDict(
+    "_OptionalReferenceStoreDetailTypeDef",
+    {
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-GetSequenceStoreResponseTypeDef = TypedDict(
-    "GetSequenceStoreResponseTypeDef",
+
+class ReferenceStoreDetailTypeDef(
+    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
+):
+    pass
+
+
+_RequiredSequenceStoreDetailTypeDef = TypedDict(
+    "_RequiredSequenceStoreDetailTypeDef",
     {
-        "id": str,
         "arn": str,
+        "id": str,
+        "creationTime": datetime,
+    },
+)
+_OptionalSequenceStoreDetailTypeDef = TypedDict(
+    "_OptionalSequenceStoreDetailTypeDef",
+    {
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
         "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-GetVariantStoreResponseTypeDef = TypedDict(
-    "GetVariantStoreResponseTypeDef",
+
+class SequenceStoreDetailTypeDef(
+    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
+):
+    pass
+
+
+VariantStoreItemTypeDef = TypedDict(
+    "VariantStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
-        "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredReferenceStoreDetailTypeDef = TypedDict(
-    "_RequiredReferenceStoreDetailTypeDef",
+BatchDeleteReadSetResponseTypeDef = TypedDict(
+    "BatchDeleteReadSetResponseTypeDef",
     {
-        "arn": str,
-        "id": str,
+        "errors": List[ReadSetBatchErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CompleteMultipartReadSetUploadResponseTypeDef",
+    {
+        "readSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CreateMultipartReadSetUploadResponseTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "generatedFrom": str,
+        "referenceArn": str,
+        "name": str,
+        "description": str,
+        "tags": Dict[str, str],
         "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalReferenceStoreDetailTypeDef = TypedDict(
-    "_OptionalReferenceStoreDetailTypeDef",
+
+CreateReferenceStoreResponseTypeDef = TypedDict(
+    "CreateReferenceStoreResponseTypeDef",
     {
+        "id": str,
+        "arn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateRunGroupResponseTypeDef = TypedDict(
+    "CreateRunGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ReferenceStoreDetailTypeDef(
-    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
-):
-    pass
+CreateSequenceStoreResponseTypeDef = TypedDict(
+    "CreateSequenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "fallbackLocation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateVariantStoreResponseTypeDef = TypedDict(
+    "CreateVariantStoreResponseTypeDef",
+    {
+        "id": str,
+        "reference": ReferenceItemTypeDef,
+        "status": StoreStatusType,
+        "name": str,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredSequenceStoreDetailTypeDef = TypedDict(
-    "_RequiredSequenceStoreDetailTypeDef",
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
     {
         "arn": str,
         "id": str,
+        "status": WorkflowStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAnnotationStoreResponseTypeDef = TypedDict(
+    "DeleteAnnotationStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVariantStoreResponseTypeDef = TypedDict(
+    "DeleteVariantStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
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
+GetReadSetActivationJobResponseTypeDef = TypedDict(
+    "GetReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "statusMessage": str,
         "creationTime": datetime,
+        "completionTime": datetime,
+        "sources": List[ActivateReadSetSourceItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSequenceStoreDetailTypeDef = TypedDict(
-    "_OptionalSequenceStoreDetailTypeDef",
+
+GetReadSetResponseTypeDef = TypedDict(
+    "GetReadSetResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReferenceResponseTypeDef = TypedDict(
+    "GetReferenceResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReferenceStoreResponseTypeDef = TypedDict(
+    "GetReferenceStoreResponseTypeDef",
     {
+        "id": str,
+        "arn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
-        "fallbackLocation": str,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetRunGroupResponseTypeDef = TypedDict(
+    "GetRunGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "maxCpus": int,
+        "maxRuns": int,
+        "maxDuration": int,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "maxGpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class SequenceStoreDetailTypeDef(
-    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
-):
-    pass
+GetRunResponseTypeDef = TypedDict(
+    "GetRunResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "workflowId": str,
+        "workflowType": WorkflowTypeType,
+        "runId": str,
+        "roleArn": str,
+        "name": str,
+        "runGroupId": str,
+        "priority": int,
+        "definition": str,
+        "digest": str,
+        "parameters": Dict[str, Any],
+        "storageCapacity": int,
+        "outputUri": str,
+        "logLevel": RunLogLevelType,
+        "resourceDigests": Dict[str, str],
+        "startedBy": str,
+        "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunTaskResponseTypeDef = TypedDict(
+    "GetRunTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "status": TaskStatusType,
+        "name": str,
+        "cpus": int,
+        "memory": int,
+        "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "logStream": str,
+        "gpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetSequenceStoreResponseTypeDef = TypedDict(
+    "GetSequenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "fallbackLocation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VariantStoreItemTypeDef = TypedDict(
-    "VariantStoreItemTypeDef",
+GetVariantStoreResponseTypeDef = TypedDict(
+    "GetVariantStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
+        "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeleteReadSetResponseTypeDef = TypedDict(
-    "BatchDeleteReadSetResponseTypeDef",
+ListAnnotationImportJobsResponseTypeDef = TypedDict(
+    "ListAnnotationImportJobsResponseTypeDef",
     {
-        "errors": List[ReadSetBatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReadSetActivationJobsResponseTypeDef = TypedDict(
+    "ListReadSetActivationJobsResponseTypeDef",
+    {
+        "nextToken": str,
+        "activationJobs": List[ActivateReadSetJobItemTypeDef],
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
+StartAnnotationImportResponseTypeDef = TypedDict(
+    "StartAnnotationImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetActivationJobResponseTypeDef = TypedDict(
+    "StartReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetExportJobResponseTypeDef = TypedDict(
+    "StartReadSetExportJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "destination": str,
+        "status": ReadSetExportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetImportJobResponseTypeDef = TypedDict(
+    "StartReadSetImportJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "roleArn": str,
+        "status": ReadSetImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReferenceImportJobResponseTypeDef = TypedDict(
+    "StartReferenceImportJobResponseTypeDef",
+    {
+        "id": str,
+        "referenceStoreId": str,
+        "roleArn": str,
+        "status": ReferenceImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRunResponseTypeDef = TypedDict(
+    "StartRunResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVariantImportResponseTypeDef = TypedDict(
+    "StartVariantImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVariantStoreResponseTypeDef = TypedDict(
+    "UpdateVariantStoreResponseTypeDef",
+    {
+        "id": str,
+        "reference": ReferenceItemTypeDef,
+        "status": StoreStatusType,
+        "name": str,
+        "description": str,
+        "creationTime": datetime,
+        "updateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadReadSetPartResponseTypeDef = TypedDict(
+    "UploadReadSetPartResponseTypeDef",
+    {
+        "checksum": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadReadSetPartRequestRequestTypeDef = TypedDict(
+    "UploadReadSetPartRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+        "partNumber": int,
+        "payload": BlobTypeDef,
     },
 )
 
 CompleteMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -2317,15 +2212,15 @@
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "engine": WorkflowEngineType,
-        "definitionZip": Union[str, bytes, IO[Any], StreamingBody],
+        "definitionZip": BlobTypeDef,
         "definitionUri": str,
         "main": str,
         "parameterTemplate": Mapping[str, WorkflowParameterTypeDef],
         "storageCapacity": int,
         "tags": Mapping[str, str],
         "accelerators": Literal["GPU"],
     },
@@ -2355,86 +2250,39 @@
         "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
         "storageCapacity": int,
         "creationTime": datetime,
         "statusMessage": str,
         "tags": Dict[str, str],
         "metadata": Dict[str, str],
         "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "readSets": List[ExportReadSetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "filter": ExportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
-    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ExportReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReadSetExportJobsRequestRequestTypeDef(
-    _RequiredListReadSetExportJobsRequestRequestTypeDef,
-    _OptionalListReadSetExportJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListReadSetExportJobsResponseTypeDef = TypedDict(
     "ListReadSetExportJobsResponseTypeDef",
     {
         "nextToken": str,
         "exportJobs": List[ExportReadSetJobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReadSetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetExportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -2853,15 +2701,15 @@
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReferenceSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantImportResponseTypeDef = TypedDict(
     "GetVariantImportResponseTypeDef",
     {
         "id": str,
@@ -2871,71 +2719,24 @@
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
-    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReadSetFilterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ListReadSetImportJobsRequestRequestTypeDef(
-    _RequiredListReadSetImportJobsRequestRequestTypeDef,
-    _OptionalListReadSetImportJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListReadSetImportJobsResponseTypeDef = TypedDict(
     "ListReadSetImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportReadSetSourceItemTypeDef = TypedDict(
     "_RequiredImportReadSetSourceItemTypeDef",
     {
         "sourceFiles": SourceFilesTypeDef,
@@ -2989,97 +2790,125 @@
 
 class StartReadSetImportJobSourceItemTypeDef(
     _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
 ):
     pass
 
 
-_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+ListReferenceImportJobsResponseTypeDef = TypedDict(
+    "ListReferenceImportJobsResponseTypeDef",
     {
-        "referenceStoreId": str,
+        "nextToken": str,
+        "importJobs": List[ImportReferenceJobItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+
+ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestRequestTypeDef",
     {
-        "filter": ImportReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "ids": Sequence[str],
+        "nextToken": str,
+        "filter": ListAnnotationImportJobsFilterTypeDef,
     },
     total=False,
 )
 
+ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    {
+        "ids": Sequence[str],
+        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
-    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     {
-        "referenceStoreId": str,
+        "sequenceStoreId": str,
     },
 )
-_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
+_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListReferenceImportJobsRequestRequestTypeDef(
-    _RequiredListReferenceImportJobsRequestRequestTypeDef,
-    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
+    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
 ):
     pass
 
 
-ListReferenceImportJobsResponseTypeDef = TypedDict(
-    "ListReferenceImportJobsResponseTypeDef",
+ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     {
-        "nextToken": str,
-        "importJobs": List[ImportReferenceJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListAnnotationImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "id": str,
+    },
+)
+_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
+    {
+        "status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestRequestTypeDef",
+
+class ListRunTasksRequestListRunTasksPaginateTypeDef(
+    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
+    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
+):
+    pass
+
+
+ListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "ListRunsRequestListRunsPaginateTypeDef",
     {
-        "maxResults": int,
-        "ids": Sequence[str],
-        "nextToken": str,
-        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "name": str,
+        "runGroupId": str,
+        "status": RunStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "type": WorkflowTypeType,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListAnnotationStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestRequestTypeDef = TypedDict(
     "ListAnnotationStoresRequestRequestTypeDef",
     {
@@ -3092,425 +2921,621 @@
 )
 
 ListMultipartReadSetUploadsResponseTypeDef = TypedDict(
     "ListMultipartReadSetUploadsResponseTypeDef",
     {
         "nextToken": str,
         "uploads": List[MultipartReadSetUploadListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+ListReadSetUploadPartsResponseTypeDef = TypedDict(
+    "ListReadSetUploadPartsResponseTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
+        "nextToken": str,
+        "parts": List[ReadSetUploadPartListItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+
+ListReferencesResponseTypeDef = TypedDict(
+    "ListReferencesResponseTypeDef",
     {
-        "filter": ReadSetUploadPartListFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "references": List[ReferenceListItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListRunGroupsResponseTypeDef = TypedDict(
+    "ListRunGroupsResponseTypeDef",
+    {
+        "items": List[RunGroupListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
-    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-):
-    pass
+ListRunTasksResponseTypeDef = TypedDict(
+    "ListRunTasksResponseTypeDef",
+    {
+        "items": List[TaskListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListRunsResponseTypeDef = TypedDict(
+    "ListRunsResponseTypeDef",
+    {
+        "items": List[RunListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
+ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
+    "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
+        "ids": Sequence[str],
+        "filter": ListVariantImportJobsFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
+
+ListVariantImportJobsRequestRequestTypeDef = TypedDict(
+    "ListVariantImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
+        "ids": Sequence[str],
         "nextToken": str,
-        "filter": ReadSetUploadPartListFilterTypeDef,
+        "filter": ListVariantImportJobsFilterTypeDef,
     },
     total=False,
 )
 
+ListVariantImportJobsResponseTypeDef = TypedDict(
+    "ListVariantImportJobsResponseTypeDef",
+    {
+        "variantImportJobs": List[VariantImportJobItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListReadSetUploadPartsRequestRequestTypeDef(
-    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
-    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
-):
-    pass
+ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
+    "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
+    {
+        "ids": Sequence[str],
+        "filter": ListVariantStoresFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
+ListVariantStoresRequestRequestTypeDef = TypedDict(
+    "ListVariantStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "ids": Sequence[str],
+        "nextToken": str,
+        "filter": ListVariantStoresFilterTypeDef,
+    },
+    total=False,
+)
 
-ListReadSetUploadPartsResponseTypeDef = TypedDict(
-    "ListReadSetUploadPartsResponseTypeDef",
+ListWorkflowsResponseTypeDef = TypedDict(
+    "ListWorkflowsResponseTypeDef",
     {
+        "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
-        "parts": List[ReadSetUploadPartListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
+TsvOptionsTypeDef = TypedDict(
+    "TsvOptionsTypeDef",
+    {
+        "readOptions": ReadOptionsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
+        "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
     },
 )
-_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
+_OptionalStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReadSetActivationJobRequestRequestTypeDef",
     {
-        "filter": ReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ListReadSetsRequestListReadSetsPaginateTypeDef(
-    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
-    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+class StartReadSetActivationJobRequestRequestTypeDef(
+    _RequiredStartReadSetActivationJobRequestRequestTypeDef,
+    _OptionalStartReadSetActivationJobRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestRequestTypeDef",
+_RequiredStartReferenceImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReferenceImportJobRequestRequestTypeDef",
     {
-        "sequenceStoreId": str,
+        "referenceStoreId": str,
+        "roleArn": str,
+        "sources": Sequence[StartReferenceImportJobSourceItemTypeDef],
     },
 )
-_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestRequestTypeDef",
+_OptionalStartReferenceImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReferenceImportJobRequestRequestTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReadSetFilterTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ListReadSetsRequestRequestTypeDef(
-    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
+class StartReferenceImportJobRequestRequestTypeDef(
+    _RequiredStartReferenceImportJobRequestRequestTypeDef,
+    _OptionalStartReferenceImportJobRequestRequestTypeDef,
 ):
     pass
 
 
-ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+_RequiredStartVariantImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartVariantImportRequestRequestTypeDef",
     {
-        "filter": ReferenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "destinationName": str,
+        "roleArn": str,
+        "items": Sequence[VariantImportItemSourceTypeDef],
+    },
+)
+_OptionalStartVariantImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartVariantImportRequestRequestTypeDef",
+    {
+        "runLeftNormalization": bool,
+        "annotationFields": Mapping[str, str],
     },
     total=False,
 )
 
-ListReferenceStoresRequestRequestTypeDef = TypedDict(
-    "ListReferenceStoresRequestRequestTypeDef",
+
+class StartVariantImportRequestRequestTypeDef(
+    _RequiredStartVariantImportRequestRequestTypeDef,
+    _OptionalStartVariantImportRequestRequestTypeDef,
+):
+    pass
+
+
+StoreOptionsOutputTypeDef = TypedDict(
+    "StoreOptionsOutputTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReferenceStoreFilterTypeDef,
+        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
+StoreOptionsTypeDef = TypedDict(
+    "StoreOptionsTypeDef",
     {
-        "referenceStoreId": str,
+        "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
+    total=False,
 )
-_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
+
+_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     {
-        "filter": ReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "filter": ActivateReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListReferencesRequestListReferencesPaginateTypeDef(
-    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
-    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
+class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
+    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListReferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferencesRequestRequestTypeDef",
+_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
     {
-        "referenceStoreId": str,
+        "sequenceStoreId": str,
     },
 )
-_OptionalListReferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferencesRequestRequestTypeDef",
+_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
-        "filter": ReferenceFilterTypeDef,
+        "filter": ActivateReadSetFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListReferencesRequestRequestTypeDef(
-    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
+class ListReadSetActivationJobsRequestRequestTypeDef(
+    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
+    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
 ):
     pass
 
 
-ListReferencesResponseTypeDef = TypedDict(
-    "ListReferencesResponseTypeDef",
+_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "references": List[ReferenceListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sequenceStoreId": str,
     },
 )
-
-ListRunGroupsResponseTypeDef = TypedDict(
-    "ListRunGroupsResponseTypeDef",
+_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     {
-        "items": List[RunGroupListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filter": ExportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListRunTasksResponseTypeDef = TypedDict(
-    "ListRunTasksResponseTypeDef",
+
+class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
+    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
     {
-        "items": List[TaskListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sequenceStoreId": str,
     },
 )
-
-ListRunsResponseTypeDef = TypedDict(
-    "ListRunsResponseTypeDef",
+_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
     {
-        "items": List[RunListItemTypeDef],
+        "maxResults": int,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filter": ExportReadSetFilterTypeDef,
     },
+    total=False,
 )
 
-ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+
+class ListReadSetExportJobsRequestRequestTypeDef(
+    _RequiredListReadSetExportJobsRequestRequestTypeDef,
+    _OptionalListReadSetExportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
     {
-        "filter": SequenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSequenceStoresRequestRequestTypeDef = TypedDict(
-    "ListSequenceStoresRequestRequestTypeDef",
+
+class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
+    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
-        "filter": SequenceStoreFilterTypeDef,
+        "filter": ImportReadSetFilterTypeDef,
     },
     total=False,
 )
 
-ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
-    "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
+
+class ListReadSetImportJobsRequestRequestTypeDef(
+    _RequiredListReadSetImportJobsRequestRequestTypeDef,
+    _OptionalListReadSetImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListVariantImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListVariantImportJobsRequestRequestTypeDef = TypedDict(
-    "ListVariantImportJobsRequestRequestTypeDef",
+
+class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
+    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
-        "ids": Sequence[str],
         "nextToken": str,
-        "filter": ListVariantImportJobsFilterTypeDef,
+        "filter": ImportReferenceFilterTypeDef,
     },
     total=False,
 )
 
-ListVariantImportJobsResponseTypeDef = TypedDict(
-    "ListVariantImportJobsResponseTypeDef",
+
+class ListReferenceImportJobsRequestRequestTypeDef(
+    _RequiredListReferenceImportJobsRequestRequestTypeDef,
+    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
     {
-        "variantImportJobs": List[VariantImportJobItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sequenceStoreId": str,
     },
 )
-
-ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
-    "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
+_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListVariantStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "filter": ReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListVariantStoresRequestRequestTypeDef = TypedDict(
-    "ListVariantStoresRequestRequestTypeDef",
+
+class ListReadSetsRequestListReadSetsPaginateTypeDef(
+    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
+    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestRequestTypeDef",
     {
         "maxResults": int,
-        "ids": Sequence[str],
         "nextToken": str,
-        "filter": ListVariantStoresFilterTypeDef,
+        "filter": ReadSetFilterTypeDef,
     },
     total=False,
 )
 
-ListWorkflowsResponseTypeDef = TypedDict(
-    "ListWorkflowsResponseTypeDef",
+
+class ListReadSetsRequestRequestTypeDef(
+    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
-        "items": List[WorkflowListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
     },
 )
-
-TsvOptionsTypeDef = TypedDict(
-    "TsvOptionsTypeDef",
+_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
-        "readOptions": ReadOptionsTypeDef,
+        "filter": ReadSetUploadPartListFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
+
+class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
+    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
-        "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
     },
 )
-_OptionalStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReadSetActivationJobRequestRequestTypeDef",
+_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
     {
-        "clientToken": str,
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReadSetUploadPartListFilterTypeDef,
     },
     total=False,
 )
 
 
-class StartReadSetActivationJobRequestRequestTypeDef(
-    _RequiredStartReadSetActivationJobRequestRequestTypeDef,
-    _OptionalStartReadSetActivationJobRequestRequestTypeDef,
+class ListReadSetUploadPartsRequestRequestTypeDef(
+    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
+    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStartReferenceImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReferenceImportJobRequestRequestTypeDef",
+_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
     {
         "referenceStoreId": str,
-        "roleArn": str,
-        "sources": Sequence[StartReferenceImportJobSourceItemTypeDef],
     },
 )
-_OptionalStartReferenceImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReferenceImportJobRequestRequestTypeDef",
+_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
     {
-        "clientToken": str,
+        "filter": ReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class StartReferenceImportJobRequestRequestTypeDef(
-    _RequiredStartReferenceImportJobRequestRequestTypeDef,
-    _OptionalStartReferenceImportJobRequestRequestTypeDef,
+class ListReferencesRequestListReferencesPaginateTypeDef(
+    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
+    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredStartVariantImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartVariantImportRequestRequestTypeDef",
+_RequiredListReferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferencesRequestRequestTypeDef",
     {
-        "destinationName": str,
-        "roleArn": str,
-        "items": Sequence[VariantImportItemSourceTypeDef],
+        "referenceStoreId": str,
     },
 )
-_OptionalStartVariantImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartVariantImportRequestRequestTypeDef",
+_OptionalListReferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferencesRequestRequestTypeDef",
     {
-        "runLeftNormalization": bool,
-        "annotationFields": Mapping[str, str],
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceFilterTypeDef,
     },
     total=False,
 )
 
 
-class StartVariantImportRequestRequestTypeDef(
-    _RequiredStartVariantImportRequestRequestTypeDef,
-    _OptionalStartVariantImportRequestRequestTypeDef,
+class ListReferencesRequestRequestTypeDef(
+    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
 ):
     pass
 
 
-StoreOptionsTypeDef = TypedDict(
-    "StoreOptionsTypeDef",
+ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
     {
-        "tsvStoreOptions": TsvStoreOptionsTypeDef,
+        "filter": ReferenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReferenceStoresRequestRequestTypeDef = TypedDict(
+    "ListReferenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceStoreFilterTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    {
+        "filter": SequenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestRequestTypeDef = TypedDict(
+    "ListSequenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": SequenceStoreFilterTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresResponseTypeDef = TypedDict(
     "ListAnnotationStoresResponseTypeDef",
     {
         "annotationStores": List[AnnotationStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReferenceStoresResponseTypeDef = TypedDict(
     "ListReferenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "referenceStores": List[ReferenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSequenceStoresResponseTypeDef = TypedDict(
     "ListSequenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "sequenceStores": List[SequenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresResponseTypeDef = TypedDict(
     "ListVariantStoresResponseTypeDef",
     {
         "variantStores": List[VariantStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetMetadataResponseTypeDef = TypedDict(
     "GetReadSetMetadataResponseTypeDef",
     {
         "id": str,
@@ -3523,15 +3548,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
         "id": str,
@@ -3540,39 +3565,39 @@
         "md5": str,
         "status": ReferenceStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "files": ReferenceFilesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReadSetsResponseTypeDef = TypedDict(
     "ListReadSetsResponseTypeDef",
     {
         "nextToken": str,
         "readSets": List[ReadSetListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetImportJobResponseTypeDef = TypedDict(
     "GetReadSetImportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetImportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -3601,52 +3626,25 @@
     {
         "tsvOptions": TsvOptionsTypeDef,
         "vcfOptions": VcfOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "storeFormat": StoreFormatType,
-    },
-)
-_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "reference": ReferenceItemTypeDef,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-        "storeOptions": StoreOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAnnotationStoreRequestRequestTypeDef(
-    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
-    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
-):
-    pass
-
-
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "storeFormat": StoreFormatType,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnnotationStoreResponseTypeDef = TypedDict(
     "GetAnnotationStoreResponseTypeDef",
     {
         "id": str,
@@ -3655,38 +3653,66 @@
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnnotationStoreResponseTypeDef = TypedDict(
     "UpdateAnnotationStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeFormat": StoreFormatType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+    {
         "storeFormat": StoreFormatType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAnnotationStoreRequestRequestTypeDef(
+    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
+    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+):
+    pass
+
 
+StoreOptionsUnionTypeDef = Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef]
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
@@ -3694,15 +3720,15 @@
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[AnnotationImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "formatOptions": FormatOptionsTypeDef,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartAnnotationImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartAnnotationImportRequestRequestTypeDef",
     {
         "destinationName": str,
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/type_defs.pyi` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_omics.type_defs import AbortMultipartReadSetUploadRequestRequestTypeDef
 
-    data: AbortMultipartReadSetUploadRequestRequestTypeDef = {...}
+    data: AbortMultipartReadSetUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -53,162 +53,156 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
-    "ActivateReadSetFilterTypeDef",
+    "TimestampTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
     "ReferenceItemTypeDef",
     "SseConfigTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
-    "CompleteMultipartReadSetUploadResponseTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
-    "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
-    "CreateRunGroupResponseTypeDef",
     "WorkflowParameterTypeDef",
-    "CreateWorkflowResponseTypeDef",
     "DeleteAnnotationStoreRequestRequestTypeDef",
-    "DeleteAnnotationStoreResponseTypeDef",
     "DeleteReferenceRequestRequestTypeDef",
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteSequenceStoreRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
-    "DeleteVariantStoreResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportReadSetDetailTypeDef",
-    "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
     "GetReadSetExportJobRequestRequestTypeDef",
     "GetReadSetImportJobRequestRequestTypeDef",
     "GetReadSetMetadataRequestRequestTypeDef",
     "SequenceInformationTypeDef",
     "GetReadSetRequestRequestTypeDef",
-    "GetReadSetResponseTypeDef",
     "GetReferenceImportJobRequestRequestTypeDef",
     "ImportReferenceSourceItemTypeDef",
     "GetReferenceMetadataRequestRequestTypeDef",
     "GetReferenceRequestRequestTypeDef",
-    "GetReferenceResponseTypeDef",
     "GetReferenceStoreRequestRequestTypeDef",
     "GetRunGroupRequestRequestTypeDef",
-    "GetRunGroupResponseTypeDef",
     "GetRunRequestRequestTypeDef",
-    "GetRunResponseTypeDef",
     "GetRunTaskRequestRequestTypeDef",
-    "GetRunTaskResponseTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
-    "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
     "SourceFilesTypeDef",
-    "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
-    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
-    "ReadSetUploadPartListFilterTypeDef",
     "ReadSetUploadPartListItemTypeDef",
-    "ReadSetFilterTypeDef",
-    "ReferenceStoreFilterTypeDef",
-    "ReferenceFilterTypeDef",
     "ReferenceListItemTypeDef",
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     "ListRunGroupsRequestRequestTypeDef",
     "RunGroupListItemTypeDef",
-    "ListRunTasksRequestListRunTasksPaginateTypeDef",
     "ListRunTasksRequestRequestTypeDef",
     "TaskListItemTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
     "RunListItemTypeDef",
-    "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
-    "PaginatorConfigTypeDef",
     "ReadOptionsTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartAnnotationImportResponseTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
-    "StartReadSetActivationJobResponseTypeDef",
-    "StartReadSetExportJobResponseTypeDef",
-    "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
-    "StartReferenceImportJobResponseTypeDef",
     "StartRunRequestRequestTypeDef",
-    "StartRunResponseTypeDef",
     "VariantImportItemSourceTypeDef",
-    "StartVariantImportResponseTypeDef",
+    "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
-    "UploadReadSetPartRequestRequestTypeDef",
-    "UploadReadSetPartResponseTypeDef",
-    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    "ListReadSetActivationJobsRequestRequestTypeDef",
-    "ListReadSetActivationJobsResponseTypeDef",
-    "GetReadSetActivationJobResponseTypeDef",
-    "ListAnnotationImportJobsResponseTypeDef",
-    "CreateVariantStoreResponseTypeDef",
-    "UpdateVariantStoreResponseTypeDef",
+    "ActivateReadSetFilterTypeDef",
+    "ExportReadSetFilterTypeDef",
+    "ImportReadSetFilterTypeDef",
+    "ImportReferenceFilterTypeDef",
+    "ReadSetFilterTypeDef",
+    "ReadSetUploadPartListFilterTypeDef",
+    "ReferenceFilterTypeDef",
+    "ReferenceStoreFilterTypeDef",
+    "SequenceStoreFilterTypeDef",
     "AnnotationStoreItemTypeDef",
     "CreateReferenceStoreRequestRequestTypeDef",
-    "CreateReferenceStoreResponseTypeDef",
     "CreateSequenceStoreRequestRequestTypeDef",
-    "CreateSequenceStoreResponseTypeDef",
     "CreateVariantStoreRequestRequestTypeDef",
-    "GetReferenceStoreResponseTypeDef",
-    "GetSequenceStoreResponseTypeDef",
-    "GetVariantStoreResponseTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
     "BatchDeleteReadSetResponseTypeDef",
+    "CompleteMultipartReadSetUploadResponseTypeDef",
+    "CreateMultipartReadSetUploadResponseTypeDef",
+    "CreateReferenceStoreResponseTypeDef",
+    "CreateRunGroupResponseTypeDef",
+    "CreateSequenceStoreResponseTypeDef",
+    "CreateVariantStoreResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "DeleteAnnotationStoreResponseTypeDef",
+    "DeleteVariantStoreResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetReadSetActivationJobResponseTypeDef",
+    "GetReadSetResponseTypeDef",
+    "GetReferenceResponseTypeDef",
+    "GetReferenceStoreResponseTypeDef",
+    "GetRunGroupResponseTypeDef",
+    "GetRunResponseTypeDef",
+    "GetRunTaskResponseTypeDef",
+    "GetSequenceStoreResponseTypeDef",
+    "GetVariantStoreResponseTypeDef",
+    "ListAnnotationImportJobsResponseTypeDef",
+    "ListReadSetActivationJobsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartAnnotationImportResponseTypeDef",
+    "StartReadSetActivationJobResponseTypeDef",
+    "StartReadSetExportJobResponseTypeDef",
+    "StartReadSetImportJobResponseTypeDef",
+    "StartReferenceImportJobResponseTypeDef",
+    "StartRunResponseTypeDef",
+    "StartVariantImportResponseTypeDef",
+    "UpdateVariantStoreResponseTypeDef",
+    "UploadReadSetPartResponseTypeDef",
+    "UploadReadSetPartRequestRequestTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
-    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef",
@@ -223,89 +217,91 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
     "StartReadSetImportJobSourceItemTypeDef",
-    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
+    "ListRunTasksRequestListRunTasksPaginateTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     "ListAnnotationStoresRequestRequestTypeDef",
     "ListMultipartReadSetUploadsResponseTypeDef",
-    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
-    "ListReadSetUploadPartsRequestRequestTypeDef",
     "ListReadSetUploadPartsResponseTypeDef",
-    "ListReadSetsRequestListReadSetsPaginateTypeDef",
-    "ListReadSetsRequestRequestTypeDef",
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
-    "ListReferenceStoresRequestRequestTypeDef",
-    "ListReferencesRequestListReferencesPaginateTypeDef",
-    "ListReferencesRequestRequestTypeDef",
     "ListReferencesResponseTypeDef",
     "ListRunGroupsResponseTypeDef",
     "ListRunTasksResponseTypeDef",
     "ListRunsResponseTypeDef",
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
-    "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TsvOptionsTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
+    "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
+    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    "ListReadSetActivationJobsRequestRequestTypeDef",
+    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    "ListReadSetExportJobsRequestRequestTypeDef",
+    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "ListReadSetImportJobsRequestRequestTypeDef",
+    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    "ListReferenceImportJobsRequestRequestTypeDef",
+    "ListReadSetsRequestListReadSetsPaginateTypeDef",
+    "ListReadSetsRequestRequestTypeDef",
+    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    "ListReadSetUploadPartsRequestRequestTypeDef",
+    "ListReferencesRequestListReferencesPaginateTypeDef",
+    "ListReferencesRequestRequestTypeDef",
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+    "ListReferenceStoresRequestRequestTypeDef",
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    "ListSequenceStoresRequestRequestTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
-    "CreateAnnotationStoreRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
+    "CreateAnnotationStoreRequestRequestTypeDef",
+    "StoreOptionsUnionTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
     },
 )
 
-ActivateReadSetFilterTypeDef = TypedDict(
-    "ActivateReadSetFilterTypeDef",
-    {
-        "status": ReadSetActivationJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredActivateReadSetJobItemTypeDef = TypedDict(
     "_RequiredActivateReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "status": ReadSetActivationJobStatusType,
         "creationTime": datetime,
@@ -423,14 +419,26 @@
     {
         "id": str,
         "code": str,
         "message": str,
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
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelAnnotationImportRequestRequestTypeDef = TypedDict(
     "CancelAnnotationImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -453,22 +461,14 @@
     {
         "partNumber": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
     },
 )
 
-CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CompleteMultipartReadSetUploadResponseTypeDef",
-    {
-        "readSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sourceFileType": FileTypeType,
         "subjectId": str,
         "sampleId": str,
@@ -489,32 +489,14 @@
 
 class CreateMultipartReadSetUploadRequestRequestTypeDef(
     _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef,
     _OptionalCreateMultipartReadSetUploadRequestRequestTypeDef,
 ):
     pass
 
-CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CreateMultipartReadSetUploadResponseTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "generatedFrom": str,
-        "referenceArn": str,
-        "name": str,
-        "description": str,
-        "tags": Dict[str, str],
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRunGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRunGroupRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateRunGroupRequestRequestTypeDef = TypedDict(
@@ -531,44 +513,23 @@
 )
 
 class CreateRunGroupRequestRequestTypeDef(
     _RequiredCreateRunGroupRequestRequestTypeDef, _OptionalCreateRunGroupRequestRequestTypeDef
 ):
     pass
 
-CreateRunGroupResponseTypeDef = TypedDict(
-    "CreateRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowParameterTypeDef = TypedDict(
     "WorkflowParameterTypeDef",
     {
         "description": str,
         "optional": bool,
     },
     total=False,
 )
 
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAnnotationStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
@@ -581,22 +542,14 @@
 
 class DeleteAnnotationStoreRequestRequestTypeDef(
     _RequiredDeleteAnnotationStoreRequestRequestTypeDef,
     _OptionalDeleteAnnotationStoreRequestRequestTypeDef,
 ):
     pass
 
-DeleteAnnotationStoreResponseTypeDef = TypedDict(
-    "DeleteAnnotationStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteReferenceRequestRequestTypeDef = TypedDict(
     "DeleteReferenceRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -645,36 +598,21 @@
 
 class DeleteVariantStoreRequestRequestTypeDef(
     _RequiredDeleteVariantStoreRequestRequestTypeDef,
     _OptionalDeleteVariantStoreRequestRequestTypeDef,
 ):
     pass
 
-DeleteVariantStoreResponseTypeDef = TypedDict(
-    "DeleteVariantStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportReadSetDetailTypeDef = TypedDict(
     "_RequiredExportReadSetDetailTypeDef",
     {
         "id": str,
         "status": ReadSetExportJobItemStatusType,
     },
 )
@@ -687,24 +625,14 @@
 )
 
 class ExportReadSetDetailTypeDef(
     _RequiredExportReadSetDetailTypeDef, _OptionalExportReadSetDetailTypeDef
 ):
     pass
 
-ExportReadSetFilterTypeDef = TypedDict(
-    "ExportReadSetFilterTypeDef",
-    {
-        "status": ReadSetExportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredExportReadSetJobDetailTypeDef = TypedDict(
     "_RequiredExportReadSetJobDetailTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
@@ -833,22 +761,14 @@
 )
 
 class GetReadSetRequestRequestTypeDef(
     _RequiredGetReadSetRequestRequestTypeDef, _OptionalGetReadSetRequestRequestTypeDef
 ):
     pass
 
-GetReadSetResponseTypeDef = TypedDict(
-    "GetReadSetResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceImportJobRequestRequestTypeDef = TypedDict(
     "GetReferenceImportJobRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -902,52 +822,28 @@
 )
 
 class GetReferenceRequestRequestTypeDef(
     _RequiredGetReferenceRequestRequestTypeDef, _OptionalGetReferenceRequestRequestTypeDef
 ):
     pass
 
-GetReferenceResponseTypeDef = TypedDict(
-    "GetReferenceResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceStoreRequestRequestTypeDef = TypedDict(
     "GetReferenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
 GetRunGroupRequestRequestTypeDef = TypedDict(
     "GetRunGroupRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetRunGroupResponseTypeDef = TypedDict(
-    "GetRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "maxCpus": int,
-        "maxRuns": int,
-        "maxDuration": int,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "maxGpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRunRequestRequestTypeDef = TypedDict(
     "_RequiredGetRunRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetRunRequestRequestTypeDef = TypedDict(
@@ -959,71 +855,22 @@
 )
 
 class GetRunRequestRequestTypeDef(
     _RequiredGetRunRequestRequestTypeDef, _OptionalGetRunRequestRequestTypeDef
 ):
     pass
 
-GetRunResponseTypeDef = TypedDict(
-    "GetRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "workflowId": str,
-        "workflowType": WorkflowTypeType,
-        "runId": str,
-        "roleArn": str,
-        "name": str,
-        "runGroupId": str,
-        "priority": int,
-        "definition": str,
-        "digest": str,
-        "parameters": Dict[str, Any],
-        "storageCapacity": int,
-        "outputUri": str,
-        "logLevel": RunLogLevelType,
-        "resourceDigests": Dict[str, str],
-        "startedBy": str,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRunTaskRequestRequestTypeDef = TypedDict(
     "GetRunTaskRequestRequestTypeDef",
     {
         "id": str,
         "taskId": str,
     },
 )
 
-GetRunTaskResponseTypeDef = TypedDict(
-    "GetRunTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "status": TaskStatusType,
-        "name": str,
-        "cpus": int,
-        "memory": int,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "logStream": str,
-        "gpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSequenceStoreRequestRequestTypeDef = TypedDict(
     "GetSequenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1077,24 +924,14 @@
 )
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
-ImportReadSetFilterTypeDef = TypedDict(
-    "ImportReadSetFilterTypeDef",
-    {
-        "status": ReadSetImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReadSetJobItemTypeDef = TypedDict(
     "_RequiredImportReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
@@ -1127,24 +964,14 @@
     },
     total=False,
 )
 
 class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
     pass
 
-ImportReferenceFilterTypeDef = TypedDict(
-    "ImportReferenceFilterTypeDef",
-    {
-        "status": ReferenceImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReferenceJobItemTypeDef = TypedDict(
     "_RequiredImportReferenceJobItemTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
@@ -1169,42 +996,32 @@
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
 )
 
-ListAnnotationStoresFilterTypeDef = TypedDict(
-    "ListAnnotationStoresFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StoreStatusType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+ListAnnotationStoresFilterTypeDef = TypedDict(
+    "ListAnnotationStoresFilterTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": StoreStatusType,
     },
     total=False,
 )
 
-class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
-    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartReadSetUploadsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
@@ -1246,23 +1063,14 @@
 )
 
 class MultipartReadSetUploadListItemTypeDef(
     _RequiredMultipartReadSetUploadListItemTypeDef, _OptionalMultipartReadSetUploadListItemTypeDef
 ):
     pass
 
-ReadSetUploadPartListFilterTypeDef = TypedDict(
-    "ReadSetUploadPartListFilterTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReadSetUploadPartListItemTypeDef = TypedDict(
     "_RequiredReadSetUploadPartListItemTypeDef",
     {
         "partNumber": int,
         "partSize": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
@@ -1278,50 +1086,14 @@
 )
 
 class ReadSetUploadPartListItemTypeDef(
     _RequiredReadSetUploadPartListItemTypeDef, _OptionalReadSetUploadPartListItemTypeDef
 ):
     pass
 
-ReadSetFilterTypeDef = TypedDict(
-    "ReadSetFilterTypeDef",
-    {
-        "name": str,
-        "status": ReadSetStatusType,
-        "referenceArn": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "sampleId": str,
-        "subjectId": str,
-        "generatedFrom": str,
-    },
-    total=False,
-)
-
-ReferenceStoreFilterTypeDef = TypedDict(
-    "ReferenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-ReferenceFilterTypeDef = TypedDict(
-    "ReferenceFilterTypeDef",
-    {
-        "name": str,
-        "md5": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReferenceListItemTypeDef = TypedDict(
     "_RequiredReferenceListItemTypeDef",
     {
         "id": str,
         "arn": str,
         "referenceStoreId": str,
         "md5": str,
@@ -1340,23 +1112,14 @@
 )
 
 class ReferenceListItemTypeDef(
     _RequiredReferenceListItemTypeDef, _OptionalReferenceListItemTypeDef
 ):
     pass
 
-ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunGroupsRequestRequestTypeDef = TypedDict(
     "ListRunGroupsRequestRequestTypeDef",
     {
         "name": str,
         "startingToken": str,
         "maxResults": int,
     },
@@ -1374,35 +1137,14 @@
         "maxDuration": int,
         "creationTime": datetime,
         "maxGpus": int,
     },
     total=False,
 )
 
-_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRunTasksRequestListRunTasksPaginateTypeDef(
-    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
-    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
-):
-    pass
-
 _RequiredListRunTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListRunTasksRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalListRunTasksRequestRequestTypeDef = TypedDict(
@@ -1432,25 +1174,14 @@
         "startTime": datetime,
         "stopTime": datetime,
         "gpus": int,
     },
     total=False,
 )
 
-ListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "ListRunsRequestListRunsPaginateTypeDef",
-    {
-        "name": str,
-        "runGroupId": str,
-        "status": RunStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunsRequestRequestTypeDef = TypedDict(
     "ListRunsRequestRequestTypeDef",
     {
         "name": str,
         "runGroupId": str,
         "startingToken": str,
         "maxResults": int,
@@ -1472,39 +1203,21 @@
         "creationTime": datetime,
         "startTime": datetime,
         "stopTime": datetime,
     },
     total=False,
 )
 
-SequenceStoreFilterTypeDef = TypedDict(
-    "SequenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
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
 ListVariantImportJobsFilterTypeDef = TypedDict(
     "ListVariantImportJobsFilterTypeDef",
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
@@ -1540,24 +1253,14 @@
     "ListVariantStoresFilterTypeDef",
     {
         "status": StoreStatusType,
     },
     total=False,
 )
 
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "type": WorkflowTypeType,
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "type": WorkflowTypeType,
         "name": str,
         "startingToken": str,
         "maxResults": int,
@@ -1576,24 +1279,14 @@
         "digest": str,
         "creationTime": datetime,
         "metadata": Dict[str, str],
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
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
         "sep": str,
         "encoding": str,
         "quote": str,
         "quoteAll": bool,
@@ -1602,75 +1295,21 @@
         "comment": str,
         "header": bool,
         "lineSep": str,
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
-StartAnnotationImportResponseTypeDef = TypedDict(
-    "StartAnnotationImportResponseTypeDef",
-    {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartReadSetActivationJobSourceItemTypeDef = TypedDict(
     "StartReadSetActivationJobSourceItemTypeDef",
     {
         "readSetId": str,
     },
 )
 
-StartReadSetActivationJobResponseTypeDef = TypedDict(
-    "StartReadSetActivationJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartReadSetExportJobResponseTypeDef = TypedDict(
-    "StartReadSetExportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "destination": str,
-        "status": ReadSetExportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartReadSetImportJobResponseTypeDef = TypedDict(
-    "StartReadSetImportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "roleArn": str,
-        "status": ReadSetImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartReferenceImportJobSourceItemTypeDef = TypedDict(
     "_RequiredStartReferenceImportJobSourceItemTypeDef",
     {
         "sourceFile": str,
         "name": str,
     },
 )
@@ -1685,26 +1324,14 @@
 
 class StartReferenceImportJobSourceItemTypeDef(
     _RequiredStartReferenceImportJobSourceItemTypeDef,
     _OptionalStartReferenceImportJobSourceItemTypeDef,
 ):
     pass
 
-StartReferenceImportJobResponseTypeDef = TypedDict(
-    "StartReferenceImportJobResponseTypeDef",
-    {
-        "id": str,
-        "referenceStoreId": str,
-        "roleArn": str,
-        "status": ReferenceImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartRunRequestRequestTypeDef",
     {
         "roleArn": str,
         "requestId": str,
     },
 )
@@ -1727,38 +1354,29 @@
 )
 
 class StartRunRequestRequestTypeDef(
     _RequiredStartRunRequestRequestTypeDef, _OptionalStartRunRequestRequestTypeDef
 ):
     pass
 
-StartRunResponseTypeDef = TypedDict(
-    "StartRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VariantImportItemSourceTypeDef = TypedDict(
     "VariantImportItemSourceTypeDef",
     {
         "source": str,
     },
 )
 
-StartVariantImportResponseTypeDef = TypedDict(
-    "StartVariantImportResponseTypeDef",
+TsvStoreOptionsOutputTypeDef = TypedDict(
+    "TsvStoreOptionsOutputTypeDef",
     {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "annotationType": AnnotationTypeType,
+        "formatToHeader": Dict[FormatToHeaderKeyType, str],
+        "schema": List[Dict[str, SchemaValueTypeType]],
     },
+    total=False,
 )
 
 TsvStoreOptionsTypeDef = TypedDict(
     "TsvStoreOptionsTypeDef",
     {
         "annotationType": AnnotationTypeType,
         "formatToHeader": Mapping[FormatToHeaderKeyType, str],
@@ -1862,132 +1480,107 @@
 )
 
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
-UploadReadSetPartRequestRequestTypeDef = TypedDict(
-    "UploadReadSetPartRequestRequestTypeDef",
+ActivateReadSetFilterTypeDef = TypedDict(
+    "ActivateReadSetFilterTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-        "partNumber": int,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "status": ReadSetActivationJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-UploadReadSetPartResponseTypeDef = TypedDict(
-    "UploadReadSetPartResponseTypeDef",
+ExportReadSetFilterTypeDef = TypedDict(
+    "ExportReadSetFilterTypeDef",
     {
-        "checksum": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": ReadSetExportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+ImportReadSetFilterTypeDef = TypedDict(
+    "ImportReadSetFilterTypeDef",
     {
-        "filter": ActivateReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": ReadSetImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
-    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
+ImportReferenceFilterTypeDef = TypedDict(
+    "ImportReferenceFilterTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ActivateReadSetFilterTypeDef,
+        "status": ReferenceImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-class ListReadSetActivationJobsRequestRequestTypeDef(
-    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
-    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
-):
-    pass
-
-ListReadSetActivationJobsResponseTypeDef = TypedDict(
-    "ListReadSetActivationJobsResponseTypeDef",
+ReadSetFilterTypeDef = TypedDict(
+    "ReadSetFilterTypeDef",
     {
-        "nextToken": str,
-        "activationJobs": List[ActivateReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "status": ReadSetStatusType,
+        "referenceArn": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "sampleId": str,
+        "subjectId": str,
+        "generatedFrom": str,
     },
+    total=False,
 )
 
-GetReadSetActivationJobResponseTypeDef = TypedDict(
-    "GetReadSetActivationJobResponseTypeDef",
+ReadSetUploadPartListFilterTypeDef = TypedDict(
+    "ReadSetUploadPartListFilterTypeDef",
     {
-        "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "statusMessage": str,
-        "creationTime": datetime,
-        "completionTime": datetime,
-        "sources": List[ActivateReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-ListAnnotationImportJobsResponseTypeDef = TypedDict(
-    "ListAnnotationImportJobsResponseTypeDef",
+ReferenceFilterTypeDef = TypedDict(
+    "ReferenceFilterTypeDef",
     {
-        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "md5": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-CreateVariantStoreResponseTypeDef = TypedDict(
-    "CreateVariantStoreResponseTypeDef",
+ReferenceStoreFilterTypeDef = TypedDict(
+    "ReferenceStoreFilterTypeDef",
     {
-        "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
         "name": str,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-UpdateVariantStoreResponseTypeDef = TypedDict(
-    "UpdateVariantStoreResponseTypeDef",
+SequenceStoreFilterTypeDef = TypedDict(
+    "SequenceStoreFilterTypeDef",
     {
-        "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
         "name": str,
-        "description": str,
-        "creationTime": datetime,
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
 AnnotationStoreItemTypeDef = TypedDict(
     "AnnotationStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
@@ -2023,27 +1616,14 @@
 
 class CreateReferenceStoreRequestRequestTypeDef(
     _RequiredCreateReferenceStoreRequestRequestTypeDef,
     _OptionalCreateReferenceStoreRequestRequestTypeDef,
 ):
     pass
 
-CreateReferenceStoreResponseTypeDef = TypedDict(
-    "CreateReferenceStoreResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSequenceStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
@@ -2060,28 +1640,14 @@
 
 class CreateSequenceStoreRequestRequestTypeDef(
     _RequiredCreateSequenceStoreRequestRequestTypeDef,
     _OptionalCreateSequenceStoreRequestRequestTypeDef,
 ):
     pass
 
-CreateSequenceStoreResponseTypeDef = TypedDict(
-    "CreateSequenceStoreResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVariantStoreRequestRequestTypeDef",
     {
         "reference": ReferenceItemTypeDef,
     },
 )
 _OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
@@ -2097,129 +1663,466 @@
 
 class CreateVariantStoreRequestRequestTypeDef(
     _RequiredCreateVariantStoreRequestRequestTypeDef,
     _OptionalCreateVariantStoreRequestRequestTypeDef,
 ):
     pass
 
-GetReferenceStoreResponseTypeDef = TypedDict(
-    "GetReferenceStoreResponseTypeDef",
+_RequiredReferenceStoreDetailTypeDef = TypedDict(
+    "_RequiredReferenceStoreDetailTypeDef",
     {
-        "id": str,
         "arn": str,
+        "id": str,
+        "creationTime": datetime,
+    },
+)
+_OptionalReferenceStoreDetailTypeDef = TypedDict(
+    "_OptionalReferenceStoreDetailTypeDef",
+    {
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-GetSequenceStoreResponseTypeDef = TypedDict(
-    "GetSequenceStoreResponseTypeDef",
+class ReferenceStoreDetailTypeDef(
+    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
+):
+    pass
+
+_RequiredSequenceStoreDetailTypeDef = TypedDict(
+    "_RequiredSequenceStoreDetailTypeDef",
     {
-        "id": str,
         "arn": str,
+        "id": str,
+        "creationTime": datetime,
+    },
+)
+_OptionalSequenceStoreDetailTypeDef = TypedDict(
+    "_OptionalSequenceStoreDetailTypeDef",
+    {
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
-        "creationTime": datetime,
         "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-GetVariantStoreResponseTypeDef = TypedDict(
-    "GetVariantStoreResponseTypeDef",
+class SequenceStoreDetailTypeDef(
+    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
+):
+    pass
+
+VariantStoreItemTypeDef = TypedDict(
+    "VariantStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
-        "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredReferenceStoreDetailTypeDef = TypedDict(
-    "_RequiredReferenceStoreDetailTypeDef",
+BatchDeleteReadSetResponseTypeDef = TypedDict(
+    "BatchDeleteReadSetResponseTypeDef",
+    {
+        "errors": List[ReadSetBatchErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CompleteMultipartReadSetUploadResponseTypeDef",
+    {
+        "readSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CreateMultipartReadSetUploadResponseTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "generatedFrom": str,
+        "referenceArn": str,
+        "name": str,
+        "description": str,
+        "tags": Dict[str, str],
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReferenceStoreResponseTypeDef = TypedDict(
+    "CreateReferenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRunGroupResponseTypeDef = TypedDict(
+    "CreateRunGroupResponseTypeDef",
     {
         "arn": str,
         "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSequenceStoreResponseTypeDef = TypedDict(
+    "CreateSequenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
+        "fallbackLocation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalReferenceStoreDetailTypeDef = TypedDict(
-    "_OptionalReferenceStoreDetailTypeDef",
+
+CreateVariantStoreResponseTypeDef = TypedDict(
+    "CreateVariantStoreResponseTypeDef",
     {
+        "id": str,
+        "reference": ReferenceItemTypeDef,
+        "status": StoreStatusType,
+        "name": str,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAnnotationStoreResponseTypeDef = TypedDict(
+    "DeleteAnnotationStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVariantStoreResponseTypeDef = TypedDict(
+    "DeleteVariantStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
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
+GetReadSetActivationJobResponseTypeDef = TypedDict(
+    "GetReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "statusMessage": str,
+        "creationTime": datetime,
+        "completionTime": datetime,
+        "sources": List[ActivateReadSetSourceItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReadSetResponseTypeDef = TypedDict(
+    "GetReadSetResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReferenceResponseTypeDef = TypedDict(
+    "GetReferenceResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReferenceStoreResponseTypeDef = TypedDict(
+    "GetReferenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ReferenceStoreDetailTypeDef(
-    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
-):
-    pass
+GetRunGroupResponseTypeDef = TypedDict(
+    "GetRunGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "maxCpus": int,
+        "maxRuns": int,
+        "maxDuration": int,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "maxGpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredSequenceStoreDetailTypeDef = TypedDict(
-    "_RequiredSequenceStoreDetailTypeDef",
+GetRunResponseTypeDef = TypedDict(
+    "GetRunResponseTypeDef",
     {
         "arn": str,
         "id": str,
+        "status": RunStatusType,
+        "workflowId": str,
+        "workflowType": WorkflowTypeType,
+        "runId": str,
+        "roleArn": str,
+        "name": str,
+        "runGroupId": str,
+        "priority": int,
+        "definition": str,
+        "digest": str,
+        "parameters": Dict[str, Any],
+        "storageCapacity": int,
+        "outputUri": str,
+        "logLevel": RunLogLevelType,
+        "resourceDigests": Dict[str, str],
+        "startedBy": str,
         "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSequenceStoreDetailTypeDef = TypedDict(
-    "_OptionalSequenceStoreDetailTypeDef",
+
+GetRunTaskResponseTypeDef = TypedDict(
+    "GetRunTaskResponseTypeDef",
     {
+        "taskId": str,
+        "status": TaskStatusType,
+        "name": str,
+        "cpus": int,
+        "memory": int,
+        "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "logStream": str,
+        "gpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSequenceStoreResponseTypeDef = TypedDict(
+    "GetSequenceStoreResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
+        "creationTime": datetime,
         "fallbackLocation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class SequenceStoreDetailTypeDef(
-    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
-):
-    pass
-
-VariantStoreItemTypeDef = TypedDict(
-    "VariantStoreItemTypeDef",
+GetVariantStoreResponseTypeDef = TypedDict(
+    "GetVariantStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
+        "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeleteReadSetResponseTypeDef = TypedDict(
-    "BatchDeleteReadSetResponseTypeDef",
+ListAnnotationImportJobsResponseTypeDef = TypedDict(
+    "ListAnnotationImportJobsResponseTypeDef",
     {
-        "errors": List[ReadSetBatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReadSetActivationJobsResponseTypeDef = TypedDict(
+    "ListReadSetActivationJobsResponseTypeDef",
+    {
+        "nextToken": str,
+        "activationJobs": List[ActivateReadSetJobItemTypeDef],
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
+StartAnnotationImportResponseTypeDef = TypedDict(
+    "StartAnnotationImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetActivationJobResponseTypeDef = TypedDict(
+    "StartReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetExportJobResponseTypeDef = TypedDict(
+    "StartReadSetExportJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "destination": str,
+        "status": ReadSetExportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetImportJobResponseTypeDef = TypedDict(
+    "StartReadSetImportJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "roleArn": str,
+        "status": ReadSetImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReferenceImportJobResponseTypeDef = TypedDict(
+    "StartReferenceImportJobResponseTypeDef",
+    {
+        "id": str,
+        "referenceStoreId": str,
+        "roleArn": str,
+        "status": ReferenceImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRunResponseTypeDef = TypedDict(
+    "StartRunResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVariantImportResponseTypeDef = TypedDict(
+    "StartVariantImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVariantStoreResponseTypeDef = TypedDict(
+    "UpdateVariantStoreResponseTypeDef",
+    {
+        "id": str,
+        "reference": ReferenceItemTypeDef,
+        "status": StoreStatusType,
+        "name": str,
+        "description": str,
+        "creationTime": datetime,
+        "updateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadReadSetPartResponseTypeDef = TypedDict(
+    "UploadReadSetPartResponseTypeDef",
+    {
+        "checksum": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadReadSetPartRequestRequestTypeDef = TypedDict(
+    "UploadReadSetPartRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+        "partNumber": int,
+        "payload": BlobTypeDef,
     },
 )
 
 CompleteMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -2236,15 +2139,15 @@
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "engine": WorkflowEngineType,
-        "definitionZip": Union[str, bytes, IO[Any], StreamingBody],
+        "definitionZip": BlobTypeDef,
         "definitionUri": str,
         "main": str,
         "parameterTemplate": Mapping[str, WorkflowParameterTypeDef],
         "storageCapacity": int,
         "tags": Mapping[str, str],
         "accelerators": Literal["GPU"],
     },
@@ -2272,82 +2175,39 @@
         "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
         "storageCapacity": int,
         "creationTime": datetime,
         "statusMessage": str,
         "tags": Dict[str, str],
         "metadata": Dict[str, str],
         "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "readSets": List[ExportReadSetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "filter": ExportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
-    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ExportReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetExportJobsRequestRequestTypeDef(
-    _RequiredListReadSetExportJobsRequestRequestTypeDef,
-    _OptionalListReadSetExportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListReadSetExportJobsResponseTypeDef = TypedDict(
     "ListReadSetExportJobsResponseTypeDef",
     {
         "nextToken": str,
         "exportJobs": List[ExportReadSetJobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReadSetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetExportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -2732,15 +2592,15 @@
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReferenceSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantImportResponseTypeDef = TypedDict(
     "GetVariantImportResponseTypeDef",
     {
         "id": str,
@@ -2750,67 +2610,24 @@
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
-    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReadSetFilterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListReadSetImportJobsRequestRequestTypeDef(
-    _RequiredListReadSetImportJobsRequestRequestTypeDef,
-    _OptionalListReadSetImportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListReadSetImportJobsResponseTypeDef = TypedDict(
     "ListReadSetImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportReadSetSourceItemTypeDef = TypedDict(
     "_RequiredImportReadSetSourceItemTypeDef",
     {
         "sourceFiles": SourceFilesTypeDef,
@@ -2860,337 +2677,196 @@
 )
 
 class StartReadSetImportJobSourceItemTypeDef(
     _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
 ):
     pass
 
-_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
-    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReferenceFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReferenceImportJobsRequestRequestTypeDef(
-    _RequiredListReferenceImportJobsRequestRequestTypeDef,
-    _OptionalListReferenceImportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListReferenceImportJobsResponseTypeDef = TypedDict(
     "ListReferenceImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReferenceJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
-    {
-        "ids": Sequence[str],
-        "filter": ListAnnotationImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
     "ListAnnotationImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
         "ids": Sequence[str],
         "nextToken": str,
         "filter": ListAnnotationImportJobsFilterTypeDef,
     },
     total=False,
 )
 
-ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
-    "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
-    {
-        "ids": Sequence[str],
-        "filter": ListAnnotationStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListAnnotationStoresRequestRequestTypeDef = TypedDict(
-    "ListAnnotationStoresRequestRequestTypeDef",
+ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     {
         "ids": Sequence[str],
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ListAnnotationStoresFilterTypeDef,
+        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListMultipartReadSetUploadsResponseTypeDef = TypedDict(
-    "ListMultipartReadSetUploadsResponseTypeDef",
-    {
-        "nextToken": str,
-        "uploads": List[MultipartReadSetUploadListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     {
         "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
     },
 )
-_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     {
-        "filter": ReadSetUploadPartListFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
-    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
+    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
 ):
     pass
 
-_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-    },
-)
-_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
+ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReadSetUploadPartListFilterTypeDef,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListReadSetUploadPartsRequestRequestTypeDef(
-    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
-    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
-):
-    pass
-
-ListReadSetUploadPartsResponseTypeDef = TypedDict(
-    "ListReadSetUploadPartsResponseTypeDef",
-    {
-        "nextToken": str,
-        "parts": List[ReadSetUploadPartListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
+_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
     {
-        "sequenceStoreId": str,
+        "id": str,
     },
 )
-_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
+_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
     {
-        "filter": ReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListReadSetsRequestListReadSetsPaginateTypeDef(
-    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
-    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+class ListRunTasksRequestListRunTasksPaginateTypeDef(
+    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
+    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
 ):
     pass
 
-_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestRequestTypeDef",
+ListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "ListRunsRequestListRunsPaginateTypeDef",
     {
-        "sequenceStoreId": str,
+        "name": str,
+        "runGroupId": str,
+        "status": RunStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestRequestTypeDef",
+
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReadSetFilterTypeDef,
+        "type": WorkflowTypeType,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListReadSetsRequestRequestTypeDef(
-    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
-):
-    pass
-
-ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
+    "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     {
-        "filter": ReferenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ids": Sequence[str],
+        "filter": ListAnnotationStoresFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListReferenceStoresRequestRequestTypeDef = TypedDict(
-    "ListReferenceStoresRequestRequestTypeDef",
+ListAnnotationStoresRequestRequestTypeDef = TypedDict(
+    "ListAnnotationStoresRequestRequestTypeDef",
     {
+        "ids": Sequence[str],
         "maxResults": int,
         "nextToken": str,
-        "filter": ReferenceStoreFilterTypeDef,
+        "filter": ListAnnotationStoresFilterTypeDef,
     },
     total=False,
 )
 
-_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
+ListMultipartReadSetUploadsResponseTypeDef = TypedDict(
+    "ListMultipartReadSetUploadsResponseTypeDef",
     {
-        "filter": ReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "uploads": List[MultipartReadSetUploadListItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListReferencesRequestListReferencesPaginateTypeDef(
-    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
-    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
-):
-    pass
-
-_RequiredListReferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferencesRequestRequestTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferencesRequestRequestTypeDef",
+ListReadSetUploadPartsResponseTypeDef = TypedDict(
+    "ListReadSetUploadPartsResponseTypeDef",
     {
-        "maxResults": int,
         "nextToken": str,
-        "filter": ReferenceFilterTypeDef,
+        "parts": List[ReadSetUploadPartListItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListReferencesRequestRequestTypeDef(
-    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
-):
-    pass
-
 ListReferencesResponseTypeDef = TypedDict(
     "ListReferencesResponseTypeDef",
     {
         "nextToken": str,
         "references": List[ReferenceListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunGroupsResponseTypeDef = TypedDict(
     "ListRunGroupsResponseTypeDef",
     {
         "items": List[RunGroupListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunTasksResponseTypeDef = TypedDict(
     "ListRunTasksResponseTypeDef",
     {
         "items": List[TaskListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunsResponseTypeDef = TypedDict(
     "ListRunsResponseTypeDef",
     {
         "items": List[RunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
-    {
-        "filter": SequenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
-)
-
-ListSequenceStoresRequestRequestTypeDef = TypedDict(
-    "ListSequenceStoresRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": SequenceStoreFilterTypeDef,
-    },
-    total=False,
 )
 
 ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListVariantImportJobsRequestRequestTypeDef = TypedDict(
     "ListVariantImportJobsRequestRequestTypeDef",
     {
@@ -3203,24 +2879,24 @@
 )
 
 ListVariantImportJobsResponseTypeDef = TypedDict(
     "ListVariantImportJobsResponseTypeDef",
     {
         "variantImportJobs": List[VariantImportJobItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListVariantStoresRequestRequestTypeDef = TypedDict(
     "ListVariantStoresRequestRequestTypeDef",
     {
@@ -3233,15 +2909,15 @@
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TsvOptionsTypeDef = TypedDict(
     "TsvOptionsTypeDef",
     {
         "readOptions": ReadOptionsTypeDef,
@@ -3311,55 +2987,404 @@
 
 class StartVariantImportRequestRequestTypeDef(
     _RequiredStartVariantImportRequestRequestTypeDef,
     _OptionalStartVariantImportRequestRequestTypeDef,
 ):
     pass
 
+StoreOptionsOutputTypeDef = TypedDict(
+    "StoreOptionsOutputTypeDef",
+    {
+        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 StoreOptionsTypeDef = TypedDict(
     "StoreOptionsTypeDef",
     {
         "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "filter": ActivateReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
+    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ActivateReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetActivationJobsRequestRequestTypeDef(
+    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
+    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "filter": ExportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
+    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ExportReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetExportJobsRequestRequestTypeDef(
+    _RequiredListReadSetExportJobsRequestRequestTypeDef,
+    _OptionalListReadSetExportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
+    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ImportReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetImportJobsRequestRequestTypeDef(
+    _RequiredListReadSetImportJobsRequestRequestTypeDef,
+    _OptionalListReadSetImportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
+    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ImportReferenceFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReferenceImportJobsRequestRequestTypeDef(
+    _RequiredListReferenceImportJobsRequestRequestTypeDef,
+    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
+    {
+        "filter": ReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetsRequestListReadSetsPaginateTypeDef(
+    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
+    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetsRequestRequestTypeDef(
+    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+    },
+)
+_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    {
+        "filter": ReadSetUploadPartListFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
+    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+    },
+)
+_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReadSetUploadPartListFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetUploadPartsRequestRequestTypeDef(
+    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
+    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
+    {
+        "filter": ReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReferencesRequestListReferencesPaginateTypeDef(
+    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
+    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
+):
+    pass
+
+_RequiredListReferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferencesRequestRequestTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferencesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReferencesRequestRequestTypeDef(
+    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
+):
+    pass
+
+ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+    {
+        "filter": ReferenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReferenceStoresRequestRequestTypeDef = TypedDict(
+    "ListReferenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceStoreFilterTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    {
+        "filter": SequenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestRequestTypeDef = TypedDict(
+    "ListSequenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": SequenceStoreFilterTypeDef,
+    },
+    total=False,
+)
+
 ListAnnotationStoresResponseTypeDef = TypedDict(
     "ListAnnotationStoresResponseTypeDef",
     {
         "annotationStores": List[AnnotationStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReferenceStoresResponseTypeDef = TypedDict(
     "ListReferenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "referenceStores": List[ReferenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSequenceStoresResponseTypeDef = TypedDict(
     "ListSequenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "sequenceStores": List[SequenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresResponseTypeDef = TypedDict(
     "ListVariantStoresResponseTypeDef",
     {
         "variantStores": List[VariantStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetMetadataResponseTypeDef = TypedDict(
     "GetReadSetMetadataResponseTypeDef",
     {
         "id": str,
@@ -3372,15 +3397,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
         "id": str,
@@ -3389,39 +3414,39 @@
         "md5": str,
         "status": ReferenceStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "files": ReferenceFilesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReadSetsResponseTypeDef = TypedDict(
     "ListReadSetsResponseTypeDef",
     {
         "nextToken": str,
         "readSets": List[ReadSetListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetImportJobResponseTypeDef = TypedDict(
     "GetReadSetImportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetImportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -3448,50 +3473,25 @@
     {
         "tsvOptions": TsvOptionsTypeDef,
         "vcfOptions": VcfOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "storeFormat": StoreFormatType,
-    },
-)
-_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "reference": ReferenceItemTypeDef,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-        "storeOptions": StoreOptionsTypeDef,
-    },
-    total=False,
-)
-
-class CreateAnnotationStoreRequestRequestTypeDef(
-    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
-    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
-):
-    pass
-
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "storeFormat": StoreFormatType,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnnotationStoreResponseTypeDef = TypedDict(
     "GetAnnotationStoreResponseTypeDef",
     {
         "id": str,
@@ -3500,38 +3500,64 @@
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnnotationStoreResponseTypeDef = TypedDict(
     "UpdateAnnotationStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeFormat": StoreFormatType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+    {
         "storeFormat": StoreFormatType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
+    },
+    total=False,
+)
+
+class CreateAnnotationStoreRequestRequestTypeDef(
+    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
+    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+):
+    pass
 
+StoreOptionsUnionTypeDef = Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef]
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
@@ -3539,15 +3565,15 @@
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[AnnotationImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "formatOptions": FormatOptionsTypeDef,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartAnnotationImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartAnnotationImportRequestRequestTypeDef",
     {
         "destinationName": str,
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/waiter.py` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics/waiter.pyi` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/PKG-INFO` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-omics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore omics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore omics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-omics"></a>
 
 # types-aiobotocore-omics
 
 [![PyPI - types-aiobotocore-omics](https://img.shields.io/pypi/v/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-omics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-omics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-omics?color=blue)](https://pypistats.org/packages/types-aiobotocore-omics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-omics)](https://pepy.tech/project/types-aiobotocore-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Omics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [types-aiobotocore-omics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/).
 
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
@@ -499,172 +498,166 @@
 )
 
 
 def check_value(value: AcceleratorsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_omics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_omics.type_defs import (
     AbortMultipartReadSetUploadRequestRequestTypeDef,
-    ActivateReadSetFilterTypeDef,
+    TimestampTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
     ReferenceItemTypeDef,
     SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    CompleteMultipartReadSetUploadResponseTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
-    CreateMultipartReadSetUploadResponseTypeDef,
     CreateRunGroupRequestRequestTypeDef,
-    CreateRunGroupResponseTypeDef,
     WorkflowParameterTypeDef,
-    CreateWorkflowResponseTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
-    DeleteAnnotationStoreResponseTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
-    DeleteVariantStoreResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportReadSetDetailTypeDef,
-    ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
     GetReadSetMetadataRequestRequestTypeDef,
     SequenceInformationTypeDef,
     GetReadSetRequestRequestTypeDef,
-    GetReadSetResponseTypeDef,
     GetReferenceImportJobRequestRequestTypeDef,
     ImportReferenceSourceItemTypeDef,
     GetReferenceMetadataRequestRequestTypeDef,
     GetReferenceRequestRequestTypeDef,
-    GetReferenceResponseTypeDef,
     GetReferenceStoreRequestRequestTypeDef,
     GetRunGroupRequestRequestTypeDef,
-    GetRunGroupResponseTypeDef,
     GetRunRequestRequestTypeDef,
-    GetRunResponseTypeDef,
     GetRunTaskRequestRequestTypeDef,
-    GetRunTaskResponseTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
     SourceFilesTypeDef,
-    ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
-    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
-    ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
-    ReadSetFilterTypeDef,
-    ReferenceStoreFilterTypeDef,
-    ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
-    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
-    ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
-    SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    PaginatorConfigTypeDef,
     ReadOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    StartAnnotationImportResponseTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
-    StartReadSetActivationJobResponseTypeDef,
-    StartReadSetExportJobResponseTypeDef,
-    StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
-    StartReferenceImportJobResponseTypeDef,
     StartRunRequestRequestTypeDef,
-    StartRunResponseTypeDef,
     VariantImportItemSourceTypeDef,
-    StartVariantImportResponseTypeDef,
+    TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
-    UploadReadSetPartRequestRequestTypeDef,
-    UploadReadSetPartResponseTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    ListReadSetActivationJobsRequestRequestTypeDef,
-    ListReadSetActivationJobsResponseTypeDef,
-    GetReadSetActivationJobResponseTypeDef,
-    ListAnnotationImportJobsResponseTypeDef,
-    CreateVariantStoreResponseTypeDef,
-    UpdateVariantStoreResponseTypeDef,
+    ActivateReadSetFilterTypeDef,
+    ExportReadSetFilterTypeDef,
+    ImportReadSetFilterTypeDef,
+    ImportReferenceFilterTypeDef,
+    ReadSetFilterTypeDef,
+    ReadSetUploadPartListFilterTypeDef,
+    ReferenceFilterTypeDef,
+    ReferenceStoreFilterTypeDef,
+    SequenceStoreFilterTypeDef,
     AnnotationStoreItemTypeDef,
     CreateReferenceStoreRequestRequestTypeDef,
-    CreateReferenceStoreResponseTypeDef,
     CreateSequenceStoreRequestRequestTypeDef,
-    CreateSequenceStoreResponseTypeDef,
     CreateVariantStoreRequestRequestTypeDef,
-    GetReferenceStoreResponseTypeDef,
-    GetSequenceStoreResponseTypeDef,
-    GetVariantStoreResponseTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    CompleteMultipartReadSetUploadResponseTypeDef,
+    CreateMultipartReadSetUploadResponseTypeDef,
+    CreateReferenceStoreResponseTypeDef,
+    CreateRunGroupResponseTypeDef,
+    CreateSequenceStoreResponseTypeDef,
+    CreateVariantStoreResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DeleteAnnotationStoreResponseTypeDef,
+    DeleteVariantStoreResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetReadSetActivationJobResponseTypeDef,
+    GetReadSetResponseTypeDef,
+    GetReferenceResponseTypeDef,
+    GetReferenceStoreResponseTypeDef,
+    GetRunGroupResponseTypeDef,
+    GetRunResponseTypeDef,
+    GetRunTaskResponseTypeDef,
+    GetSequenceStoreResponseTypeDef,
+    GetVariantStoreResponseTypeDef,
+    ListAnnotationImportJobsResponseTypeDef,
+    ListReadSetActivationJobsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartAnnotationImportResponseTypeDef,
+    StartReadSetActivationJobResponseTypeDef,
+    StartReadSetExportJobResponseTypeDef,
+    StartReadSetImportJobResponseTypeDef,
+    StartReferenceImportJobResponseTypeDef,
+    StartRunResponseTypeDef,
+    StartVariantImportResponseTypeDef,
+    UpdateVariantStoreResponseTypeDef,
+    UploadReadSetPartResponseTypeDef,
+    UploadReadSetPartRequestRequestTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef,
@@ -679,73 +672,84 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
-    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
+    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
+    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
+    ListRunTasksRequestListRunTasksPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
-    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
-    ListReadSetsRequestListReadSetsPaginateTypeDef,
-    ListReadSetsRequestRequestTypeDef,
-    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
-    ListReferenceStoresRequestRequestTypeDef,
-    ListReferencesRequestListReferencesPaginateTypeDef,
-    ListReferencesRequestRequestTypeDef,
     ListReferencesResponseTypeDef,
     ListRunGroupsResponseTypeDef,
     ListRunTasksResponseTypeDef,
     ListRunsResponseTypeDef,
-    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
-    ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TsvOptionsTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetActivationJobsRequestRequestTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestRequestTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestRequestTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestRequestTypeDef,
+    ListReadSetsRequestListReadSetsPaginateTypeDef,
+    ListReadSetsRequestRequestTypeDef,
+    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    ListReadSetUploadPartsRequestRequestTypeDef,
+    ListReferencesRequestListReferencesPaginateTypeDef,
+    ListReferencesRequestRequestTypeDef,
+    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
+    ListReferenceStoresRequestRequestTypeDef,
+    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
+    ListSequenceStoresRequestRequestTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
     FormatOptionsTypeDef,
-    CreateAnnotationStoreRequestRequestTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
+    CreateAnnotationStoreRequestRequestTypeDef,
+    StoreOptionsUnionTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
+def get_value() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-omics-2.5.2/types_aiobotocore_omics.egg-info/SOURCES.txt` & `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


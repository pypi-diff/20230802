# Comparing `tmp/types-aiobotocore-codecommit-2.5.2.tar.gz` & `tmp/types-aiobotocore-codecommit-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codecommit-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codecommit-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codecommit-2.5.2.tar` & `types-aiobotocore-codecommit-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.881870 types-aiobotocore-codecommit-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-07-08 01:43:23.881870 types-aiobotocore-codecommit-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21730 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.881870 types-aiobotocore-codecommit-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.881870 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74833 2023-07-08 01:27:28.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    74740 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-07-08 01:27:28.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-07-08 01:27:28.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-07-08 01:27:28.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-08 01:27:28.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    78928 2023-07-08 01:27:30.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    78833 2023-07-08 01:27:29.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:27.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.881870 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23307 2023-07-08 01:43:23.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:23.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:23.000000 types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.577625 types-aiobotocore-codecommit-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-08-02 14:52:02.573625 types-aiobotocore-codecommit-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21801 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.577625 types-aiobotocore-codecommit-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.573625 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74777 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74684 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-02 14:35:01.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79510 2023-08-02 14:35:03.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79413 2023-08-02 14:35:03.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:00.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.573625 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23331 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codecommit-2.5.2/LICENSE` & `types-aiobotocore-codecommit-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2/PKG-INFO` & `types-aiobotocore-codecommit-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecommit
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeCommit 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeCommit 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codecommit type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codecommit type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codecommit"></a>
 
 # types-aiobotocore-codecommit
 
 [![PyPI - types-aiobotocore-codecommit](https://img.shields.io/pypi/v/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codecommit?color=blue)](https://pypistats.org/packages/types-aiobotocore-codecommit)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecommit)](https://pepy.tech/project/types-aiobotocore-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeCommit 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [types-aiobotocore-codecommit docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/).
 
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
@@ -350,236 +349,239 @@
 )
 
 
 def check_value(value: ApprovalStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codecommit.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codecommit.type_defs import (
     ApprovalRuleEventMetadataTypeDef,
     ApprovalRuleOverriddenEventMetadataTypeDef,
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
+    BlobTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
     LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
-    ReplaceContentEntryTypeDef,
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
-    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
-    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
-    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
-    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
-    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
-    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
-    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
-    PutFileInputRequestTypeDef,
-    PutFileOutputTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
-    ResponseMetadataTypeDef,
+    RepositoryTriggerTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
+    ApprovalRuleTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
+    DeleteFileOutputTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
+    GetBlobOutputTypeDef,
+    GetFileOutputTypeDef,
+    GetMergeCommitOutputTypeDef,
+    GetMergeOptionsOutputTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsOutputTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
-    ApprovalRuleTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
+    PutFileInputRequestTypeDef,
+    ReplaceContentEntryTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
     PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
-    ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
+    RepositoryTriggerUnionTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
+    ConflictResolutionTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     GetCommitOutputTypeDef,
     GetMergeConflictsOutputTypeDef,
-    CreateUnreferencedMergeCommitInputRequestTypeDef,
-    MergeBranchesBySquashInputRequestTypeDef,
-    MergeBranchesByThreeWayInputRequestTypeDef,
-    MergePullRequestBySquashInputRequestTypeDef,
-    MergePullRequestByThreeWayInputRequestTypeDef,
     ConflictTypeDef,
     DescribeMergeConflictsOutputTypeDef,
     PullRequestEventTypeDef,
     PullRequestTypeDef,
     CreateCommitInputRequestTypeDef,
     GetCommentReactionsOutputTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
+    CreateUnreferencedMergeCommitInputRequestTypeDef,
+    MergeBranchesBySquashInputRequestTypeDef,
+    MergeBranchesByThreeWayInputRequestTypeDef,
+    MergePullRequestBySquashInputRequestTypeDef,
+    MergePullRequestByThreeWayInputRequestTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     DescribePullRequestEventsOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     GetPullRequestOutputTypeDef,
     MergePullRequestByFastForwardOutputTypeDef,
     MergePullRequestBySquashOutputTypeDef,
     MergePullRequestByThreeWayOutputTypeDef,
     UpdatePullRequestDescriptionOutputTypeDef,
     UpdatePullRequestStatusOutputTypeDef,
     UpdatePullRequestTitleOutputTypeDef,
 )
 
 
-def get_structure() -> ApprovalRuleEventMetadataTypeDef:
+def get_value() -> ApprovalRuleEventMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codecommit-2.5.2/README.md` & `types-aiobotocore-codecommit-2.5.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codecommit"></a>
 
 # types-aiobotocore-codecommit
 
 [![PyPI - types-aiobotocore-codecommit](https://img.shields.io/pypi/v/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codecommit?color=blue)](https://pypistats.org/packages/types-aiobotocore-codecommit)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecommit)](https://pepy.tech/project/types-aiobotocore-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeCommit 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [types-aiobotocore-codecommit docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/).
 
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
@@ -317,236 +317,239 @@
 )
 
 
 def check_value(value: ApprovalStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codecommit.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codecommit.type_defs import (
     ApprovalRuleEventMetadataTypeDef,
     ApprovalRuleOverriddenEventMetadataTypeDef,
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
+    BlobTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
     LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
-    ReplaceContentEntryTypeDef,
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
-    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
-    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
-    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
-    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
-    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
-    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
-    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
-    PutFileInputRequestTypeDef,
-    PutFileOutputTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
-    ResponseMetadataTypeDef,
+    RepositoryTriggerTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
+    ApprovalRuleTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
+    DeleteFileOutputTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
+    GetBlobOutputTypeDef,
+    GetFileOutputTypeDef,
+    GetMergeCommitOutputTypeDef,
+    GetMergeOptionsOutputTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsOutputTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
-    ApprovalRuleTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
+    PutFileInputRequestTypeDef,
+    ReplaceContentEntryTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
     PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
-    ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
+    RepositoryTriggerUnionTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
+    ConflictResolutionTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     GetCommitOutputTypeDef,
     GetMergeConflictsOutputTypeDef,
-    CreateUnreferencedMergeCommitInputRequestTypeDef,
-    MergeBranchesBySquashInputRequestTypeDef,
-    MergeBranchesByThreeWayInputRequestTypeDef,
-    MergePullRequestBySquashInputRequestTypeDef,
-    MergePullRequestByThreeWayInputRequestTypeDef,
     ConflictTypeDef,
     DescribeMergeConflictsOutputTypeDef,
     PullRequestEventTypeDef,
     PullRequestTypeDef,
     CreateCommitInputRequestTypeDef,
     GetCommentReactionsOutputTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
+    CreateUnreferencedMergeCommitInputRequestTypeDef,
+    MergeBranchesBySquashInputRequestTypeDef,
+    MergeBranchesByThreeWayInputRequestTypeDef,
+    MergePullRequestBySquashInputRequestTypeDef,
+    MergePullRequestByThreeWayInputRequestTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     DescribePullRequestEventsOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     GetPullRequestOutputTypeDef,
     MergePullRequestByFastForwardOutputTypeDef,
     MergePullRequestBySquashOutputTypeDef,
     MergePullRequestByThreeWayOutputTypeDef,
     UpdatePullRequestDescriptionOutputTypeDef,
     UpdatePullRequestStatusOutputTypeDef,
     UpdatePullRequestTitleOutputTypeDef,
 )
 
 
-def get_structure() -> ApprovalRuleEventMetadataTypeDef:
+def get_value() -> ApprovalRuleEventMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codecommit-2.5.2/setup.py` & `types-aiobotocore-codecommit-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codecommit",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeCommit 2.5.2 service generated with"
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
-    keywords="aiobotocore codecommit type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codecommit type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codecommit": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/"
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/__init__.py` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/__init__.pyi` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/__main__.py` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeCommit 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeCommit 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/client.py` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("codecommit") as client:
         client: CodeCommitClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ApprovalStateType,
     ConflictDetailLevelTypeEnumType,
     ConflictResolutionStrategyTypeEnumType,
     FileModeTypeEnumType,
@@ -44,14 +43,15 @@
 )
 from .type_defs import (
     BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
+    BlobTypeDef,
     ConflictResolutionTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     CreateUnreferencedMergeCommitOutputTypeDef,
@@ -101,15 +101,15 @@
     MergePullRequestByThreeWayOutputTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     PutFileEntryTypeDef,
     PutFileOutputTypeDef,
     PutRepositoryTriggersOutputTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerUnionTypeDef,
     SetFileModeEntryTypeDef,
     TargetTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     UpdateCommentOutputTypeDef,
@@ -1183,15 +1183,15 @@
         """
 
     async def put_file(
         self,
         *,
         repositoryName: str,
         branchName: str,
-        fileContent: Union[str, bytes, IO[Any], StreamingBody],
+        fileContent: BlobTypeDef,
         filePath: str,
         fileMode: FileModeTypeEnumType = ...,
         parentCommitId: str = ...,
         commitMessage: str = ...,
         name: str = ...,
         email: str = ...
     ) -> PutFileOutputTypeDef:
@@ -1200,15 +1200,15 @@
         generates a commit for the addition in the specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_file)
         """
 
     async def put_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> PutRepositoryTriggersOutputTypeDef:
         """
         Replaces all triggers for a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_repository_triggers)
         """
@@ -1220,15 +1220,15 @@
         Adds or updates tags for a resource in AWS CodeCommit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#tag_resource)
         """
 
     async def test_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> TestRepositoryTriggersOutputTypeDef:
         """
         Tests the functionality of repository triggers by sending information to the
         trigger target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.test_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#test_repository_triggers)
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/client.pyi` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("codecommit") as client:
         client: CodeCommitClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ApprovalStateType,
     ConflictDetailLevelTypeEnumType,
     ConflictResolutionStrategyTypeEnumType,
     FileModeTypeEnumType,
@@ -44,14 +43,15 @@
 )
 from .type_defs import (
     BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
+    BlobTypeDef,
     ConflictResolutionTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     CreateUnreferencedMergeCommitOutputTypeDef,
@@ -101,15 +101,15 @@
     MergePullRequestByThreeWayOutputTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     PutFileEntryTypeDef,
     PutFileOutputTypeDef,
     PutRepositoryTriggersOutputTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerUnionTypeDef,
     SetFileModeEntryTypeDef,
     TargetTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     UpdateCommentOutputTypeDef,
@@ -1115,15 +1115,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_comment_reaction)
         """
     async def put_file(
         self,
         *,
         repositoryName: str,
         branchName: str,
-        fileContent: Union[str, bytes, IO[Any], StreamingBody],
+        fileContent: BlobTypeDef,
         filePath: str,
         fileMode: FileModeTypeEnumType = ...,
         parentCommitId: str = ...,
         commitMessage: str = ...,
         name: str = ...,
         email: str = ...
     ) -> PutFileOutputTypeDef:
@@ -1131,15 +1131,15 @@
         Adds or updates a file in a branch in an AWS CodeCommit repository, and
         generates a commit for the addition in the specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_file)
         """
     async def put_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> PutRepositoryTriggersOutputTypeDef:
         """
         Replaces all triggers for a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#put_repository_triggers)
         """
@@ -1149,15 +1149,15 @@
         """
         Adds or updates tags for a resource in AWS CodeCommit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#tag_resource)
         """
     async def test_repository_triggers(
-        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerTypeDef]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> TestRepositoryTriggersOutputTypeDef:
         """
         Tests the functionality of repository triggers by sending information to the
         trigger target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.test_repository_triggers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/client/#test_repository_triggers)
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/literals.py` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/literals.pyi` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/paginator.py` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
 
@@ -103,15 +103,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
 
@@ -124,15 +124,15 @@
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
 
@@ -146,30 +146,30 @@
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getdifferencespaginator)
         """
 
 
 class ListBranchesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listbranchespaginator)
     """
 
     def paginate(
-        self, *, repositoryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBranchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listbranchespaginator)
         """
 
 
@@ -181,15 +181,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listpullrequestspaginator)
         """
 
 
@@ -200,13 +200,13 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/paginator.pyi` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     def paginate(
         self,
         *,
         pullRequestId: str,
         pullRequestEventType: PullRequestEventTypeType = ...,
         actorArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePullRequestEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.DescribePullRequestEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#describepullrequesteventspaginator)
         """
 
 class GetCommentsForComparedCommitPaginator(AioPaginator):
@@ -99,15 +99,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         afterCommitId: str,
         beforeCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCommentsForComparedCommitOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForComparedCommit.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforcomparedcommitpaginator)
         """
 
 class GetCommentsForPullRequestPaginator(AioPaginator):
@@ -119,15 +119,15 @@
     def paginate(
         self,
         *,
         pullRequestId: str,
         repositoryName: str = ...,
         beforeCommitId: str = ...,
         afterCommitId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCommentsForPullRequestOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetCommentsForPullRequest.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getcommentsforpullrequestpaginator)
         """
 
 class GetDifferencesPaginator(AioPaginator):
@@ -140,29 +140,29 @@
         self,
         *,
         repositoryName: str,
         afterCommitSpecifier: str,
         beforeCommitSpecifier: str = ...,
         beforePath: str = ...,
         afterPath: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDifferencesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.GetDifferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#getdifferencespaginator)
         """
 
 class ListBranchesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listbranchespaginator)
     """
 
     def paginate(
-        self, *, repositoryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, repositoryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBranchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListBranches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listbranchespaginator)
         """
 
 class ListPullRequestsPaginator(AioPaginator):
@@ -173,15 +173,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         authorArn: str = ...,
         pullRequestStatus: PullRequestStatusEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPullRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListPullRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listpullrequestspaginator)
         """
 
 class ListRepositoriesPaginator(AioPaginator):
@@ -191,13 +191,13 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SortByEnumType = ...,
         order: OrderEnumType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Paginator.ListRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/paginators/#listrepositoriespaginator)
         """
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/type_defs.py` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codecommit.type_defs import ApprovalRuleEventMetadataTypeDef
 
-    data: ApprovalRuleEventMetadataTypeDef = {...}
+    data: ApprovalRuleEventMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -47,204 +47,207 @@
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
     "AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeMergeConflictsErrorTypeDef",
     "BatchDescribeMergeConflictsInputRequestTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
+    "BlobTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
     "LocationTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
-    "ReplaceContentEntryTypeDef",
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
-    "CreateUnreferencedMergeCommitOutputTypeDef",
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
-    "DeleteApprovalRuleTemplateOutputTypeDef",
     "DeleteBranchInputRequestTypeDef",
     "DeleteCommentContentInputRequestTypeDef",
     "DeleteFileInputRequestTypeDef",
-    "DeleteFileOutputTypeDef",
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
-    "DeletePullRequestApprovalRuleOutputTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
-    "DeleteRepositoryOutputTypeDef",
     "DescribeMergeConflictsInputRequestTypeDef",
-    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribePullRequestEventsInputRequestTypeDef",
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     "EvaluationTypeDef",
     "FileTypeDef",
     "FolderTypeDef",
     "GetApprovalRuleTemplateInputRequestTypeDef",
     "GetBlobInputRequestTypeDef",
-    "GetBlobOutputTypeDef",
     "GetBranchInputRequestTypeDef",
     "GetCommentInputRequestTypeDef",
     "GetCommentReactionsInputRequestTypeDef",
-    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForComparedCommitInputRequestTypeDef",
-    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetCommentsForPullRequestInputRequestTypeDef",
     "GetCommitInputRequestTypeDef",
-    "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "GetDifferencesInputRequestTypeDef",
     "GetFileInputRequestTypeDef",
-    "GetFileOutputTypeDef",
     "GetFolderInputRequestTypeDef",
     "SubModuleTypeDef",
     "SymbolicLinkTypeDef",
     "GetMergeCommitInputRequestTypeDef",
-    "GetMergeCommitOutputTypeDef",
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
-    "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
-    "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
-    "RepositoryTriggerTypeDef",
+    "RepositoryTriggerOutputTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
-    "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
-    "ListBranchesOutputTypeDef",
-    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListPullRequestsInputRequestTypeDef",
-    "ListPullRequestsOutputTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
-    "MergeBranchesByFastForwardOutputTypeDef",
-    "MergeBranchesBySquashOutputTypeDef",
-    "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
-    "PutFileInputRequestTypeDef",
-    "PutFileOutputTypeDef",
-    "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
-    "ResponseMetadataTypeDef",
+    "RepositoryTriggerTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
     "UpdatePullRequestApprovalRuleContentInputRequestTypeDef",
     "UpdatePullRequestApprovalStateInputRequestTypeDef",
     "UpdatePullRequestDescriptionInputRequestTypeDef",
     "UpdatePullRequestStatusInputRequestTypeDef",
     "UpdatePullRequestTitleInputRequestTypeDef",
     "UpdateRepositoryDescriptionInputRequestTypeDef",
     "UpdateRepositoryNameInputRequestTypeDef",
+    "ApprovalRuleTypeDef",
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "CreateApprovalRuleTemplateOutputTypeDef",
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    "DeleteFileOutputTypeDef",
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    "DeleteRepositoryOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApprovalRuleTemplateOutputTypeDef",
+    "GetBlobOutputTypeDef",
+    "GetFileOutputTypeDef",
+    "GetMergeCommitOutputTypeDef",
+    "GetMergeOptionsOutputTypeDef",
+    "GetPullRequestApprovalStatesOutputTypeDef",
+    "GetPullRequestOverrideStateOutputTypeDef",
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    "ListBranchesOutputTypeDef",
+    "ListPullRequestsOutputTypeDef",
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "MergeBranchesByFastForwardOutputTypeDef",
+    "MergeBranchesBySquashOutputTypeDef",
+    "MergeBranchesByThreeWayOutputTypeDef",
+    "PutFileOutputTypeDef",
+    "PutRepositoryTriggersOutputTypeDef",
     "UpdateApprovalRuleTemplateContentOutputTypeDef",
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
-    "ApprovalRuleTypeDef",
-    "GetPullRequestApprovalStatesOutputTypeDef",
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
+    "PutFileInputRequestTypeDef",
+    "ReplaceContentEntryTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
     "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
     "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
-    "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
+    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    "GetDifferencesInputGetDifferencesPaginateTypeDef",
+    "ListBranchesInputListBranchesPaginateTypeDef",
+    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
+    "RepositoryTriggerUnionTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
+    "ConflictResolutionTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
     "BatchGetCommitsOutputTypeDef",
     "GetCommitOutputTypeDef",
     "GetMergeConflictsOutputTypeDef",
-    "CreateUnreferencedMergeCommitInputRequestTypeDef",
-    "MergeBranchesBySquashInputRequestTypeDef",
-    "MergeBranchesByThreeWayInputRequestTypeDef",
-    "MergePullRequestBySquashInputRequestTypeDef",
-    "MergePullRequestByThreeWayInputRequestTypeDef",
     "ConflictTypeDef",
     "DescribeMergeConflictsOutputTypeDef",
     "PullRequestEventTypeDef",
     "PullRequestTypeDef",
     "CreateCommitInputRequestTypeDef",
     "GetCommentReactionsOutputTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
+    "CreateUnreferencedMergeCommitInputRequestTypeDef",
+    "MergeBranchesBySquashInputRequestTypeDef",
+    "MergeBranchesByThreeWayInputRequestTypeDef",
+    "MergePullRequestBySquashInputRequestTypeDef",
+    "MergePullRequestByThreeWayInputRequestTypeDef",
     "BatchDescribeMergeConflictsOutputTypeDef",
     "DescribePullRequestEventsOutputTypeDef",
     "CreatePullRequestOutputTypeDef",
     "GetPullRequestOutputTypeDef",
     "MergePullRequestByFastForwardOutputTypeDef",
     "MergePullRequestBySquashOutputTypeDef",
     "MergePullRequestByThreeWayOutputTypeDef",
@@ -336,14 +339,25 @@
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryNames": Sequence[str],
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
 BatchDescribeMergeConflictsErrorTypeDef = TypedDict(
     "BatchDescribeMergeConflictsErrorTypeDef",
     {
         "filePath": str,
         "exceptionName": str,
         "message": str,
     },
@@ -445,14 +459,15 @@
         "blobId": str,
         "path": str,
         "mode": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BranchInfoTypeDef = TypedDict(
     "BranchInfoTypeDef",
     {
         "branchName": str,
         "commitId": str,
     },
     total=False,
@@ -547,37 +562,14 @@
 DeleteFileEntryTypeDef = TypedDict(
     "DeleteFileEntryTypeDef",
     {
         "filePath": str,
     },
 )
 
-_RequiredReplaceContentEntryTypeDef = TypedDict(
-    "_RequiredReplaceContentEntryTypeDef",
-    {
-        "filePath": str,
-        "replacementType": ReplacementTypeEnumType,
-    },
-)
-_OptionalReplaceContentEntryTypeDef = TypedDict(
-    "_OptionalReplaceContentEntryTypeDef",
-    {
-        "content": Union[str, bytes, IO[Any], StreamingBody],
-        "fileMode": FileModeTypeEnumType,
-    },
-    total=False,
-)
-
-
-class ReplaceContentEntryTypeDef(
-    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
-):
-    pass
-
-
 SetFileModeEntryTypeDef = TypedDict(
     "SetFileModeEntryTypeDef",
     {
         "filePath": str,
         "fileMode": FileModeTypeEnumType,
     },
 )
@@ -671,38 +663,21 @@
 
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
 
-CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 
-DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    {
-        "approvalRuleTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBranchInputRequestTypeDef = TypedDict(
     "DeleteBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
 )
@@ -737,56 +712,29 @@
 
 class DeleteFileInputRequestTypeDef(
     _RequiredDeleteFileInputRequestTypeDef, _OptionalDeleteFileInputRequestTypeDef
 ):
     pass
 
 
-DeleteFileOutputTypeDef = TypedDict(
-    "DeleteFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "filePath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePullRequestApprovalRuleInputRequestTypeDef = TypedDict(
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
     {
         "pullRequestId": str,
         "approvalRuleName": str,
     },
 )
 
-DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    {
-        "approvalRuleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRepositoryInputRequestTypeDef = TypedDict(
     "DeleteRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
-    {
-        "repositoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -808,38 +756,24 @@
 class DescribeMergeConflictsInputRequestTypeDef(
     _RequiredDescribeMergeConflictsInputRequestTypeDef,
     _OptionalDescribeMergeConflictsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
-    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribePullRequestEventsInputRequestTypeDef = TypedDict(
     "_RequiredDescribePullRequestEventsInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalDescribePullRequestEventsInputRequestTypeDef = TypedDict(
@@ -865,21 +799,14 @@
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluatePullRequestApprovalRulesInputRequestTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -927,22 +854,14 @@
     "GetBlobInputRequestTypeDef",
     {
         "repositoryName": str,
         "blobId": str,
     },
 )
 
-GetBlobOutputTypeDef = TypedDict(
-    "GetBlobOutputTypeDef",
-    {
-        "content": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBranchInputRequestTypeDef = TypedDict(
     "GetBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
     total=False,
@@ -974,38 +893,14 @@
 
 class GetCommentReactionsInputRequestTypeDef(
     _RequiredGetCommentReactionsInputRequestTypeDef, _OptionalGetCommentReactionsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-    },
-)
-_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "beforeCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
-    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCommentsForComparedCommitInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitId": str,
     },
 )
@@ -1023,39 +918,14 @@
 class GetCommentsForComparedCommitInputRequestTypeDef(
     _RequiredGetCommentsForComparedCommitInputRequestTypeDef,
     _OptionalGetCommentsForComparedCommitInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
-    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
@@ -1082,40 +952,14 @@
     "GetCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "commitId": str,
     },
 )
 
-_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitSpecifier": str,
-    },
-)
-_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "beforeCommitSpecifier": str,
-        "beforePath": str,
-        "afterPath": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDifferencesInputGetDifferencesPaginateTypeDef(
-    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
-    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDifferencesInputRequestTypeDef = TypedDict(
     "_RequiredGetDifferencesInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitSpecifier": str,
     },
 )
@@ -1156,27 +1000,14 @@
 
 class GetFileInputRequestTypeDef(
     _RequiredGetFileInputRequestTypeDef, _OptionalGetFileInputRequestTypeDef
 ):
     pass
 
 
-GetFileOutputTypeDef = TypedDict(
-    "GetFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "filePath": str,
-        "fileMode": FileModeTypeEnumType,
-        "fileSize": int,
-        "fileContent": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFolderInputRequestTypeDef = TypedDict(
     "_RequiredGetFolderInputRequestTypeDef",
     {
         "repositoryName": str,
         "folderPath": str,
     },
 )
@@ -1236,25 +1067,14 @@
 
 class GetMergeCommitInputRequestTypeDef(
     _RequiredGetMergeCommitInputRequestTypeDef, _OptionalGetMergeCommitInputRequestTypeDef
 ):
     pass
 
 
-GetMergeCommitOutputTypeDef = TypedDict(
-    "GetMergeCommitOutputTypeDef",
-    {
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "mergedCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredGetMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -1298,25 +1118,14 @@
 
 class GetMergeOptionsInputRequestTypeDef(
     _RequiredGetMergeOptionsInputRequestTypeDef, _OptionalGetMergeOptionsInputRequestTypeDef
 ):
     pass
 
 
-GetMergeOptionsOutputTypeDef = TypedDict(
-    "GetMergeOptionsOutputTypeDef",
-    {
-        "mergeOptions": List[MergeOptionTypeEnumType],
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPullRequestApprovalStatesInputRequestTypeDef = TypedDict(
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -1332,79 +1141,61 @@
     "GetPullRequestOverrideStateInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
 
-GetPullRequestOverrideStateOutputTypeDef = TypedDict(
-    "GetPullRequestOverrideStateOutputTypeDef",
-    {
-        "overridden": bool,
-        "overrider": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRepositoryInputRequestTypeDef = TypedDict(
     "GetRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
 GetRepositoryTriggersInputRequestTypeDef = TypedDict(
     "GetRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-_RequiredRepositoryTriggerTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerTypeDef",
+_RequiredRepositoryTriggerOutputTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerOutputTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": List[RepositoryTriggerEventEnumType],
     },
 )
-_OptionalRepositoryTriggerTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerTypeDef",
+_OptionalRepositoryTriggerOutputTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerOutputTypeDef",
     {
         "customData": str,
         "branches": List[str],
     },
     total=False,
 )
 
 
-class RepositoryTriggerTypeDef(
-    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+class RepositoryTriggerOutputTypeDef(
+    _RequiredRepositoryTriggerOutputTypeDef, _OptionalRepositoryTriggerOutputTypeDef
 ):
     pass
 
 
 ListApprovalRuleTemplatesInputRequestTypeDef = TypedDict(
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
@@ -1420,45 +1211,14 @@
 class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(
     _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
 ):
     pass
 
 
-ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBranchesInputListBranchesPaginateTypeDef(
-    _RequiredListBranchesInputListBranchesPaginateTypeDef,
-    _OptionalListBranchesInputListBranchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBranchesInputRequestTypeDef = TypedDict(
     "_RequiredListBranchesInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListBranchesInputRequestTypeDef = TypedDict(
@@ -1472,47 +1232,14 @@
 
 class ListBranchesInputRequestTypeDef(
     _RequiredListBranchesInputRequestTypeDef, _OptionalListBranchesInputRequestTypeDef
 ):
     pass
 
 
-ListBranchesOutputTypeDef = TypedDict(
-    "ListBranchesOutputTypeDef",
-    {
-        "branches": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "authorArn": str,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPullRequestsInputListPullRequestsPaginateTypeDef(
-    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
-    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPullRequestsInputRequestTypeDef = TypedDict(
     "_RequiredListPullRequestsInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListPullRequestsInputRequestTypeDef = TypedDict(
@@ -1529,23 +1256,14 @@
 
 class ListPullRequestsInputRequestTypeDef(
     _RequiredListPullRequestsInputRequestTypeDef, _OptionalListPullRequestsInputRequestTypeDef
 ):
     pass
 
 
-ListPullRequestsOutputTypeDef = TypedDict(
-    "ListPullRequestsOutputTypeDef",
-    {
-        "pullRequestIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
@@ -1561,33 +1279,14 @@
 class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(
     _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
 ):
     pass
 
 
-ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    {
-        "repositoryNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "sortBy": SortByEnumType,
-        "order": OrderEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "nextToken": str,
         "sortBy": SortByEnumType,
         "order": OrderEnumType,
     },
@@ -1620,23 +1319,14 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1653,41 +1343,14 @@
 class MergeBranchesByFastForwardInputRequestTypeDef(
     _RequiredMergeBranchesByFastForwardInputRequestTypeDef,
     _OptionalMergeBranchesByFastForwardInputRequestTypeDef,
 ):
     pass
 
 
-MergeBranchesByFastForwardOutputTypeDef = TypedDict(
-    "MergeBranchesByFastForwardOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesBySquashOutputTypeDef = TypedDict(
-    "MergeBranchesBySquashOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesByThreeWayOutputTypeDef = TypedDict(
-    "MergeBranchesByThreeWayOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MergeHunkDetailTypeDef = TypedDict(
     "MergeHunkDetailTypeDef",
     {
         "startLine": int,
         "endLine": int,
         "hunkContent": str,
     },
@@ -1733,24 +1396,14 @@
     {
         "pullRequestId": str,
         "revisionId": str,
         "overrideStatus": OverrideStatusType,
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
 _RequiredPostCommentReplyInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentReplyInputRequestTypeDef",
     {
         "inReplyTo": str,
         "content": str,
     },
 )
@@ -1824,60 +1477,14 @@
 
 class SourceFileSpecifierTypeDef(
     _RequiredSourceFileSpecifierTypeDef, _OptionalSourceFileSpecifierTypeDef
 ):
     pass
 
 
-_RequiredPutFileInputRequestTypeDef = TypedDict(
-    "_RequiredPutFileInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "branchName": str,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
-        "filePath": str,
-    },
-)
-_OptionalPutFileInputRequestTypeDef = TypedDict(
-    "_OptionalPutFileInputRequestTypeDef",
-    {
-        "fileMode": FileModeTypeEnumType,
-        "parentCommitId": str,
-        "commitMessage": str,
-        "name": str,
-        "email": str,
-    },
-    total=False,
-)
-
-
-class PutFileInputRequestTypeDef(
-    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
-):
-    pass
-
-
-PutFileOutputTypeDef = TypedDict(
-    "PutFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutRepositoryTriggersOutputTypeDef = TypedDict(
-    "PutRepositoryTriggersOutputTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReactionValueFormatsTypeDef = TypedDict(
     "ReactionValueFormatsTypeDef",
     {
         "emoji": str,
         "shortCode": str,
         "unicode": str,
     },
@@ -1889,25 +1496,38 @@
     {
         "trigger": str,
         "failureMessage": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredRepositoryTriggerTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "name": str,
+        "destinationArn": str,
+        "events": Sequence[RepositoryTriggerEventEnumType],
+    },
+)
+_OptionalRepositoryTriggerTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerTypeDef",
+    {
+        "customData": str,
+        "branches": Sequence[str],
     },
+    total=False,
 )
 
+
+class RepositoryTriggerTypeDef(
+    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+):
+    pass
+
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2058,175 +1678,428 @@
     "UpdateRepositoryNameInputRequestTypeDef",
     {
         "oldName": str,
         "newName": str,
     },
 )
 
+ApprovalRuleTypeDef = TypedDict(
+    "ApprovalRuleTypeDef",
+    {
+        "approvalRuleId": str,
+        "approvalRuleName": str,
+        "approvalRuleContent": str,
+        "ruleContentSha256": str,
+        "lastModifiedDate": datetime,
+        "creationDate": datetime,
+        "lastModifiedUser": str,
+        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+    },
+    total=False,
+)
+
+BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+    {
+        "associatedRepositoryNames": List[str],
+        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApprovalRuleTemplateOutputTypeDef = TypedDict(
     "CreateApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    {
+        "approvalRuleTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileOutputTypeDef = TypedDict(
+    "DeleteFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "filePath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    {
+        "approvalRuleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
+    {
+        "repositoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApprovalRuleTemplateOutputTypeDef = TypedDict(
     "GetApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+GetBlobOutputTypeDef = TypedDict(
+    "GetBlobOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "content": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+GetFileOutputTypeDef = TypedDict(
+    "GetFileOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "commitId": str,
+        "blobId": str,
+        "filePath": str,
+        "fileMode": FileModeTypeEnumType,
+        "fileSize": int,
+        "fileContent": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+GetMergeCommitOutputTypeDef = TypedDict(
+    "GetMergeCommitOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "mergedCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApprovalRuleTypeDef = TypedDict(
-    "ApprovalRuleTypeDef",
+GetMergeOptionsOutputTypeDef = TypedDict(
+    "GetMergeOptionsOutputTypeDef",
     {
-        "approvalRuleId": str,
-        "approvalRuleName": str,
-        "approvalRuleContent": str,
-        "ruleContentSha256": str,
-        "lastModifiedDate": datetime,
-        "creationDate": datetime,
-        "lastModifiedUser": str,
-        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+        "mergeOptions": List[MergeOptionTypeEnumType],
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetPullRequestApprovalStatesOutputTypeDef = TypedDict(
     "GetPullRequestApprovalStatesOutputTypeDef",
     {
         "approvals": List[ApprovalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+GetPullRequestOverrideStateOutputTypeDef = TypedDict(
+    "GetPullRequestOverrideStateOutputTypeDef",
     {
-        "associatedRepositoryNames": List[str],
-        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "overridden": bool,
+        "overrider": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBranchesOutputTypeDef = TypedDict(
+    "ListBranchesOutputTypeDef",
+    {
+        "branches": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPullRequestsOutputTypeDef = TypedDict(
+    "ListPullRequestsOutputTypeDef",
+    {
+        "pullRequestIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    {
+        "repositoryNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByFastForwardOutputTypeDef = TypedDict(
+    "MergeBranchesByFastForwardOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesBySquashOutputTypeDef = TypedDict(
+    "MergeBranchesBySquashOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByThreeWayOutputTypeDef = TypedDict(
+    "MergeBranchesByThreeWayOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFileOutputTypeDef = TypedDict(
+    "PutFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersOutputTypeDef = TypedDict(
+    "PutRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef = TypedDict(
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     {
         "disassociatedRepositoryNames": List[str],
         "errors": List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetRepositoriesOutputTypeDef = TypedDict(
     "BatchGetRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryMetadataTypeDef],
         "repositoriesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DifferenceTypeDef = TypedDict(
     "DifferenceTypeDef",
     {
         "beforeBlob": BlobMetadataTypeDef,
         "afterBlob": BlobMetadataTypeDef,
         "changeType": ChangeTypeEnumType,
     },
     total=False,
 )
 
+_RequiredPutFileInputRequestTypeDef = TypedDict(
+    "_RequiredPutFileInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+        "fileContent": BlobTypeDef,
+        "filePath": str,
+    },
+)
+_OptionalPutFileInputRequestTypeDef = TypedDict(
+    "_OptionalPutFileInputRequestTypeDef",
+    {
+        "fileMode": FileModeTypeEnumType,
+        "parentCommitId": str,
+        "commitMessage": str,
+        "name": str,
+        "email": str,
+    },
+    total=False,
+)
+
+
+class PutFileInputRequestTypeDef(
+    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
+):
+    pass
+
+
+_RequiredReplaceContentEntryTypeDef = TypedDict(
+    "_RequiredReplaceContentEntryTypeDef",
+    {
+        "filePath": str,
+        "replacementType": ReplacementTypeEnumType,
+    },
+)
+_OptionalReplaceContentEntryTypeDef = TypedDict(
+    "_OptionalReplaceContentEntryTypeDef",
+    {
+        "content": BlobTypeDef,
+        "fileMode": FileModeTypeEnumType,
+    },
+    total=False,
+)
+
+
+class ReplaceContentEntryTypeDef(
+    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
+):
+    pass
+
+
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBranchOutputTypeDef = TypedDict(
     "GetBranchOutputTypeDef",
     {
         "branch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCommentContentOutputTypeDef = TypedDict(
     "DeleteCommentContentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentOutputTypeDef = TypedDict(
     "GetCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PostCommentReplyOutputTypeDef = TypedDict(
     "PostCommentReplyOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCommentOutputTypeDef = TypedDict(
     "UpdateCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentsForComparedCommitTypeDef = TypedDict(
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
@@ -2287,15 +2160,15 @@
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
@@ -2329,15 +2202,15 @@
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
     {
         "commitId": str,
@@ -2364,33 +2237,23 @@
         "fileModeConflict": bool,
         "objectTypeConflict": bool,
         "mergeOperations": MergeOperationsTypeDef,
     },
     total=False,
 )
 
-ConflictResolutionTypeDef = TypedDict(
-    "ConflictResolutionTypeDef",
-    {
-        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
 CreateCommitOutputTypeDef = TypedDict(
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
         "filesDeleted": List[FileMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePullRequestInputRequestTypeDef = TypedDict(
     "_RequiredCreatePullRequestInputRequestTypeDef",
     {
         "title": str,
@@ -2409,67 +2272,206 @@
 
 class CreatePullRequestInputRequestTypeDef(
     _RequiredCreatePullRequestInputRequestTypeDef, _OptionalCreatePullRequestInputRequestTypeDef
 ):
     pass
 
 
+_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestId": str,
+    },
+)
+_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
+    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitId": str,
+    },
+)
+_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "beforeCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
+    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "pullRequestId": str,
+    },
+)
+_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
+    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitSpecifier": str,
+    },
+)
+_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "beforeCommitSpecifier": str,
+        "beforePath": str,
+        "afterPath": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDifferencesInputGetDifferencesPaginateTypeDef(
+    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
+    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBranchesInputListBranchesPaginateTypeDef(
+    _RequiredListBranchesInputListBranchesPaginateTypeDef,
+    _OptionalListBranchesInputListBranchesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "authorArn": str,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPullRequestsInputListPullRequestsPaginateTypeDef(
+    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
+    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
+):
+    pass
+
+
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "sortBy": SortByEnumType,
+        "order": OrderEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     {
         "evaluation": EvaluationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderOutputTypeDef = TypedDict(
     "GetFolderOutputTypeDef",
     {
         "commitId": str,
         "folderPath": str,
         "treeId": str,
         "subFolders": List[FolderTypeDef],
         "files": List[FileTypeDef],
         "symbolicLinks": List[SymbolicLinkTypeDef],
         "subModules": List[SubModuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
-        "triggers": List[RepositoryTriggerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
-    },
-)
-
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
+        "triggers": List[RepositoryTriggerOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryNameIdPairTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
@@ -2510,15 +2512,15 @@
         "filePath": str,
     },
 )
 _OptionalPutFileEntryTypeDef = TypedDict(
     "_OptionalPutFileEntryTypeDef",
     {
         "fileMode": FileModeTypeEnumType,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "fileContent": BlobTypeDef,
         "sourceFile": SourceFileSpecifierTypeDef,
     },
     total=False,
 )
 
 
 class PutFileEntryTypeDef(_RequiredPutFileEntryTypeDef, _OptionalPutFileEntryTypeDef):
@@ -2536,88 +2538,215 @@
 )
 
 TestRepositoryTriggersOutputTypeDef = TypedDict(
     "TestRepositoryTriggersOutputTypeDef",
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RepositoryTriggerUnionTypeDef = Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestApprovalRuleContentOutputTypeDef = TypedDict(
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDifferencesOutputTypeDef = TypedDict(
     "GetDifferencesOutputTypeDef",
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConflictResolutionTypeDef = TypedDict(
+    "ConflictResolutionTypeDef",
+    {
+        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentsForPullRequestOutputTypeDef = TypedDict(
     "GetCommentsForPullRequestOutputTypeDef",
     {
         "commentsForPullRequestData": List[CommentsForPullRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetCommitsOutputTypeDef = TypedDict(
     "BatchGetCommitsOutputTypeDef",
     {
         "commits": List[CommitTypeDef],
         "errors": List[BatchGetCommitsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommitOutputTypeDef = TypedDict(
     "GetCommitOutputTypeDef",
     {
         "commit": CommitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMergeConflictsOutputTypeDef = TypedDict(
     "GetMergeConflictsOutputTypeDef",
     {
         "mergeable": bool,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConflictTypeDef = TypedDict(
+    "ConflictTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+    },
+    total=False,
+)
+
+DescribeMergeConflictsOutputTypeDef = TypedDict(
+    "DescribeMergeConflictsOutputTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+        "nextToken": str,
+        "destinationCommitId": str,
+        "sourceCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PullRequestEventTypeDef = TypedDict(
+    "PullRequestEventTypeDef",
+    {
+        "pullRequestId": str,
+        "eventDate": datetime,
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
+        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
+        "pullRequestSourceReferenceUpdatedEventMetadata": (
+            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
+        ),
+        "pullRequestMergedStateChangedEventMetadata": (
+            PullRequestMergedStateChangedEventMetadataTypeDef
+        ),
+        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
+        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
+        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
+    },
+    total=False,
+)
+
+PullRequestTypeDef = TypedDict(
+    "PullRequestTypeDef",
+    {
+        "pullRequestId": str,
+        "title": str,
+        "description": str,
+        "lastActivityDate": datetime,
+        "creationDate": datetime,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "authorArn": str,
+        "pullRequestTargets": List[PullRequestTargetTypeDef],
+        "clientRequestToken": str,
+        "revisionId": str,
+        "approvalRules": List[ApprovalRuleTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateCommitInputRequestTypeDef = TypedDict(
+    "_RequiredCreateCommitInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+    },
+)
+_OptionalCreateCommitInputRequestTypeDef = TypedDict(
+    "_OptionalCreateCommitInputRequestTypeDef",
+    {
+        "parentCommitId": str,
+        "authorName": str,
+        "email": str,
+        "commitMessage": str,
+        "keepEmptyFolders": bool,
+        "putFiles": Sequence[PutFileEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateCommitInputRequestTypeDef(
+    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
+):
+    pass
+
+
+GetCommentReactionsOutputTypeDef = TypedDict(
+    "GetCommentReactionsOutputTypeDef",
+    {
+        "reactionsForComment": List[ReactionForCommentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
     },
 )
 
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2766,192 +2895,92 @@
 class MergePullRequestByThreeWayInputRequestTypeDef(
     _RequiredMergePullRequestByThreeWayInputRequestTypeDef,
     _OptionalMergePullRequestByThreeWayInputRequestTypeDef,
 ):
     pass
 
 
-ConflictTypeDef = TypedDict(
-    "ConflictTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-    },
-    total=False,
-)
-
-DescribeMergeConflictsOutputTypeDef = TypedDict(
-    "DescribeMergeConflictsOutputTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-        "nextToken": str,
-        "destinationCommitId": str,
-        "sourceCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PullRequestEventTypeDef = TypedDict(
-    "PullRequestEventTypeDef",
-    {
-        "pullRequestId": str,
-        "eventDate": datetime,
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
-        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
-        "pullRequestSourceReferenceUpdatedEventMetadata": (
-            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
-        ),
-        "pullRequestMergedStateChangedEventMetadata": (
-            PullRequestMergedStateChangedEventMetadataTypeDef
-        ),
-        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
-        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
-        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
-    },
-    total=False,
-)
-
-PullRequestTypeDef = TypedDict(
-    "PullRequestTypeDef",
-    {
-        "pullRequestId": str,
-        "title": str,
-        "description": str,
-        "lastActivityDate": datetime,
-        "creationDate": datetime,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "authorArn": str,
-        "pullRequestTargets": List[PullRequestTargetTypeDef],
-        "clientRequestToken": str,
-        "revisionId": str,
-        "approvalRules": List[ApprovalRuleTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateCommitInputRequestTypeDef = TypedDict(
-    "_RequiredCreateCommitInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "branchName": str,
-    },
-)
-_OptionalCreateCommitInputRequestTypeDef = TypedDict(
-    "_OptionalCreateCommitInputRequestTypeDef",
-    {
-        "parentCommitId": str,
-        "authorName": str,
-        "email": str,
-        "commitMessage": str,
-        "keepEmptyFolders": bool,
-        "putFiles": Sequence[PutFileEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateCommitInputRequestTypeDef(
-    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
-):
-    pass
-
-
-GetCommentReactionsOutputTypeDef = TypedDict(
-    "GetCommentReactionsOutputTypeDef",
-    {
-        "reactionsForComment": List[ReactionForCommentTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePullRequestEventsOutputTypeDef = TypedDict(
     "DescribePullRequestEventsOutputTypeDef",
     {
         "pullRequestEvents": List[PullRequestEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePullRequestOutputTypeDef = TypedDict(
     "CreatePullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPullRequestOutputTypeDef = TypedDict(
     "GetPullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByFastForwardOutputTypeDef = TypedDict(
     "MergePullRequestByFastForwardOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestBySquashOutputTypeDef = TypedDict(
     "MergePullRequestBySquashOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByThreeWayOutputTypeDef = TypedDict(
     "MergePullRequestByThreeWayOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestDescriptionOutputTypeDef = TypedDict(
     "UpdatePullRequestDescriptionOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestStatusOutputTypeDef = TypedDict(
     "UpdatePullRequestStatusOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestTitleOutputTypeDef = TypedDict(
     "UpdatePullRequestTitleOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit/type_defs.pyi` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codecommit.type_defs import ApprovalRuleEventMetadataTypeDef
 
-    data: ApprovalRuleEventMetadataTypeDef = {...}
+    data: ApprovalRuleEventMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -46,204 +46,207 @@
     "ApprovalRuleTemplateTypeDef",
     "OriginApprovalRuleTemplateTypeDef",
     "ApprovalStateChangedEventMetadataTypeDef",
     "ApprovalTypeDef",
     "AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef",
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeMergeConflictsErrorTypeDef",
     "BatchDescribeMergeConflictsInputRequestTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
+    "BlobTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
     "LocationTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
-    "ReplaceContentEntryTypeDef",
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
-    "CreateUnreferencedMergeCommitOutputTypeDef",
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
-    "DeleteApprovalRuleTemplateOutputTypeDef",
     "DeleteBranchInputRequestTypeDef",
     "DeleteCommentContentInputRequestTypeDef",
     "DeleteFileInputRequestTypeDef",
-    "DeleteFileOutputTypeDef",
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
-    "DeletePullRequestApprovalRuleOutputTypeDef",
     "DeleteRepositoryInputRequestTypeDef",
-    "DeleteRepositoryOutputTypeDef",
     "DescribeMergeConflictsInputRequestTypeDef",
-    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribePullRequestEventsInputRequestTypeDef",
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     "EvaluationTypeDef",
     "FileTypeDef",
     "FolderTypeDef",
     "GetApprovalRuleTemplateInputRequestTypeDef",
     "GetBlobInputRequestTypeDef",
-    "GetBlobOutputTypeDef",
     "GetBranchInputRequestTypeDef",
     "GetCommentInputRequestTypeDef",
     "GetCommentReactionsInputRequestTypeDef",
-    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForComparedCommitInputRequestTypeDef",
-    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetCommentsForPullRequestInputRequestTypeDef",
     "GetCommitInputRequestTypeDef",
-    "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "GetDifferencesInputRequestTypeDef",
     "GetFileInputRequestTypeDef",
-    "GetFileOutputTypeDef",
     "GetFolderInputRequestTypeDef",
     "SubModuleTypeDef",
     "SymbolicLinkTypeDef",
     "GetMergeCommitInputRequestTypeDef",
-    "GetMergeCommitOutputTypeDef",
     "GetMergeConflictsInputRequestTypeDef",
     "GetMergeOptionsInputRequestTypeDef",
-    "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
-    "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
-    "RepositoryTriggerTypeDef",
+    "RepositoryTriggerOutputTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
-    "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
-    "ListBranchesOutputTypeDef",
-    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
     "ListPullRequestsInputRequestTypeDef",
-    "ListPullRequestsOutputTypeDef",
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
-    "MergeBranchesByFastForwardOutputTypeDef",
-    "MergeBranchesBySquashOutputTypeDef",
-    "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
-    "PutFileInputRequestTypeDef",
-    "PutFileOutputTypeDef",
-    "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
-    "ResponseMetadataTypeDef",
+    "RepositoryTriggerTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
     "UpdatePullRequestApprovalRuleContentInputRequestTypeDef",
     "UpdatePullRequestApprovalStateInputRequestTypeDef",
     "UpdatePullRequestDescriptionInputRequestTypeDef",
     "UpdatePullRequestStatusInputRequestTypeDef",
     "UpdatePullRequestTitleInputRequestTypeDef",
     "UpdateRepositoryDescriptionInputRequestTypeDef",
     "UpdateRepositoryNameInputRequestTypeDef",
+    "ApprovalRuleTypeDef",
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "CreateApprovalRuleTemplateOutputTypeDef",
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    "DeleteFileOutputTypeDef",
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    "DeleteRepositoryOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetApprovalRuleTemplateOutputTypeDef",
+    "GetBlobOutputTypeDef",
+    "GetFileOutputTypeDef",
+    "GetMergeCommitOutputTypeDef",
+    "GetMergeOptionsOutputTypeDef",
+    "GetPullRequestApprovalStatesOutputTypeDef",
+    "GetPullRequestOverrideStateOutputTypeDef",
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    "ListBranchesOutputTypeDef",
+    "ListPullRequestsOutputTypeDef",
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "MergeBranchesByFastForwardOutputTypeDef",
+    "MergeBranchesBySquashOutputTypeDef",
+    "MergeBranchesByThreeWayOutputTypeDef",
+    "PutFileOutputTypeDef",
+    "PutRepositoryTriggersOutputTypeDef",
     "UpdateApprovalRuleTemplateContentOutputTypeDef",
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
-    "ApprovalRuleTypeDef",
-    "GetPullRequestApprovalStatesOutputTypeDef",
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
+    "PutFileInputRequestTypeDef",
+    "ReplaceContentEntryTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
     "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
     "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
-    "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
+    "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    "GetDifferencesInputGetDifferencesPaginateTypeDef",
+    "ListBranchesInputListBranchesPaginateTypeDef",
+    "ListPullRequestsInputListPullRequestsPaginateTypeDef",
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
+    "RepositoryTriggerUnionTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
+    "ConflictResolutionTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
     "BatchGetCommitsOutputTypeDef",
     "GetCommitOutputTypeDef",
     "GetMergeConflictsOutputTypeDef",
-    "CreateUnreferencedMergeCommitInputRequestTypeDef",
-    "MergeBranchesBySquashInputRequestTypeDef",
-    "MergeBranchesByThreeWayInputRequestTypeDef",
-    "MergePullRequestBySquashInputRequestTypeDef",
-    "MergePullRequestByThreeWayInputRequestTypeDef",
     "ConflictTypeDef",
     "DescribeMergeConflictsOutputTypeDef",
     "PullRequestEventTypeDef",
     "PullRequestTypeDef",
     "CreateCommitInputRequestTypeDef",
     "GetCommentReactionsOutputTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
+    "CreateUnreferencedMergeCommitInputRequestTypeDef",
+    "MergeBranchesBySquashInputRequestTypeDef",
+    "MergeBranchesByThreeWayInputRequestTypeDef",
+    "MergePullRequestBySquashInputRequestTypeDef",
+    "MergePullRequestByThreeWayInputRequestTypeDef",
     "BatchDescribeMergeConflictsOutputTypeDef",
     "DescribePullRequestEventsOutputTypeDef",
     "CreatePullRequestOutputTypeDef",
     "GetPullRequestOutputTypeDef",
     "MergePullRequestByFastForwardOutputTypeDef",
     "MergePullRequestBySquashOutputTypeDef",
     "MergePullRequestByThreeWayOutputTypeDef",
@@ -335,14 +338,25 @@
     "BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryNames": Sequence[str],
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
 BatchDescribeMergeConflictsErrorTypeDef = TypedDict(
     "BatchDescribeMergeConflictsErrorTypeDef",
     {
         "filePath": str,
         "exceptionName": str,
         "message": str,
     },
@@ -442,14 +456,15 @@
         "blobId": str,
         "path": str,
         "mode": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BranchInfoTypeDef = TypedDict(
     "BranchInfoTypeDef",
     {
         "branchName": str,
         "commitId": str,
     },
     total=False,
@@ -544,35 +559,14 @@
 DeleteFileEntryTypeDef = TypedDict(
     "DeleteFileEntryTypeDef",
     {
         "filePath": str,
     },
 )
 
-_RequiredReplaceContentEntryTypeDef = TypedDict(
-    "_RequiredReplaceContentEntryTypeDef",
-    {
-        "filePath": str,
-        "replacementType": ReplacementTypeEnumType,
-    },
-)
-_OptionalReplaceContentEntryTypeDef = TypedDict(
-    "_OptionalReplaceContentEntryTypeDef",
-    {
-        "content": Union[str, bytes, IO[Any], StreamingBody],
-        "fileMode": FileModeTypeEnumType,
-    },
-    total=False,
-)
-
-class ReplaceContentEntryTypeDef(
-    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
-):
-    pass
-
 SetFileModeEntryTypeDef = TypedDict(
     "SetFileModeEntryTypeDef",
     {
         "filePath": str,
         "fileMode": FileModeTypeEnumType,
     },
 )
@@ -660,38 +654,21 @@
 )
 
 class CreateRepositoryInputRequestTypeDef(
     _RequiredCreateRepositoryInputRequestTypeDef, _OptionalCreateRepositoryInputRequestTypeDef
 ):
     pass
 
-CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
-    "CreateUnreferencedMergeCommitOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "DeleteApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 
-DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "DeleteApprovalRuleTemplateOutputTypeDef",
-    {
-        "approvalRuleTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBranchInputRequestTypeDef = TypedDict(
     "DeleteBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
 )
@@ -724,56 +701,29 @@
 )
 
 class DeleteFileInputRequestTypeDef(
     _RequiredDeleteFileInputRequestTypeDef, _OptionalDeleteFileInputRequestTypeDef
 ):
     pass
 
-DeleteFileOutputTypeDef = TypedDict(
-    "DeleteFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "filePath": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePullRequestApprovalRuleInputRequestTypeDef = TypedDict(
     "DeletePullRequestApprovalRuleInputRequestTypeDef",
     {
         "pullRequestId": str,
         "approvalRuleName": str,
     },
 )
 
-DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
-    "DeletePullRequestApprovalRuleOutputTypeDef",
-    {
-        "approvalRuleId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRepositoryInputRequestTypeDef = TypedDict(
     "DeleteRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-DeleteRepositoryOutputTypeDef = TypedDict(
-    "DeleteRepositoryOutputTypeDef",
-    {
-        "repositoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -793,36 +743,24 @@
 
 class DescribeMergeConflictsInputRequestTypeDef(
     _RequiredDescribeMergeConflictsInputRequestTypeDef,
     _OptionalDescribeMergeConflictsInputRequestTypeDef,
 ):
     pass
 
-_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
-    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribePullRequestEventsInputRequestTypeDef = TypedDict(
     "_RequiredDescribePullRequestEventsInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalDescribePullRequestEventsInputRequestTypeDef = TypedDict(
@@ -846,21 +784,14 @@
     "DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
         "repositoryName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluatePullRequestApprovalRulesInputRequestTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -908,22 +839,14 @@
     "GetBlobInputRequestTypeDef",
     {
         "repositoryName": str,
         "blobId": str,
     },
 )
 
-GetBlobOutputTypeDef = TypedDict(
-    "GetBlobOutputTypeDef",
-    {
-        "content": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBranchInputRequestTypeDef = TypedDict(
     "GetBranchInputRequestTypeDef",
     {
         "repositoryName": str,
         "branchName": str,
     },
     total=False,
@@ -953,36 +876,14 @@
 )
 
 class GetCommentReactionsInputRequestTypeDef(
     _RequiredGetCommentReactionsInputRequestTypeDef, _OptionalGetCommentReactionsInputRequestTypeDef
 ):
     pass
 
-_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-    },
-)
-_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
-    {
-        "beforeCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
-    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
-):
-    pass
-
 _RequiredGetCommentsForComparedCommitInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitId": str,
     },
 )
@@ -998,37 +899,14 @@
 
 class GetCommentsForComparedCommitInputRequestTypeDef(
     _RequiredGetCommentsForComparedCommitInputRequestTypeDef,
     _OptionalGetCommentsForComparedCommitInputRequestTypeDef,
 ):
     pass
 
-_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "pullRequestId": str,
-    },
-)
-_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
-    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
-    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
-):
-    pass
-
 _RequiredGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredGetCommentsForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
     },
 )
 _OptionalGetCommentsForPullRequestInputRequestTypeDef = TypedDict(
@@ -1053,38 +931,14 @@
     "GetCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "commitId": str,
     },
 )
 
-_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitSpecifier": str,
-    },
-)
-_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
-    {
-        "beforeCommitSpecifier": str,
-        "beforePath": str,
-        "afterPath": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDifferencesInputGetDifferencesPaginateTypeDef(
-    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
-    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetDifferencesInputRequestTypeDef = TypedDict(
     "_RequiredGetDifferencesInputRequestTypeDef",
     {
         "repositoryName": str,
         "afterCommitSpecifier": str,
     },
 )
@@ -1121,27 +975,14 @@
 )
 
 class GetFileInputRequestTypeDef(
     _RequiredGetFileInputRequestTypeDef, _OptionalGetFileInputRequestTypeDef
 ):
     pass
 
-GetFileOutputTypeDef = TypedDict(
-    "GetFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "filePath": str,
-        "fileMode": FileModeTypeEnumType,
-        "fileSize": int,
-        "fileContent": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetFolderInputRequestTypeDef = TypedDict(
     "_RequiredGetFolderInputRequestTypeDef",
     {
         "repositoryName": str,
         "folderPath": str,
     },
 )
@@ -1197,25 +1038,14 @@
 )
 
 class GetMergeCommitInputRequestTypeDef(
     _RequiredGetMergeCommitInputRequestTypeDef, _OptionalGetMergeCommitInputRequestTypeDef
 ):
     pass
 
-GetMergeCommitOutputTypeDef = TypedDict(
-    "GetMergeCommitOutputTypeDef",
-    {
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "mergedCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMergeConflictsInputRequestTypeDef = TypedDict(
     "_RequiredGetMergeConflictsInputRequestTypeDef",
     {
         "repositoryName": str,
         "destinationCommitSpecifier": str,
         "sourceCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -1255,25 +1085,14 @@
 )
 
 class GetMergeOptionsInputRequestTypeDef(
     _RequiredGetMergeOptionsInputRequestTypeDef, _OptionalGetMergeOptionsInputRequestTypeDef
 ):
     pass
 
-GetMergeOptionsOutputTypeDef = TypedDict(
-    "GetMergeOptionsOutputTypeDef",
-    {
-        "mergeOptions": List[MergeOptionTypeEnumType],
-        "sourceCommitId": str,
-        "destinationCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPullRequestApprovalStatesInputRequestTypeDef = TypedDict(
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
@@ -1289,77 +1108,59 @@
     "GetPullRequestOverrideStateInputRequestTypeDef",
     {
         "pullRequestId": str,
         "revisionId": str,
     },
 )
 
-GetPullRequestOverrideStateOutputTypeDef = TypedDict(
-    "GetPullRequestOverrideStateOutputTypeDef",
-    {
-        "overridden": bool,
-        "overrider": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRepositoryInputRequestTypeDef = TypedDict(
     "GetRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
 GetRepositoryTriggersInputRequestTypeDef = TypedDict(
     "GetRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-_RequiredRepositoryTriggerTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerTypeDef",
+_RequiredRepositoryTriggerOutputTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerOutputTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": List[RepositoryTriggerEventEnumType],
     },
 )
-_OptionalRepositoryTriggerTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerTypeDef",
+_OptionalRepositoryTriggerOutputTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerOutputTypeDef",
     {
         "customData": str,
         "branches": List[str],
     },
     total=False,
 )
 
-class RepositoryTriggerTypeDef(
-    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+class RepositoryTriggerOutputTypeDef(
+    _RequiredRepositoryTriggerOutputTypeDef, _OptionalRepositoryTriggerOutputTypeDef
 ):
     pass
 
 ListApprovalRuleTemplatesInputRequestTypeDef = TypedDict(
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
-    "ListApprovalRuleTemplatesOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
     "_RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef = TypedDict(
@@ -1373,43 +1174,14 @@
 
 class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(
     _RequiredListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     _OptionalListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
 ):
     pass
 
-ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
-    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
-    {
-        "approvalRuleTemplateNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBranchesInputListBranchesPaginateTypeDef(
-    _RequiredListBranchesInputListBranchesPaginateTypeDef,
-    _OptionalListBranchesInputListBranchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListBranchesInputRequestTypeDef = TypedDict(
     "_RequiredListBranchesInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListBranchesInputRequestTypeDef = TypedDict(
@@ -1421,45 +1193,14 @@
 )
 
 class ListBranchesInputRequestTypeDef(
     _RequiredListBranchesInputRequestTypeDef, _OptionalListBranchesInputRequestTypeDef
 ):
     pass
 
-ListBranchesOutputTypeDef = TypedDict(
-    "ListBranchesOutputTypeDef",
-    {
-        "branches": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "repositoryName": str,
-    },
-)
-_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
-    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
-    {
-        "authorArn": str,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPullRequestsInputListPullRequestsPaginateTypeDef(
-    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
-    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPullRequestsInputRequestTypeDef = TypedDict(
     "_RequiredListPullRequestsInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListPullRequestsInputRequestTypeDef = TypedDict(
@@ -1474,23 +1215,14 @@
 )
 
 class ListPullRequestsInputRequestTypeDef(
     _RequiredListPullRequestsInputRequestTypeDef, _OptionalListPullRequestsInputRequestTypeDef
 ):
     pass
 
-ListPullRequestsOutputTypeDef = TypedDict(
-    "ListPullRequestsOutputTypeDef",
-    {
-        "pullRequestIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
     "_RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     {
         "approvalRuleTemplateName": str,
     },
 )
 _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef = TypedDict(
@@ -1504,33 +1236,14 @@
 
 class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(
     _RequiredListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     _OptionalListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
 ):
     pass
 
-ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
-    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
-    {
-        "repositoryNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
-    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
-    {
-        "sortBy": SortByEnumType,
-        "order": OrderEnumType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRepositoriesInputRequestTypeDef = TypedDict(
     "ListRepositoriesInputRequestTypeDef",
     {
         "nextToken": str,
         "sortBy": SortByEnumType,
         "order": OrderEnumType,
     },
@@ -1561,23 +1274,14 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1592,41 +1296,14 @@
 
 class MergeBranchesByFastForwardInputRequestTypeDef(
     _RequiredMergeBranchesByFastForwardInputRequestTypeDef,
     _OptionalMergeBranchesByFastForwardInputRequestTypeDef,
 ):
     pass
 
-MergeBranchesByFastForwardOutputTypeDef = TypedDict(
-    "MergeBranchesByFastForwardOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesBySquashOutputTypeDef = TypedDict(
-    "MergeBranchesBySquashOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MergeBranchesByThreeWayOutputTypeDef = TypedDict(
-    "MergeBranchesByThreeWayOutputTypeDef",
-    {
-        "commitId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MergeHunkDetailTypeDef = TypedDict(
     "MergeHunkDetailTypeDef",
     {
         "startLine": int,
         "endLine": int,
         "hunkContent": str,
     },
@@ -1670,24 +1347,14 @@
     {
         "pullRequestId": str,
         "revisionId": str,
         "overrideStatus": OverrideStatusType,
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
 _RequiredPostCommentReplyInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentReplyInputRequestTypeDef",
     {
         "inReplyTo": str,
         "content": str,
     },
 )
@@ -1757,58 +1424,14 @@
 )
 
 class SourceFileSpecifierTypeDef(
     _RequiredSourceFileSpecifierTypeDef, _OptionalSourceFileSpecifierTypeDef
 ):
     pass
 
-_RequiredPutFileInputRequestTypeDef = TypedDict(
-    "_RequiredPutFileInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "branchName": str,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
-        "filePath": str,
-    },
-)
-_OptionalPutFileInputRequestTypeDef = TypedDict(
-    "_OptionalPutFileInputRequestTypeDef",
-    {
-        "fileMode": FileModeTypeEnumType,
-        "parentCommitId": str,
-        "commitMessage": str,
-        "name": str,
-        "email": str,
-    },
-    total=False,
-)
-
-class PutFileInputRequestTypeDef(
-    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
-):
-    pass
-
-PutFileOutputTypeDef = TypedDict(
-    "PutFileOutputTypeDef",
-    {
-        "commitId": str,
-        "blobId": str,
-        "treeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutRepositoryTriggersOutputTypeDef = TypedDict(
-    "PutRepositoryTriggersOutputTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReactionValueFormatsTypeDef = TypedDict(
     "ReactionValueFormatsTypeDef",
     {
         "emoji": str,
         "shortCode": str,
         "unicode": str,
     },
@@ -1820,25 +1443,36 @@
     {
         "trigger": str,
         "failureMessage": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredRepositoryTriggerTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "name": str,
+        "destinationArn": str,
+        "events": Sequence[RepositoryTriggerEventEnumType],
+    },
+)
+_OptionalRepositoryTriggerTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerTypeDef",
+    {
+        "customData": str,
+        "branches": Sequence[str],
     },
+    total=False,
 )
 
+class RepositoryTriggerTypeDef(
+    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+):
+    pass
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1983,175 +1617,424 @@
     "UpdateRepositoryNameInputRequestTypeDef",
     {
         "oldName": str,
         "newName": str,
     },
 )
 
+ApprovalRuleTypeDef = TypedDict(
+    "ApprovalRuleTypeDef",
+    {
+        "approvalRuleId": str,
+        "approvalRuleName": str,
+        "approvalRuleContent": str,
+        "ruleContentSha256": str,
+        "lastModifiedDate": datetime,
+        "creationDate": datetime,
+        "lastModifiedUser": str,
+        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+    },
+    total=False,
+)
+
+BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
+    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+    {
+        "associatedRepositoryNames": List[str],
+        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApprovalRuleTemplateOutputTypeDef = TypedDict(
     "CreateApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUnreferencedMergeCommitOutputTypeDef = TypedDict(
+    "CreateUnreferencedMergeCommitOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "DeleteApprovalRuleTemplateOutputTypeDef",
+    {
+        "approvalRuleTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileOutputTypeDef = TypedDict(
+    "DeleteFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "filePath": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullRequestApprovalRuleOutputTypeDef = TypedDict(
+    "DeletePullRequestApprovalRuleOutputTypeDef",
+    {
+        "approvalRuleId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryOutputTypeDef = TypedDict(
+    "DeleteRepositoryOutputTypeDef",
+    {
+        "repositoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApprovalRuleTemplateOutputTypeDef = TypedDict(
     "GetApprovalRuleTemplateOutputTypeDef",
     {
         "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+GetBlobOutputTypeDef = TypedDict(
+    "GetBlobOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "content": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+GetFileOutputTypeDef = TypedDict(
+    "GetFileOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "commitId": str,
+        "blobId": str,
+        "filePath": str,
+        "fileMode": FileModeTypeEnumType,
+        "fileSize": int,
+        "fileContent": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
-    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+GetMergeCommitOutputTypeDef = TypedDict(
+    "GetMergeCommitOutputTypeDef",
     {
-        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "mergedCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ApprovalRuleTypeDef = TypedDict(
-    "ApprovalRuleTypeDef",
+GetMergeOptionsOutputTypeDef = TypedDict(
+    "GetMergeOptionsOutputTypeDef",
     {
-        "approvalRuleId": str,
-        "approvalRuleName": str,
-        "approvalRuleContent": str,
-        "ruleContentSha256": str,
-        "lastModifiedDate": datetime,
-        "creationDate": datetime,
-        "lastModifiedUser": str,
-        "originApprovalRuleTemplate": OriginApprovalRuleTemplateTypeDef,
+        "mergeOptions": List[MergeOptionTypeEnumType],
+        "sourceCommitId": str,
+        "destinationCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetPullRequestApprovalStatesOutputTypeDef = TypedDict(
     "GetPullRequestApprovalStatesOutputTypeDef",
     {
         "approvals": List[ApprovalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef = TypedDict(
-    "BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef",
+GetPullRequestOverrideStateOutputTypeDef = TypedDict(
+    "GetPullRequestOverrideStateOutputTypeDef",
     {
-        "associatedRepositoryNames": List[str],
-        "errors": List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "overridden": bool,
+        "overrider": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApprovalRuleTemplatesOutputTypeDef = TypedDict(
+    "ListApprovalRuleTemplatesOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef = TypedDict(
+    "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
+    {
+        "approvalRuleTemplateNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBranchesOutputTypeDef = TypedDict(
+    "ListBranchesOutputTypeDef",
+    {
+        "branches": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPullRequestsOutputTypeDef = TypedDict(
+    "ListPullRequestsOutputTypeDef",
+    {
+        "pullRequestIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRepositoriesForApprovalRuleTemplateOutputTypeDef = TypedDict(
+    "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
+    {
+        "repositoryNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByFastForwardOutputTypeDef = TypedDict(
+    "MergeBranchesByFastForwardOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesBySquashOutputTypeDef = TypedDict(
+    "MergeBranchesBySquashOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MergeBranchesByThreeWayOutputTypeDef = TypedDict(
+    "MergeBranchesByThreeWayOutputTypeDef",
+    {
+        "commitId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFileOutputTypeDef = TypedDict(
+    "PutFileOutputTypeDef",
+    {
+        "commitId": str,
+        "blobId": str,
+        "treeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersOutputTypeDef = TypedDict(
+    "PutRepositoryTriggersOutputTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateContentOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateContentOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateDescriptionOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApprovalRuleTemplateNameOutputTypeDef = TypedDict(
+    "UpdateApprovalRuleTemplateNameOutputTypeDef",
+    {
+        "approvalRuleTemplate": ApprovalRuleTemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef = TypedDict(
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     {
         "disassociatedRepositoryNames": List[str],
         "errors": List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetRepositoriesOutputTypeDef = TypedDict(
     "BatchGetRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryMetadataTypeDef],
         "repositoriesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryOutputTypeDef = TypedDict(
     "CreateRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryOutputTypeDef = TypedDict(
     "GetRepositoryOutputTypeDef",
     {
         "repositoryMetadata": RepositoryMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DifferenceTypeDef = TypedDict(
     "DifferenceTypeDef",
     {
         "beforeBlob": BlobMetadataTypeDef,
         "afterBlob": BlobMetadataTypeDef,
         "changeType": ChangeTypeEnumType,
     },
     total=False,
 )
 
+_RequiredPutFileInputRequestTypeDef = TypedDict(
+    "_RequiredPutFileInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+        "fileContent": BlobTypeDef,
+        "filePath": str,
+    },
+)
+_OptionalPutFileInputRequestTypeDef = TypedDict(
+    "_OptionalPutFileInputRequestTypeDef",
+    {
+        "fileMode": FileModeTypeEnumType,
+        "parentCommitId": str,
+        "commitMessage": str,
+        "name": str,
+        "email": str,
+    },
+    total=False,
+)
+
+class PutFileInputRequestTypeDef(
+    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
+):
+    pass
+
+_RequiredReplaceContentEntryTypeDef = TypedDict(
+    "_RequiredReplaceContentEntryTypeDef",
+    {
+        "filePath": str,
+        "replacementType": ReplacementTypeEnumType,
+    },
+)
+_OptionalReplaceContentEntryTypeDef = TypedDict(
+    "_OptionalReplaceContentEntryTypeDef",
+    {
+        "content": BlobTypeDef,
+        "fileMode": FileModeTypeEnumType,
+    },
+    total=False,
+)
+
+class ReplaceContentEntryTypeDef(
+    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
+):
+    pass
+
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBranchOutputTypeDef = TypedDict(
     "GetBranchOutputTypeDef",
     {
         "branch": BranchInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCommentContentOutputTypeDef = TypedDict(
     "DeleteCommentContentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentOutputTypeDef = TypedDict(
     "GetCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PostCommentReplyOutputTypeDef = TypedDict(
     "PostCommentReplyOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCommentOutputTypeDef = TypedDict(
     "UpdateCommentOutputTypeDef",
     {
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentsForComparedCommitTypeDef = TypedDict(
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
@@ -2210,15 +2093,15 @@
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
     "_RequiredPostCommentForPullRequestInputRequestTypeDef",
     {
         "pullRequestId": str,
@@ -2250,15 +2133,15 @@
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
         "location": LocationTypeDef,
         "comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
     {
         "commitId": str,
@@ -2285,33 +2168,23 @@
         "fileModeConflict": bool,
         "objectTypeConflict": bool,
         "mergeOperations": MergeOperationsTypeDef,
     },
     total=False,
 )
 
-ConflictResolutionTypeDef = TypedDict(
-    "ConflictResolutionTypeDef",
-    {
-        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
 CreateCommitOutputTypeDef = TypedDict(
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
         "filesDeleted": List[FileMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePullRequestInputRequestTypeDef = TypedDict(
     "_RequiredCreatePullRequestInputRequestTypeDef",
     {
         "title": str,
@@ -2328,67 +2201,194 @@
 )
 
 class CreatePullRequestInputRequestTypeDef(
     _RequiredCreatePullRequestInputRequestTypeDef, _OptionalCreatePullRequestInputRequestTypeDef
 ):
     pass
 
+_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestId": str,
+    },
+)
+_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
+    {
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef(
+    _RequiredDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    _OptionalDescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitId": str,
+    },
+)
+_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
+    {
+        "beforeCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef(
+    _RequiredGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    _OptionalGetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "pullRequestId": str,
+    },
+)
+_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef = TypedDict(
+    "_OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef(
+    _RequiredGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    _OptionalGetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+):
+    pass
+
+_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "afterCommitSpecifier": str,
+    },
+)
+_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetDifferencesInputGetDifferencesPaginateTypeDef",
+    {
+        "beforeCommitSpecifier": str,
+        "beforePath": str,
+        "afterPath": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetDifferencesInputGetDifferencesPaginateTypeDef(
+    _RequiredGetDifferencesInputGetDifferencesPaginateTypeDef,
+    _OptionalGetDifferencesInputGetDifferencesPaginateTypeDef,
+):
+    pass
+
+_RequiredListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListBranchesInputListBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListBranchesInputListBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBranchesInputListBranchesPaginateTypeDef(
+    _RequiredListBranchesInputListBranchesPaginateTypeDef,
+    _OptionalListBranchesInputListBranchesPaginateTypeDef,
+):
+    pass
+
+_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_RequiredListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "repositoryName": str,
+    },
+)
+_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef = TypedDict(
+    "_OptionalListPullRequestsInputListPullRequestsPaginateTypeDef",
+    {
+        "authorArn": str,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPullRequestsInputListPullRequestsPaginateTypeDef(
+    _RequiredListPullRequestsInputListPullRequestsPaginateTypeDef,
+    _OptionalListPullRequestsInputListPullRequestsPaginateTypeDef,
+):
+    pass
+
+ListRepositoriesInputListRepositoriesPaginateTypeDef = TypedDict(
+    "ListRepositoriesInputListRepositoriesPaginateTypeDef",
+    {
+        "sortBy": SortByEnumType,
+        "order": OrderEnumType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 EvaluatePullRequestApprovalRulesOutputTypeDef = TypedDict(
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     {
         "evaluation": EvaluationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderOutputTypeDef = TypedDict(
     "GetFolderOutputTypeDef",
     {
         "commitId": str,
         "folderPath": str,
         "treeId": str,
         "subFolders": List[FolderTypeDef],
         "files": List[FileTypeDef],
         "symbolicLinks": List[SymbolicLinkTypeDef],
         "subModules": List[SubModuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
-        "triggers": List[RepositoryTriggerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
-    },
-)
-
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
+        "triggers": List[RepositoryTriggerOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRepositoriesOutputTypeDef = TypedDict(
     "ListRepositoriesOutputTypeDef",
     {
         "repositories": List[RepositoryNameIdPairTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
@@ -2429,15 +2429,15 @@
         "filePath": str,
     },
 )
 _OptionalPutFileEntryTypeDef = TypedDict(
     "_OptionalPutFileEntryTypeDef",
     {
         "fileMode": FileModeTypeEnumType,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "fileContent": BlobTypeDef,
         "sourceFile": SourceFileSpecifierTypeDef,
     },
     total=False,
 )
 
 class PutFileEntryTypeDef(_RequiredPutFileEntryTypeDef, _OptionalPutFileEntryTypeDef):
     pass
@@ -2453,88 +2453,213 @@
 )
 
 TestRepositoryTriggersOutputTypeDef = TypedDict(
     "TestRepositoryTriggersOutputTypeDef",
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RepositoryTriggerUnionTypeDef = Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestApprovalRuleContentOutputTypeDef = TypedDict(
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDifferencesOutputTypeDef = TypedDict(
     "GetDifferencesOutputTypeDef",
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConflictResolutionTypeDef = TypedDict(
+    "ConflictResolutionTypeDef",
+    {
+        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
     },
+    total=False,
 )
 
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommentsForPullRequestOutputTypeDef = TypedDict(
     "GetCommentsForPullRequestOutputTypeDef",
     {
         "commentsForPullRequestData": List[CommentsForPullRequestTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetCommitsOutputTypeDef = TypedDict(
     "BatchGetCommitsOutputTypeDef",
     {
         "commits": List[CommitTypeDef],
         "errors": List[BatchGetCommitsErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCommitOutputTypeDef = TypedDict(
     "GetCommitOutputTypeDef",
     {
         "commit": CommitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMergeConflictsOutputTypeDef = TypedDict(
     "GetMergeConflictsOutputTypeDef",
     {
         "mergeable": bool,
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConflictTypeDef = TypedDict(
+    "ConflictTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+    },
+    total=False,
+)
+
+DescribeMergeConflictsOutputTypeDef = TypedDict(
+    "DescribeMergeConflictsOutputTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+        "nextToken": str,
+        "destinationCommitId": str,
+        "sourceCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PullRequestEventTypeDef = TypedDict(
+    "PullRequestEventTypeDef",
+    {
+        "pullRequestId": str,
+        "eventDate": datetime,
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
+        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
+        "pullRequestSourceReferenceUpdatedEventMetadata": (
+            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
+        ),
+        "pullRequestMergedStateChangedEventMetadata": (
+            PullRequestMergedStateChangedEventMetadataTypeDef
+        ),
+        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
+        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
+        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
+    },
+    total=False,
+)
+
+PullRequestTypeDef = TypedDict(
+    "PullRequestTypeDef",
+    {
+        "pullRequestId": str,
+        "title": str,
+        "description": str,
+        "lastActivityDate": datetime,
+        "creationDate": datetime,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "authorArn": str,
+        "pullRequestTargets": List[PullRequestTargetTypeDef],
+        "clientRequestToken": str,
+        "revisionId": str,
+        "approvalRules": List[ApprovalRuleTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateCommitInputRequestTypeDef = TypedDict(
+    "_RequiredCreateCommitInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+    },
+)
+_OptionalCreateCommitInputRequestTypeDef = TypedDict(
+    "_OptionalCreateCommitInputRequestTypeDef",
+    {
+        "parentCommitId": str,
+        "authorName": str,
+        "email": str,
+        "commitMessage": str,
+        "keepEmptyFolders": bool,
+        "putFiles": Sequence[PutFileEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
+class CreateCommitInputRequestTypeDef(
+    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
+):
+    pass
+
+GetCommentReactionsOutputTypeDef = TypedDict(
+    "GetCommentReactionsOutputTypeDef",
+    {
+        "reactionsForComment": List[ReactionForCommentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
     },
 )
 
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
@@ -2673,190 +2798,92 @@
 
 class MergePullRequestByThreeWayInputRequestTypeDef(
     _RequiredMergePullRequestByThreeWayInputRequestTypeDef,
     _OptionalMergePullRequestByThreeWayInputRequestTypeDef,
 ):
     pass
 
-ConflictTypeDef = TypedDict(
-    "ConflictTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-    },
-    total=False,
-)
-
-DescribeMergeConflictsOutputTypeDef = TypedDict(
-    "DescribeMergeConflictsOutputTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-        "nextToken": str,
-        "destinationCommitId": str,
-        "sourceCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PullRequestEventTypeDef = TypedDict(
-    "PullRequestEventTypeDef",
-    {
-        "pullRequestId": str,
-        "eventDate": datetime,
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
-        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
-        "pullRequestSourceReferenceUpdatedEventMetadata": (
-            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
-        ),
-        "pullRequestMergedStateChangedEventMetadata": (
-            PullRequestMergedStateChangedEventMetadataTypeDef
-        ),
-        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
-        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
-        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
-    },
-    total=False,
-)
-
-PullRequestTypeDef = TypedDict(
-    "PullRequestTypeDef",
-    {
-        "pullRequestId": str,
-        "title": str,
-        "description": str,
-        "lastActivityDate": datetime,
-        "creationDate": datetime,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "authorArn": str,
-        "pullRequestTargets": List[PullRequestTargetTypeDef],
-        "clientRequestToken": str,
-        "revisionId": str,
-        "approvalRules": List[ApprovalRuleTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateCommitInputRequestTypeDef = TypedDict(
-    "_RequiredCreateCommitInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "branchName": str,
-    },
-)
-_OptionalCreateCommitInputRequestTypeDef = TypedDict(
-    "_OptionalCreateCommitInputRequestTypeDef",
-    {
-        "parentCommitId": str,
-        "authorName": str,
-        "email": str,
-        "commitMessage": str,
-        "keepEmptyFolders": bool,
-        "putFiles": Sequence[PutFileEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
-class CreateCommitInputRequestTypeDef(
-    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
-):
-    pass
-
-GetCommentReactionsOutputTypeDef = TypedDict(
-    "GetCommentReactionsOutputTypeDef",
-    {
-        "reactionsForComment": List[ReactionForCommentTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
         "sourceCommitId": str,
         "baseCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePullRequestEventsOutputTypeDef = TypedDict(
     "DescribePullRequestEventsOutputTypeDef",
     {
         "pullRequestEvents": List[PullRequestEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePullRequestOutputTypeDef = TypedDict(
     "CreatePullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPullRequestOutputTypeDef = TypedDict(
     "GetPullRequestOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByFastForwardOutputTypeDef = TypedDict(
     "MergePullRequestByFastForwardOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestBySquashOutputTypeDef = TypedDict(
     "MergePullRequestBySquashOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MergePullRequestByThreeWayOutputTypeDef = TypedDict(
     "MergePullRequestByThreeWayOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestDescriptionOutputTypeDef = TypedDict(
     "UpdatePullRequestDescriptionOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestStatusOutputTypeDef = TypedDict(
     "UpdatePullRequestStatusOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePullRequestTitleOutputTypeDef = TypedDict(
     "UpdatePullRequestTitleOutputTypeDef",
     {
         "pullRequest": PullRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/PKG-INFO` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codecommit
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeCommit 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeCommit 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codecommit type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codecommit type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codecommit"></a>
 
 # types-aiobotocore-codecommit
 
 [![PyPI - types-aiobotocore-codecommit](https://img.shields.io/pypi/v/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codecommit.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codecommit)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codecommit?color=blue)](https://pypistats.org/packages/types-aiobotocore-codecommit)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codecommit)](https://pepy.tech/project/types-aiobotocore-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeCommit 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [types-aiobotocore-codecommit docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codecommit/).
 
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
@@ -350,236 +349,239 @@
 )
 
 
 def check_value(value: ApprovalStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codecommit.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codecommit.type_defs import (
     ApprovalRuleEventMetadataTypeDef,
     ApprovalRuleOverriddenEventMetadataTypeDef,
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
     ApprovalStateChangedEventMetadataTypeDef,
     ApprovalTypeDef,
     AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef,
     BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeMergeConflictsErrorTypeDef,
     BatchDescribeMergeConflictsInputRequestTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
+    BlobTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
     LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
-    ReplaceContentEntryTypeDef,
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
-    CreateUnreferencedMergeCommitOutputTypeDef,
     DeleteApprovalRuleTemplateInputRequestTypeDef,
-    DeleteApprovalRuleTemplateOutputTypeDef,
     DeleteBranchInputRequestTypeDef,
     DeleteCommentContentInputRequestTypeDef,
     DeleteFileInputRequestTypeDef,
-    DeleteFileOutputTypeDef,
     DeletePullRequestApprovalRuleInputRequestTypeDef,
-    DeletePullRequestApprovalRuleOutputTypeDef,
     DeleteRepositoryInputRequestTypeDef,
-    DeleteRepositoryOutputTypeDef,
     DescribeMergeConflictsInputRequestTypeDef,
-    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribePullRequestEventsInputRequestTypeDef,
     DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluatePullRequestApprovalRulesInputRequestTypeDef,
     EvaluationTypeDef,
     FileTypeDef,
     FolderTypeDef,
     GetApprovalRuleTemplateInputRequestTypeDef,
     GetBlobInputRequestTypeDef,
-    GetBlobOutputTypeDef,
     GetBranchInputRequestTypeDef,
     GetCommentInputRequestTypeDef,
     GetCommentReactionsInputRequestTypeDef,
-    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForComparedCommitInputRequestTypeDef,
-    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetCommentsForPullRequestInputRequestTypeDef,
     GetCommitInputRequestTypeDef,
-    GetDifferencesInputGetDifferencesPaginateTypeDef,
     GetDifferencesInputRequestTypeDef,
     GetFileInputRequestTypeDef,
-    GetFileOutputTypeDef,
     GetFolderInputRequestTypeDef,
     SubModuleTypeDef,
     SymbolicLinkTypeDef,
     GetMergeCommitInputRequestTypeDef,
-    GetMergeCommitOutputTypeDef,
     GetMergeConflictsInputRequestTypeDef,
     GetMergeOptionsInputRequestTypeDef,
-    GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
-    GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
-    ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
-    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
-    ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
-    ListBranchesOutputTypeDef,
-    ListPullRequestsInputListPullRequestsPaginateTypeDef,
     ListPullRequestsInputRequestTypeDef,
-    ListPullRequestsOutputTypeDef,
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
-    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
-    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
-    MergeBranchesByFastForwardOutputTypeDef,
-    MergeBranchesBySquashOutputTypeDef,
-    MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
     OverridePullRequestApprovalRulesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
-    PutFileInputRequestTypeDef,
-    PutFileOutputTypeDef,
-    PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
-    ResponseMetadataTypeDef,
+    RepositoryTriggerTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
     UpdatePullRequestApprovalRuleContentInputRequestTypeDef,
     UpdatePullRequestApprovalStateInputRequestTypeDef,
     UpdatePullRequestDescriptionInputRequestTypeDef,
     UpdatePullRequestStatusInputRequestTypeDef,
     UpdatePullRequestTitleInputRequestTypeDef,
     UpdateRepositoryDescriptionInputRequestTypeDef,
     UpdateRepositoryNameInputRequestTypeDef,
+    ApprovalRuleTypeDef,
+    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
+    CreateUnreferencedMergeCommitOutputTypeDef,
+    DeleteApprovalRuleTemplateOutputTypeDef,
+    DeleteFileOutputTypeDef,
+    DeletePullRequestApprovalRuleOutputTypeDef,
+    DeleteRepositoryOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetApprovalRuleTemplateOutputTypeDef,
+    GetBlobOutputTypeDef,
+    GetFileOutputTypeDef,
+    GetMergeCommitOutputTypeDef,
+    GetMergeOptionsOutputTypeDef,
+    GetPullRequestApprovalStatesOutputTypeDef,
+    GetPullRequestOverrideStateOutputTypeDef,
+    ListApprovalRuleTemplatesOutputTypeDef,
+    ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
+    ListBranchesOutputTypeDef,
+    ListPullRequestsOutputTypeDef,
+    ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    MergeBranchesByFastForwardOutputTypeDef,
+    MergeBranchesBySquashOutputTypeDef,
+    MergeBranchesByThreeWayOutputTypeDef,
+    PutFileOutputTypeDef,
+    PutRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
-    ApprovalRuleTypeDef,
-    GetPullRequestApprovalStatesOutputTypeDef,
-    BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
+    PutFileInputRequestTypeDef,
+    ReplaceContentEntryTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
     PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
-    ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
+    DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
+    GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
+    GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
+    GetDifferencesInputGetDifferencesPaginateTypeDef,
+    ListBranchesInputListBranchesPaginateTypeDef,
+    ListPullRequestsInputListPullRequestsPaginateTypeDef,
+    ListRepositoriesInputListRepositoriesPaginateTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
+    RepositoryTriggerUnionTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
+    ConflictResolutionTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     GetCommitOutputTypeDef,
     GetMergeConflictsOutputTypeDef,
-    CreateUnreferencedMergeCommitInputRequestTypeDef,
-    MergeBranchesBySquashInputRequestTypeDef,
-    MergeBranchesByThreeWayInputRequestTypeDef,
-    MergePullRequestBySquashInputRequestTypeDef,
-    MergePullRequestByThreeWayInputRequestTypeDef,
     ConflictTypeDef,
     DescribeMergeConflictsOutputTypeDef,
     PullRequestEventTypeDef,
     PullRequestTypeDef,
     CreateCommitInputRequestTypeDef,
     GetCommentReactionsOutputTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
+    CreateUnreferencedMergeCommitInputRequestTypeDef,
+    MergeBranchesBySquashInputRequestTypeDef,
+    MergeBranchesByThreeWayInputRequestTypeDef,
+    MergePullRequestBySquashInputRequestTypeDef,
+    MergePullRequestByThreeWayInputRequestTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     DescribePullRequestEventsOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     GetPullRequestOutputTypeDef,
     MergePullRequestByFastForwardOutputTypeDef,
     MergePullRequestBySquashOutputTypeDef,
     MergePullRequestByThreeWayOutputTypeDef,
     UpdatePullRequestDescriptionOutputTypeDef,
     UpdatePullRequestStatusOutputTypeDef,
     UpdatePullRequestTitleOutputTypeDef,
 )
 
 
-def get_structure() -> ApprovalRuleEventMetadataTypeDef:
+def get_value() -> ApprovalRuleEventMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codecommit-2.5.2/types_aiobotocore_codecommit.egg-info/SOURCES.txt` & `types-aiobotocore-codecommit-2.5.2.post1/types_aiobotocore_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


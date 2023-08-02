# Comparing `tmp/types-aiobotocore-codeguru-reviewer-2.5.2.tar.gz` & `tmp/types-aiobotocore-codeguru-reviewer-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.tar` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codeguru-reviewer-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-07-08 01:43:23.857869 types-aiobotocore-codeguru-reviewer-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.861869 types-aiobotocore-codeguru-reviewer-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.857869 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-07-08 01:27:35.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:33.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-08 01:27:34.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.857869 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16972 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.637625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-08-02 14:52:02.629625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.637625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.621625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.629625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/LICENSE` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeguru-reviewer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-reviewer?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-reviewer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
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
@@ -352,24 +351,25 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguru_reviewer.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
+    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
@@ -379,34 +379,33 @@
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
     EventInfoTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
@@ -421,15 +420,15 @@
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
     CodeReviewTypeTypeDef,
     CreateCodeReviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> KMSKeyDetailsTypeDef:
+def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/README.md` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-reviewer?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-reviewer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
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
@@ -319,24 +319,25 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguru_reviewer.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
+    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
@@ -346,34 +347,33 @@
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
     EventInfoTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
@@ -388,15 +388,15 @@
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
     CodeReviewTypeTypeDef,
     CreateCodeReviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> KMSKeyDetailsTypeDef:
+def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/setup.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-reviewer",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with"
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
-        "aiobotocore codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore codeguru-reviewer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeguru_reviewer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/"
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__init__.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/__main__.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/client.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/literals.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,13 +50,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/paginator.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,13 +47,13 @@
     def paginate(
         self,
         *,
         ProviderTypes: Sequence[ProviderTypeType] = ...,
         States: Sequence[RepositoryAssociationStateType] = ...,
         Names: Sequence[str] = ...,
         Owners: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRepositoryAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer.Paginator.ListRepositoryAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/paginators/#listrepositoryassociationspaginator)
         """
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
-    data: KMSKeyDetailsTypeDef = {...}
+    data: KMSKeyDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -33,14 +33,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "KMSKeyDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
@@ -50,34 +51,33 @@
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
     "EventInfoTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
@@ -100,14 +100,25 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
     },
     total=False,
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
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
@@ -322,22 +333,20 @@
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ProviderTypes": Sequence[ProviderTypeType],
-        "States": Sequence[RepositoryAssociationStateType],
-        "Names": Sequence[str],
-        "Owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRepositoryAssociationsRequestRequestTypeDef = TypedDict(
     "ListRepositoryAssociationsRequestRequestTypeDef",
     {
@@ -369,32 +378,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
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
 PutRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "PutRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": Sequence[ReactionType],
     },
@@ -432,25 +423,14 @@
     {
         "Name": str,
         "ConnectionArn": str,
         "Owner": str,
     },
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -459,14 +439,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
     },
     total=False,
@@ -516,15 +504,15 @@
     pass
 
 
 DescribeRecommendationFeedbackResponseTypeDef = TypedDict(
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
@@ -536,24 +524,36 @@
 )
 
 ListRecommendationFeedbackResponseTypeDef = TypedDict(
     "ListRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedbackSummaries": List[RecommendationFeedbackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    {
+        "ProviderTypes": Sequence[ProviderTypeType],
+        "States": Sequence[RepositoryAssociationStateType],
+        "Names": Sequence[str],
+        "Owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRepositoryAssociationsResponseTypeDef = TypedDict(
     "ListRepositoryAssociationsResponseTypeDef",
     {
         "RepositoryAssociationSummaries": List[RepositoryAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "FilePath": str,
@@ -620,15 +620,15 @@
 
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "RecommendationSummaries": List[RecommendationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateRepositoryRequestRequestTypeDef",
     {
         "Repository": RepositoryTypeDef,
@@ -653,33 +653,33 @@
 
 
 AssociateRepositoryResponseTypeDef = TypedDict(
     "AssociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryAssociationResponseTypeDef = TypedDict(
     "DescribeRepositoryAssociationResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateRepositoryResponseTypeDef = TypedDict(
     "DisassociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
@@ -743,31 +743,31 @@
 )
 
 ListCodeReviewsResponseTypeDef = TypedDict(
     "ListCodeReviewsResponseTypeDef",
     {
         "CodeReviewSummaries": List[CodeReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCodeReviewResponseTypeDef = TypedDict(
     "CreateCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCodeReviewResponseTypeDef = TypedDict(
     "DescribeCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCodeReviewTypeTypeDef = TypedDict(
     "_RequiredCodeReviewTypeTypeDef",
     {
         "RepositoryAnalysis": RepositoryAnalysisTypeDef,
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/type_defs.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
-    data: KMSKeyDetailsTypeDef = {...}
+    data: KMSKeyDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -32,14 +32,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "KMSKeyDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
@@ -49,34 +50,33 @@
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
     "EventInfoTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
@@ -99,14 +99,25 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
     },
     total=False,
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
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
@@ -311,22 +322,20 @@
 
 class ListRecommendationsRequestRequestTypeDef(
     _RequiredListRecommendationsRequestRequestTypeDef,
     _OptionalListRecommendationsRequestRequestTypeDef,
 ):
     pass
 
-ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
-    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ProviderTypes": Sequence[ProviderTypeType],
-        "States": Sequence[RepositoryAssociationStateType],
-        "Names": Sequence[str],
-        "Owners": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRepositoryAssociationsRequestRequestTypeDef = TypedDict(
     "ListRepositoryAssociationsRequestRequestTypeDef",
     {
@@ -358,32 +367,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
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
 PutRecommendationFeedbackRequestRequestTypeDef = TypedDict(
     "PutRecommendationFeedbackRequestRequestTypeDef",
     {
         "CodeReviewArn": str,
         "RecommendationId": str,
         "Reactions": Sequence[ReactionType],
     },
@@ -421,25 +412,14 @@
     {
         "Name": str,
         "ConnectionArn": str,
         "Owner": str,
     },
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -448,14 +428,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
     },
     total=False,
@@ -501,15 +489,15 @@
 ):
     pass
 
 DescribeRecommendationFeedbackResponseTypeDef = TypedDict(
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
@@ -521,24 +509,36 @@
 )
 
 ListRecommendationFeedbackResponseTypeDef = TypedDict(
     "ListRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedbackSummaries": List[RecommendationFeedbackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef = TypedDict(
+    "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
+    {
+        "ProviderTypes": Sequence[ProviderTypeType],
+        "States": Sequence[RepositoryAssociationStateType],
+        "Names": Sequence[str],
+        "Owners": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRepositoryAssociationsResponseTypeDef = TypedDict(
     "ListRepositoryAssociationsResponseTypeDef",
     {
         "RepositoryAssociationSummaries": List[RepositoryAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "FilePath": str,
@@ -603,15 +603,15 @@
     pass
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "RecommendationSummaries": List[RecommendationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateRepositoryRequestRequestTypeDef",
     {
         "Repository": RepositoryTypeDef,
@@ -634,33 +634,33 @@
     pass
 
 AssociateRepositoryResponseTypeDef = TypedDict(
     "AssociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoryAssociationResponseTypeDef = TypedDict(
     "DescribeRepositoryAssociationResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateRepositoryResponseTypeDef = TypedDict(
     "DisassociateRepositoryResponseTypeDef",
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
@@ -724,31 +724,31 @@
 )
 
 ListCodeReviewsResponseTypeDef = TypedDict(
     "ListCodeReviewsResponseTypeDef",
     {
         "CodeReviewSummaries": List[CodeReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCodeReviewResponseTypeDef = TypedDict(
     "CreateCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCodeReviewResponseTypeDef = TypedDict(
     "DescribeCodeReviewResponseTypeDef",
     {
         "CodeReview": CodeReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCodeReviewTypeTypeDef = TypedDict(
     "_RequiredCodeReviewTypeTypeDef",
     {
         "RepositoryAnalysis": RepositoryAnalysisTypeDef,
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer/waiter.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeguru-reviewer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguru-reviewer?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguru-reviewer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguru-reviewer)](https://pepy.tech/project/types-aiobotocore-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruReviewer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
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
@@ -352,24 +351,25 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguru_reviewer.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
+    ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
@@ -379,34 +379,33 @@
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
     EventInfoTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
+    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
@@ -421,15 +420,15 @@
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
     CodeReviewTypeTypeDef,
     CreateCodeReviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> KMSKeyDetailsTypeDef:
+def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


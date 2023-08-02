# Comparing `tmp/types-aiobotocore-wisdom-2.5.2.tar.gz` & `tmp/types-aiobotocore-wisdom-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wisdom-2.5.2.tar", last modified: Sat Jul  8 01:44:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-wisdom-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
```

## Comparing `types-aiobotocore-wisdom-2.5.2.tar` & `types-aiobotocore-wisdom-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.383050 types-aiobotocore-wisdom-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-07-08 01:44:28.383050 types-aiobotocore-wisdom-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:28.383050 types-aiobotocore-wisdom-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:42:36.000000 types-aiobotocore-wisdom-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.383050 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26892 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35592 2023-07-08 01:42:38.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35531 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:37.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.383050 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-07-08 01:44:28.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:44:28.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:28.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:28.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:44:28.000000 types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16488 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26949 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36458 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wisdom-2.5.2/LICENSE` & `types-aiobotocore-wisdom-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2/PKG-INFO` & `types-aiobotocore-wisdom-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wisdom
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore wisdom type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore wisdom type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-wisdom"></a>
 
 # types-aiobotocore-wisdom
 
 [![PyPI - types-aiobotocore-wisdom](https://img.shields.io/pypi/v/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wisdom?color=blue)](https://pypistats.org/packages/types-aiobotocore-wisdom)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectWisdomService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [types-aiobotocore-wisdom docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/).
 
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
@@ -341,30 +340,32 @@
 )
 
 
 def check_value(value: AssistantStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wisdom.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wisdom.type_defs import (
+    AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
+    ResponseMetadataTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
@@ -374,61 +375,62 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
     StartContentUploadRequestRequestTypeDef,
-    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
     CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
-    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
+    StartContentUploadResponseTypeDef,
+    UpdateContentResponseTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
-    CreateKnowledgeBaseRequestRequestTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
+    CreateKnowledgeBaseRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
@@ -446,15 +448,15 @@
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationTypeDef:
+def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wisdom-2.5.2/README.md` & `types-aiobotocore-wisdom-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-wisdom"></a>
 
 # types-aiobotocore-wisdom
 
 [![PyPI - types-aiobotocore-wisdom](https://img.shields.io/pypi/v/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wisdom?color=blue)](https://pypistats.org/packages/types-aiobotocore-wisdom)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectWisdomService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [types-aiobotocore-wisdom docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/).
 
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
@@ -308,30 +308,32 @@
 )
 
 
 def check_value(value: AssistantStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wisdom.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wisdom.type_defs import (
+    AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
+    ResponseMetadataTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
@@ -341,61 +343,62 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
     StartContentUploadRequestRequestTypeDef,
-    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
     CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
-    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
+    StartContentUploadResponseTypeDef,
+    UpdateContentResponseTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
-    CreateKnowledgeBaseRequestRequestTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
+    CreateKnowledgeBaseRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
@@ -413,15 +416,15 @@
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationTypeDef:
+def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wisdom-2.5.2/setup.py` & `types-aiobotocore-wisdom-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wisdom",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with"
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
-    keywords="aiobotocore wisdom type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore wisdom type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_wisdom": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/"
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/__init__.py` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/__init__.pyi` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/__main__.py` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConnectWisdomService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/client.py` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SourceConfigurationTypeDef,
+    SourceConfigurationUnionTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -181,15 +181,15 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: SourceConfigurationTypeDef = ...,
+        sourceConfiguration: SourceConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_knowledge_base)
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/client.pyi` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SourceConfigurationTypeDef,
+    SourceConfigurationUnionTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -171,15 +171,15 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: SourceConfigurationTypeDef = ...,
+        sourceConfiguration: SourceConfigurationUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_knowledge_base)
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/literals.py` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/literals.pyi` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/paginator.py` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,129 +55,120 @@
     "ListContentsPaginator",
     "ListKnowledgeBasesPaginator",
     "QueryAssistantPaginator",
     "SearchContentPaginator",
     "SearchSessionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAssistantAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantassociationspaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssistantAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantassociationspaginator)
         """
 
-
 class ListAssistantsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssistantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantspaginator)
         """
 
-
 class ListContentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listcontentspaginator)
     """
 
     def paginate(
-        self, *, knowledgeBaseId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, knowledgeBaseId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listcontentspaginator)
         """
 
-
 class ListKnowledgeBasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listknowledgebasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKnowledgeBasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listknowledgebasespaginator)
         """
 
-
 class QueryAssistantPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#queryassistantpaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, queryText: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, queryText: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#queryassistantpaginator)
         """
 
-
 class SearchContentPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchcontentpaginator)
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchcontentpaginator)
         """
 
-
 class SearchSessionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchsessionspaginator)
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/paginator.pyi` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,120 +55,129 @@
     "ListContentsPaginator",
     "ListKnowledgeBasesPaginator",
     "QueryAssistantPaginator",
     "SearchContentPaginator",
     "SearchSessionsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAssistantAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantassociationspaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssistantAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantassociationspaginator)
         """
 
+
 class ListAssistantsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssistantsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listassistantspaginator)
         """
 
+
 class ListContentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listcontentspaginator)
     """
 
     def paginate(
-        self, *, knowledgeBaseId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, knowledgeBaseId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listcontentspaginator)
         """
 
+
 class ListKnowledgeBasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listknowledgebasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKnowledgeBasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#listknowledgebasespaginator)
         """
 
+
 class QueryAssistantPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#queryassistantpaginator)
     """
 
     def paginate(
-        self, *, assistantId: str, queryText: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assistantId: str, queryText: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryAssistantResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#queryassistantpaginator)
         """
 
+
 class SearchContentPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchcontentpaginator)
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchcontentpaginator)
         """
 
+
 class SearchSessionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchsessionspaginator)
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/type_defs.py` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for wisdom service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationTypeDef
+    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
 
-    data: AppIntegrationsConfigurationTypeDef = {...}
+    data: AppIntegrationsConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AssistantStatusType,
     ContentStatusType,
     KnowledgeBaseStatusType,
     KnowledgeBaseTypeType,
     RecommendationSourceTypeType,
@@ -31,21 +31,23 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
@@ -55,61 +57,62 @@
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListAssistantsRequestRequestTypeDef",
-    "ListContentsRequestListContentsPaginateTypeDef",
     "ListContentsRequestRequestTypeDef",
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SessionSummaryTypeDef",
     "StartContentUploadRequestRequestTypeDef",
-    "StartContentUploadResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
     "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
-    "UpdateContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
+    "StartContentUploadResponseTypeDef",
+    "UpdateContentResponseTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
+    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
+    "ListContentsRequestListContentsPaginateTypeDef",
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
-    "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
+    "CreateKnowledgeBaseRequestRequestTypeDef",
+    "SourceConfigurationUnionTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
@@ -126,14 +129,36 @@
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
+_RequiredAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAppIntegrationsConfigurationOutputTypeDef",
+    {
+        "appIntegrationArn": str,
+    },
+)
+_OptionalAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAppIntegrationsConfigurationOutputTypeDef",
+    {
+        "objectFields": List[str],
+    },
+    total=False,
+)
+
+
+class AppIntegrationsConfigurationOutputTypeDef(
+    _RequiredAppIntegrationsConfigurationOutputTypeDef,
+    _OptionalAppIntegrationsConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -242,14 +267,25 @@
 )
 
 
 class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
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
+
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -441,36 +477,24 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    {
-        "assistantId": str,
-    },
-)
-_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
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
-class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
-    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssistantAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssistantAssociationsRequestRequestTypeDef",
     {
         "assistantId": str,
     },
 )
 _OptionalListAssistantAssociationsRequestRequestTypeDef = TypedDict(
@@ -486,53 +510,23 @@
 class ListAssistantAssociationsRequestRequestTypeDef(
     _RequiredListAssistantAssociationsRequestRequestTypeDef,
     _OptionalListAssistantAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssistantsRequestRequestTypeDef = TypedDict(
     "ListAssistantsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_RequiredListContentsRequestListContentsPaginateTypeDef",
-    {
-        "knowledgeBaseId": str,
-    },
-)
-_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_OptionalListContentsRequestListContentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListContentsRequestListContentsPaginateTypeDef(
-    _RequiredListContentsRequestListContentsPaginateTypeDef,
-    _OptionalListContentsRequestListContentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListContentsRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 _OptionalListContentsRequestRequestTypeDef = TypedDict(
@@ -547,22 +541,14 @@
 
 class ListContentsRequestRequestTypeDef(
     _RequiredListContentsRequestRequestTypeDef, _OptionalListContentsRequestRequestTypeDef
 ):
     pass
 
 
-ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKnowledgeBasesRequestRequestTypeDef = TypedDict(
     "ListKnowledgeBasesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -571,22 +557,14 @@
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
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
     total=False,
@@ -597,47 +575,14 @@
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
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
-_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "assistantId": str,
-        "queryText": str,
-    },
-)
-_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryAssistantRequestQueryAssistantPaginateTypeDef(
-    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
-    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
-):
-    pass
-
-
 _RequiredQueryAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredQueryAssistantRequestRequestTypeDef",
     {
         "assistantId": str,
         "queryText": str,
     },
 )
@@ -668,25 +613,14 @@
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
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
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
@@ -697,25 +631,14 @@
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
     },
 )
 
-StartContentUploadResponseTypeDef = TypedDict(
-    "StartContentUploadResponseTypeDef",
-    {
-        "headersToInclude": Dict[str, str],
-        "uploadId": str,
-        "url": str,
-        "urlExpiry": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -759,14 +682,22 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "templateUri": str,
     },
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
     total=False,
 )
@@ -879,73 +810,92 @@
     pass
 
 
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContentResponseTypeDef = TypedDict(
     "GetContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateContentResponseTypeDef = TypedDict(
-    "UpdateContentResponseTypeDef",
-    {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContentSummaryResponseTypeDef = TypedDict(
     "GetContentSummaryResponseTypeDef",
     {
         "contentSummary": ContentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListContentsResponseTypeDef = TypedDict(
     "ListContentsResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchContentResponseTypeDef = TypedDict(
     "SearchContentResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContentUploadResponseTypeDef = TypedDict(
+    "StartContentUploadResponseTypeDef",
+    {
+        "headersToInclude": Dict[str, str],
+        "uploadId": str,
+        "url": str,
+        "urlExpiry": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateContentResponseTypeDef = TypedDict(
+    "UpdateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
@@ -957,68 +907,123 @@
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
     },
 )
 
-NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
-    "NotifyRecommendationsReceivedResponseTypeDef",
+_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
-        "recommendationIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assistantId": str,
     },
 )
+_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-RecommendationTriggerDataTypeDef = TypedDict(
-    "RecommendationTriggerDataTypeDef",
+
+class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
+    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+):
+    pass
+
+
+ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     {
-        "query": QueryRecommendationTriggerDataTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SearchSessionsResponseTypeDef = TypedDict(
-    "SearchSessionsResponseTypeDef",
+_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_RequiredListContentsRequestListContentsPaginateTypeDef",
     {
-        "nextToken": str,
-        "sessionSummaries": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "knowledgeBaseId": str,
+    },
+)
+_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_OptionalListContentsRequestListContentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
+
+class ListContentsRequestListContentsPaginateTypeDef(
+    _RequiredListContentsRequestListContentsPaginateTypeDef,
+    _OptionalListContentsRequestListContentsPaginateTypeDef,
+):
+    pass
+
+
+ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     {
-        "knowledgeBaseType": KnowledgeBaseTypeType,
-        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+
+_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
-        "clientToken": str,
-        "description": str,
-        "renderingConfiguration": RenderingConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Mapping[str, str],
+        "assistantId": str,
+        "queryText": str,
+    },
+)
+_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class CreateKnowledgeBaseRequestRequestTypeDef(
-    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
-    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
+class QueryAssistantRequestQueryAssistantPaginateTypeDef(
+    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
+    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
 ):
     pass
 
 
+NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
+    "NotifyRecommendationsReceivedResponseTypeDef",
+    {
+        "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
+        "recommendationIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecommendationTriggerDataTypeDef = TypedDict(
+    "RecommendationTriggerDataTypeDef",
+    {
+        "query": QueryRecommendationTriggerDataTypeDef,
+    },
+    total=False,
+)
+
+SearchSessionsResponseTypeDef = TypedDict(
+    "SearchSessionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "sessionSummaries": List[SessionSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredKnowledgeBaseDataTypeDef = TypedDict(
     "_RequiredKnowledgeBaseDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
@@ -1028,15 +1033,15 @@
 _OptionalKnowledgeBaseDataTypeDef = TypedDict(
     "_OptionalKnowledgeBaseDataTypeDef",
     {
         "description": str,
         "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class KnowledgeBaseDataTypeDef(
@@ -1057,27 +1062,58 @@
 )
 _OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
     "_OptionalKnowledgeBaseSummaryTypeDef",
     {
         "description": str,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class KnowledgeBaseSummaryTypeDef(
     _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
 ):
     pass
 
 
+_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
+    {
+        "knowledgeBaseType": KnowledgeBaseTypeType,
+        "name": str,
+    },
+)
+_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "description": str,
+        "renderingConfiguration": RenderingConfigurationTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "sourceConfiguration": SourceConfigurationTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateKnowledgeBaseRequestRequestTypeDef(
+    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
+    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
+):
+    pass
+
+
+SourceConfigurationUnionTypeDef = Union[
+    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+]
 _RequiredAssistantAssociationDataTypeDef = TypedDict(
     "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
@@ -1126,32 +1162,32 @@
     pass
 
 
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantResponseTypeDef = TypedDict(
     "GetAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantsResponseTypeDef = TypedDict(
     "ListAssistantsResponseTypeDef",
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
@@ -1200,15 +1236,15 @@
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchContentRequestSearchContentPaginateTypeDef = TypedDict(
     "_OptionalSearchContentRequestSearchContentPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchContentRequestSearchContentPaginateTypeDef(
     _RequiredSearchContentRequestSearchContentPaginateTypeDef,
@@ -1246,15 +1282,15 @@
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef = TypedDict(
     "_OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchSessionsRequestSearchSessionsPaginateTypeDef(
     _RequiredSearchSessionsRequestSearchSessionsPaginateTypeDef,
@@ -1274,65 +1310,65 @@
     },
 )
 
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKnowledgeBaseResponseTypeDef = TypedDict(
     "GetKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKnowledgeBaseTemplateUriResponseTypeDef = TypedDict(
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKnowledgeBasesResponseTypeDef = TypedDict(
     "ListKnowledgeBasesResponseTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssistantAssociationResponseTypeDef = TypedDict(
     "CreateAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantAssociationResponseTypeDef = TypedDict(
     "GetAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantAssociationsResponseTypeDef = TypedDict(
     "ListAssistantAssociationsResponseTypeDef",
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRecommendationDataTypeDef = TypedDict(
     "_RequiredRecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
@@ -1377,19 +1413,19 @@
 
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryAssistantResponseTypeDef = TypedDict(
     "QueryAssistantResponseTypeDef",
     {
         "nextToken": str,
         "results": List[ResultDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom/type_defs.pyi` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for wisdom service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationTypeDef
+    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
 
-    data: AppIntegrationsConfigurationTypeDef = {...}
+    data: AppIntegrationsConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AssistantStatusType,
     ContentStatusType,
     KnowledgeBaseStatusType,
     KnowledgeBaseTypeType,
     RecommendationSourceTypeType,
@@ -30,21 +30,23 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
@@ -54,61 +56,62 @@
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListAssistantsRequestRequestTypeDef",
-    "ListContentsRequestListContentsPaginateTypeDef",
     "ListContentsRequestRequestTypeDef",
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SessionSummaryTypeDef",
     "StartContentUploadRequestRequestTypeDef",
-    "StartContentUploadResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
     "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
-    "UpdateContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
+    "StartContentUploadResponseTypeDef",
+    "UpdateContentResponseTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
+    "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
+    "ListContentsRequestListContentsPaginateTypeDef",
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
+    "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
-    "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
+    "CreateKnowledgeBaseRequestRequestTypeDef",
+    "SourceConfigurationUnionTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
@@ -125,14 +128,34 @@
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
+_RequiredAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAppIntegrationsConfigurationOutputTypeDef",
+    {
+        "appIntegrationArn": str,
+    },
+)
+_OptionalAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAppIntegrationsConfigurationOutputTypeDef",
+    {
+        "objectFields": List[str],
+    },
+    total=False,
+)
+
+class AppIntegrationsConfigurationOutputTypeDef(
+    _RequiredAppIntegrationsConfigurationOutputTypeDef,
+    _OptionalAppIntegrationsConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -235,14 +258,25 @@
     },
     total=False,
 )
 
 class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
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
+
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -426,34 +460,24 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
-    {
-        "assistantId": str,
-    },
-)
-_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
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
 
-class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
-    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssistantAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssistantAssociationsRequestRequestTypeDef",
     {
         "assistantId": str,
     },
 )
 _OptionalListAssistantAssociationsRequestRequestTypeDef = TypedDict(
@@ -467,51 +491,23 @@
 
 class ListAssistantAssociationsRequestRequestTypeDef(
     _RequiredListAssistantAssociationsRequestRequestTypeDef,
     _OptionalListAssistantAssociationsRequestRequestTypeDef,
 ):
     pass
 
-ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
-    "ListAssistantsRequestListAssistantsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssistantsRequestRequestTypeDef = TypedDict(
     "ListAssistantsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_RequiredListContentsRequestListContentsPaginateTypeDef",
-    {
-        "knowledgeBaseId": str,
-    },
-)
-_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
-    "_OptionalListContentsRequestListContentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListContentsRequestListContentsPaginateTypeDef(
-    _RequiredListContentsRequestListContentsPaginateTypeDef,
-    _OptionalListContentsRequestListContentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListContentsRequestRequestTypeDef = TypedDict(
     "_RequiredListContentsRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
 )
 _OptionalListContentsRequestRequestTypeDef = TypedDict(
@@ -524,22 +520,14 @@
 )
 
 class ListContentsRequestRequestTypeDef(
     _RequiredListContentsRequestRequestTypeDef, _OptionalListContentsRequestRequestTypeDef
 ):
     pass
 
-ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
-    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKnowledgeBasesRequestRequestTypeDef = TypedDict(
     "ListKnowledgeBasesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -548,22 +536,14 @@
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
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
     total=False,
@@ -574,45 +554,14 @@
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
         "sessionId": str,
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
-_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "assistantId": str,
-        "queryText": str,
-    },
-)
-_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
-    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class QueryAssistantRequestQueryAssistantPaginateTypeDef(
-    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
-    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
-):
-    pass
-
 _RequiredQueryAssistantRequestRequestTypeDef = TypedDict(
     "_RequiredQueryAssistantRequestRequestTypeDef",
     {
         "assistantId": str,
         "queryText": str,
     },
 )
@@ -641,25 +590,14 @@
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
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
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
@@ -670,25 +608,14 @@
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
     },
 )
 
-StartContentUploadResponseTypeDef = TypedDict(
-    "StartContentUploadResponseTypeDef",
-    {
-        "headersToInclude": Dict[str, str],
-        "uploadId": str,
-        "url": str,
-        "urlExpiry": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -730,14 +657,22 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "templateUri": str,
     },
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
     total=False,
 )
@@ -842,73 +777,92 @@
 ):
     pass
 
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContentResponseTypeDef = TypedDict(
     "GetContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateContentResponseTypeDef = TypedDict(
-    "UpdateContentResponseTypeDef",
-    {
-        "content": ContentDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContentSummaryResponseTypeDef = TypedDict(
     "GetContentSummaryResponseTypeDef",
     {
         "contentSummary": ContentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListContentsResponseTypeDef = TypedDict(
     "ListContentsResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchContentResponseTypeDef = TypedDict(
     "SearchContentResponseTypeDef",
     {
         "contentSummaries": List[ContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContentUploadResponseTypeDef = TypedDict(
+    "StartContentUploadResponseTypeDef",
+    {
+        "headersToInclude": Dict[str, str],
+        "uploadId": str,
+        "url": str,
+        "urlExpiry": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateContentResponseTypeDef = TypedDict(
+    "UpdateContentResponseTypeDef",
+    {
+        "content": ContentDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "session": SessionDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
@@ -920,66 +874,117 @@
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
     },
 )
 
-NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
-    "NotifyRecommendationsReceivedResponseTypeDef",
+_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     {
-        "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
-        "recommendationIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assistantId": str,
     },
 )
+_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-RecommendationTriggerDataTypeDef = TypedDict(
-    "RecommendationTriggerDataTypeDef",
+class ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef(
+    _RequiredListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    _OptionalListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+):
+    pass
+
+ListAssistantsRequestListAssistantsPaginateTypeDef = TypedDict(
+    "ListAssistantsRequestListAssistantsPaginateTypeDef",
     {
-        "query": QueryRecommendationTriggerDataTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SearchSessionsResponseTypeDef = TypedDict(
-    "SearchSessionsResponseTypeDef",
+_RequiredListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_RequiredListContentsRequestListContentsPaginateTypeDef",
     {
-        "nextToken": str,
-        "sessionSummaries": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "knowledgeBaseId": str,
+    },
+)
+_OptionalListContentsRequestListContentsPaginateTypeDef = TypedDict(
+    "_OptionalListContentsRequestListContentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
+class ListContentsRequestListContentsPaginateTypeDef(
+    _RequiredListContentsRequestListContentsPaginateTypeDef,
+    _OptionalListContentsRequestListContentsPaginateTypeDef,
+):
+    pass
+
+ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = TypedDict(
+    "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     {
-        "knowledgeBaseType": KnowledgeBaseTypeType,
-        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+
+_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef",
     {
-        "clientToken": str,
-        "description": str,
-        "renderingConfiguration": RenderingConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Mapping[str, str],
+        "assistantId": str,
+        "queryText": str,
+    },
+)
+_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef = TypedDict(
+    "_OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateKnowledgeBaseRequestRequestTypeDef(
-    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
-    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
+class QueryAssistantRequestQueryAssistantPaginateTypeDef(
+    _RequiredQueryAssistantRequestQueryAssistantPaginateTypeDef,
+    _OptionalQueryAssistantRequestQueryAssistantPaginateTypeDef,
 ):
     pass
 
+NotifyRecommendationsReceivedResponseTypeDef = TypedDict(
+    "NotifyRecommendationsReceivedResponseTypeDef",
+    {
+        "errors": List[NotifyRecommendationsReceivedErrorTypeDef],
+        "recommendationIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecommendationTriggerDataTypeDef = TypedDict(
+    "RecommendationTriggerDataTypeDef",
+    {
+        "query": QueryRecommendationTriggerDataTypeDef,
+    },
+    total=False,
+)
+
+SearchSessionsResponseTypeDef = TypedDict(
+    "SearchSessionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "sessionSummaries": List[SessionSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredKnowledgeBaseDataTypeDef = TypedDict(
     "_RequiredKnowledgeBaseDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
@@ -989,15 +994,15 @@
 _OptionalKnowledgeBaseDataTypeDef = TypedDict(
     "_OptionalKnowledgeBaseDataTypeDef",
     {
         "description": str,
         "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class KnowledgeBaseDataTypeDef(
     _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
@@ -1016,25 +1021,54 @@
 )
 _OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
     "_OptionalKnowledgeBaseSummaryTypeDef",
     {
         "description": str,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationTypeDef,
+        "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class KnowledgeBaseSummaryTypeDef(
     _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
 ):
     pass
 
+_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
+    {
+        "knowledgeBaseType": KnowledgeBaseTypeType,
+        "name": str,
+    },
+)
+_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "description": str,
+        "renderingConfiguration": RenderingConfigurationTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "sourceConfiguration": SourceConfigurationTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateKnowledgeBaseRequestRequestTypeDef(
+    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
+    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
+):
+    pass
+
+SourceConfigurationUnionTypeDef = Union[
+    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+]
 _RequiredAssistantAssociationDataTypeDef = TypedDict(
     "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
@@ -1079,32 +1113,32 @@
 ):
     pass
 
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantResponseTypeDef = TypedDict(
     "GetAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantsResponseTypeDef = TypedDict(
     "ListAssistantsResponseTypeDef",
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDocumentTypeDef = TypedDict(
     "_RequiredDocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
@@ -1149,15 +1183,15 @@
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchContentRequestSearchContentPaginateTypeDef = TypedDict(
     "_OptionalSearchContentRequestSearchContentPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchContentRequestSearchContentPaginateTypeDef(
     _RequiredSearchContentRequestSearchContentPaginateTypeDef,
     _OptionalSearchContentRequestSearchContentPaginateTypeDef,
@@ -1191,15 +1225,15 @@
         "assistantId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
 _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef = TypedDict(
     "_OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchSessionsRequestSearchSessionsPaginateTypeDef(
     _RequiredSearchSessionsRequestSearchSessionsPaginateTypeDef,
     _OptionalSearchSessionsRequestSearchSessionsPaginateTypeDef,
@@ -1217,65 +1251,65 @@
     },
 )
 
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKnowledgeBaseResponseTypeDef = TypedDict(
     "GetKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKnowledgeBaseTemplateUriResponseTypeDef = TypedDict(
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKnowledgeBasesResponseTypeDef = TypedDict(
     "ListKnowledgeBasesResponseTypeDef",
     {
         "knowledgeBaseSummaries": List[KnowledgeBaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssistantAssociationResponseTypeDef = TypedDict(
     "CreateAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssistantAssociationResponseTypeDef = TypedDict(
     "GetAssistantAssociationResponseTypeDef",
     {
         "assistantAssociation": AssistantAssociationDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssistantAssociationsResponseTypeDef = TypedDict(
     "ListAssistantAssociationsResponseTypeDef",
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRecommendationDataTypeDef = TypedDict(
     "_RequiredRecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
@@ -1316,19 +1350,19 @@
     pass
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryAssistantResponseTypeDef = TypedDict(
     "QueryAssistantResponseTypeDef",
     {
         "nextToken": str,
         "results": List[ResultDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/PKG-INFO` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wisdom
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore wisdom type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore wisdom type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-wisdom"></a>
 
 # types-aiobotocore-wisdom
 
 [![PyPI - types-aiobotocore-wisdom](https://img.shields.io/pypi/v/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wisdom?color=blue)](https://pypistats.org/packages/types-aiobotocore-wisdom)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectWisdomService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [types-aiobotocore-wisdom docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/).
 
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
@@ -341,30 +340,32 @@
 )
 
 
 def check_value(value: AssistantStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wisdom.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wisdom.type_defs import (
+    AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
+    ResponseMetadataTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionDataTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
@@ -374,61 +375,62 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
-    ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListAssistantsRequestRequestTypeDef,
-    ListContentsRequestListContentsPaginateTypeDef,
     ListContentsRequestRequestTypeDef,
-    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
     NotifyRecommendationsReceivedRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     QueryAssistantRequestRequestTypeDef,
     QueryRecommendationTriggerDataTypeDef,
     RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SessionSummaryTypeDef,
     StartContentUploadRequestRequestTypeDef,
-    StartContentUploadResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContentRequestRequestTypeDef,
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
     CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
-    UpdateContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
+    StartContentUploadResponseTypeDef,
+    UpdateContentResponseTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
+    ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
+    ListAssistantsRequestListAssistantsPaginateTypeDef,
+    ListContentsRequestListContentsPaginateTypeDef,
+    ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
+    QueryAssistantRequestQueryAssistantPaginateTypeDef,
     NotifyRecommendationsReceivedResponseTypeDef,
     RecommendationTriggerDataTypeDef,
     SearchSessionsResponseTypeDef,
-    CreateKnowledgeBaseRequestRequestTypeDef,
     KnowledgeBaseDataTypeDef,
     KnowledgeBaseSummaryTypeDef,
+    CreateKnowledgeBaseRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     AssistantAssociationDataTypeDef,
     AssistantAssociationSummaryTypeDef,
     CreateAssistantResponseTypeDef,
     GetAssistantResponseTypeDef,
     ListAssistantsResponseTypeDef,
     DocumentTypeDef,
     SearchContentRequestRequestTypeDef,
@@ -446,15 +448,15 @@
     RecommendationDataTypeDef,
     ResultDataTypeDef,
     GetRecommendationsResponseTypeDef,
     QueryAssistantResponseTypeDef,
 )
 
 
-def get_structure() -> AppIntegrationsConfigurationTypeDef:
+def get_value() -> AppIntegrationsConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wisdom-2.5.2/types_aiobotocore_wisdom.egg-info/SOURCES.txt` & `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*


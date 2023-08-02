# Comparing `tmp/types-aiobotocore-resiliencehub-2.5.2.tar.gz` & `tmp/types-aiobotocore-resiliencehub-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resiliencehub-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-resiliencehub-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-resiliencehub-2.5.2.tar` & `types-aiobotocore-resiliencehub-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.662768 types-aiobotocore-resiliencehub-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18938 2023-07-08 01:44:11.662768 types-aiobotocore-resiliencehub-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.662768 types-aiobotocore-resiliencehub-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.658768 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41861 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41801 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60903 2023-07-08 01:39:15.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60798 2023-07-08 01:39:15.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:14.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.662768 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18938 2023-07-08 01:44:11.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 01:44:11.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:44:11.000000 types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.637482 types-aiobotocore-resiliencehub-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-02 14:52:52.625482 types-aiobotocore-resiliencehub-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.637482 types-aiobotocore-resiliencehub-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.625482 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41871 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41811 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-08-02 14:47:50.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61091 2023-08-02 14:47:53.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60986 2023-08-02 14:47:53.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:49.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.625482 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:52.000000 types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/LICENSE` & `types-aiobotocore-resiliencehub-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.5.2/PKG-INFO` & `types-aiobotocore-resiliencehub-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resiliencehub
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resiliencehub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resiliencehub type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resiliencehub"></a>
 
 # types-aiobotocore-resiliencehub
 
 [![PyPI - types-aiobotocore-resiliencehub](https://img.shields.io/pypi/v/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resiliencehub?color=blue)](https://pypistats.org/packages/types-aiobotocore-resiliencehub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResilienceHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [types-aiobotocore-resiliencehub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -307,23 +306,24 @@
 )
 
 
 def check_value(value: AlarmTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resiliencehub.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_resiliencehub.type_defs import (
+    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
@@ -333,34 +333,27 @@
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
     DeleteAppRequestRequestTypeDef,
-    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceOutputTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
@@ -369,35 +362,42 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
-    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
-    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishAppVersionResponseTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
@@ -416,16 +416,16 @@
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
+    EksSourceUnionTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
@@ -436,14 +436,15 @@
     ListAppInputSourcesResponseTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
@@ -454,15 +455,15 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> RecommendationItemTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/README.md` & `types-aiobotocore-resiliencehub-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-resiliencehub"></a>
 
 # types-aiobotocore-resiliencehub
 
 [![PyPI - types-aiobotocore-resiliencehub](https://img.shields.io/pypi/v/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resiliencehub?color=blue)](https://pypistats.org/packages/types-aiobotocore-resiliencehub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResilienceHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [types-aiobotocore-resiliencehub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -274,23 +274,24 @@
 )
 
 
 def check_value(value: AlarmTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resiliencehub.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_resiliencehub.type_defs import (
+    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
@@ -300,34 +301,27 @@
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
     DeleteAppRequestRequestTypeDef,
-    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceOutputTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
@@ -336,35 +330,42 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
-    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
-    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishAppVersionResponseTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
@@ -383,16 +384,16 @@
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
+    EksSourceUnionTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
@@ -403,14 +404,15 @@
     ListAppInputSourcesResponseTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
@@ -421,15 +423,15 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> RecommendationItemTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/setup.py` & `types-aiobotocore-resiliencehub-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resiliencehub",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with"
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
-    keywords="aiobotocore resiliencehub type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore resiliencehub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resiliencehub": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/"
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/__main__.py` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResilienceHub 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ResilienceHub 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/client.py` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceTypeDef,
+    EksSourceUnionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
@@ -445,15 +445,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#generate_presigned_url)
         """
 
     async def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[EksSourceTypeDef] = ...,
+        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input sources.
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/client.pyi` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceTypeDef,
+    EksSourceUnionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
@@ -416,15 +416,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/client/#generate_presigned_url)
         """
     async def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[EksSourceTypeDef] = ...,
+        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input sources.
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/literals.py` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/literals.pyi` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/type_defs.py` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for resiliencehub service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_resiliencehub.type_defs import RecommendationItemTypeDef
+    from types_aiobotocore_resiliencehub.type_defs import ResponseMetadataTypeDef
 
-    data: RecommendationItemTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
@@ -51,14 +51,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
@@ -68,34 +69,27 @@
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
-    "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppRequestRequestTypeDef",
-    "DeleteAppResponseTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
-    "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
-    "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    "DescribeAppVersionResponseTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
-    "DescribeAppVersionTemplateResponseTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
@@ -104,35 +98,42 @@
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
-    "PublishAppVersionResponseTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
-    "PutDraftAppVersionTemplateResponseTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
-    "ResolveAppVersionResourcesResponseTypeDef",
     "ResourceErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
+    "DeleteAppAssessmentResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteRecommendationTemplateResponseTypeDef",
+    "DeleteResiliencyPolicyResponseTypeDef",
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    "DescribeAppVersionResponseTypeDef",
+    "DescribeAppVersionTemplateResponseTypeDef",
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PublishAppVersionResponseTypeDef",
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
@@ -151,16 +152,16 @@
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
+    "EksSourceUnionTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
@@ -171,14 +172,15 @@
     "ListAppInputSourcesResponseTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
@@ -188,14 +190,25 @@
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
@@ -500,23 +513,14 @@
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteAppAssessmentResponseTypeDef = TypedDict(
-    "DeleteAppAssessmentResponseTypeDef",
-    {
-        "assessmentArn": str,
-        "assessmentStatus": AssessmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalDeleteAppRequestRequestTypeDef = TypedDict(
@@ -531,22 +535,14 @@
 
 class DeleteAppRequestRequestTypeDef(
     _RequiredDeleteAppRequestRequestTypeDef, _OptionalDeleteAppRequestRequestTypeDef
 ):
     pass
 
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
-    {
-        "appArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -584,23 +580,14 @@
 class DeleteRecommendationTemplateRequestRequestTypeDef(
     _RequiredDeleteRecommendationTemplateRequestRequestTypeDef,
     _OptionalDeleteRecommendationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteRecommendationTemplateResponseTypeDef = TypedDict(
-    "DeleteRecommendationTemplateResponseTypeDef",
-    {
-        "recommendationTemplateArn": str,
-        "status": RecommendationTemplateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -615,22 +602,14 @@
 class DeleteResiliencyPolicyRequestRequestTypeDef(
     _RequiredDeleteResiliencyPolicyRequestRequestTypeDef,
     _OptionalDeleteResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteResiliencyPolicyResponseTypeDef = TypedDict(
-    "DeleteResiliencyPolicyResponseTypeDef",
-    {
-        "policyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppAssessmentRequestRequestTypeDef = TypedDict(
     "DescribeAppAssessmentRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 
@@ -677,77 +656,41 @@
 class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(
     _RequiredDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     _OptionalDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppVersionResponseTypeDef = TypedDict(
-    "DescribeAppVersionResponseTypeDef",
-    {
-        "additionalInfo": Dict[str, List[str]],
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-DescribeAppVersionTemplateResponseTypeDef = TypedDict(
-    "DescribeAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appTemplateBody": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = TypedDict(
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
+    "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "status": ResourceImportStatusTypeType,
-        "statusChangeTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policyArn": str,
     },
 )
 
-DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
-    "DescribeResiliencyPolicyRequestRequestTypeDef",
+EksSourceOutputTypeDef = TypedDict(
+    "EksSourceOutputTypeDef",
     {
-        "policyArn": str,
+        "eksClusterArn": str,
+        "namespaces": List[str],
     },
 )
 
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
@@ -1041,22 +984,14 @@
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
 _RequiredListTestRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListTestRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1127,40 +1062,22 @@
 PublishAppVersionRequestRequestTypeDef = TypedDict(
     "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-PublishAppVersionResponseTypeDef = TypedDict(
-    "PublishAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
 )
 
-PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -1189,63 +1106,32 @@
 class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(
     _RequiredRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
 ):
     pass
 
 
-RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResolveAppVersionResourcesRequestRequestTypeDef = TypedDict(
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-ResolveAppVersionResourcesResponseTypeDef = TypedDict(
-    "ResolveAppVersionResourcesResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceErrorTypeDef = TypedDict(
     "ResourceErrorTypeDef",
     {
         "logicalResourceId": str,
         "physicalResourceId": str,
         "reason": str,
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
 _RequiredStartAppAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartAppAssessmentRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
     },
@@ -1349,21 +1235,145 @@
 
 class UpdateAppVersionRequestRequestTypeDef(
     _RequiredUpdateAppVersionRequestRequestTypeDef, _OptionalUpdateAppVersionRequestRequestTypeDef
 ):
     pass
 
 
+DeleteAppAssessmentResponseTypeDef = TypedDict(
+    "DeleteAppAssessmentResponseTypeDef",
+    {
+        "assessmentArn": str,
+        "assessmentStatus": AssessmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
+    {
+        "appArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRecommendationTemplateResponseTypeDef = TypedDict(
+    "DeleteRecommendationTemplateResponseTypeDef",
+    {
+        "recommendationTemplateArn": str,
+        "status": RecommendationTemplateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResiliencyPolicyResponseTypeDef = TypedDict(
+    "DeleteResiliencyPolicyResponseTypeDef",
+    {
+        "policyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResponseTypeDef = TypedDict(
+    "DescribeAppVersionResponseTypeDef",
+    {
+        "additionalInfo": Dict[str, List[str]],
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionTemplateResponseTypeDef = TypedDict(
+    "DescribeAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appTemplateBody": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "status": ResourceImportStatusTypeType,
+        "statusChangeTime": datetime,
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
+PublishAppVersionResponseTypeDef = TypedDict(
+    "PublishAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolveAppVersionResourcesResponseTypeDef = TypedDict(
+    "ResolveAppVersionResourcesResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateAppVersionResponseTypeDef = TypedDict(
     "UpdateAppVersionResponseTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appArn": str,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAlarmRecommendationTypeDef = TypedDict(
     "_RequiredAlarmRecommendationTypeDef",
     {
         "name": str,
@@ -1493,56 +1503,56 @@
 
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
     "CreateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionAppComponentResponseTypeDef = TypedDict(
     "DeleteAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionAppComponentResponseTypeDef = TypedDict(
     "DescribeAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionAppComponentsResponseTypeDef = TypedDict(
     "ListAppVersionAppComponentsResponseTypeDef",
     {
         "appArn": str,
         "appComponents": List[AppComponentTypeDef],
         "appVersion": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionAppComponentResponseTypeDef = TypedDict(
     "UpdateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppInputSourceTypeDef = TypedDict(
     "_RequiredAppInputSourceTypeDef",
     {
         "importType": ResourceMappingTypeType,
@@ -1591,48 +1601,48 @@
 
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppResponseTypeDef = TypedDict(
     "DescribeAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
@@ -1842,52 +1852,28 @@
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "eksSources": Sequence[EksSourceTypeDef],
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
-
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "eksSources": List[EksSourceTypeDef],
+        "eksSources": List[EksSourceOutputTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2001,69 +1987,69 @@
 )
 
 ListAlarmRecommendationsResponseTypeDef = TypedDict(
     "ListAlarmRecommendationsResponseTypeDef",
     {
         "alarmRecommendations": List[AlarmRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSopRecommendationsResponseTypeDef = TypedDict(
     "ListSopRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "sopRecommendations": List[SopRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestRecommendationsResponseTypeDef = TypedDict(
     "ListTestRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "testRecommendations": List[TestRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppAssessmentsResponseTypeDef = TypedDict(
     "ListAppAssessmentsResponseTypeDef",
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppInputSourceResponseTypeDef = TypedDict(
     "DeleteAppInputSourceResponseTypeDef",
     {
         "appArn": str,
         "appInputSource": AppInputSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInputSourcesResponseTypeDef = TypedDict(
     "ListAppInputSourcesResponseTypeDef",
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
@@ -2072,99 +2058,124 @@
     },
 )
 
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResiliencyPolicyResponseTypeDef = TypedDict(
     "DescribeResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuggestedResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceUnionTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
     },
+    total=False,
 )
 
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
+
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionResourceResponseTypeDef = TypedDict(
     "DeleteAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionResourceResponseTypeDef = TypedDict(
     "DescribeAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourcesResponseTypeDef = TypedDict(
     "ListAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "physicalResources": List[PhysicalResourceTypeDef],
         "resolutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionResourceResponseTypeDef = TypedDict(
     "UpdateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     {
         "appArn": str,
@@ -2174,51 +2185,51 @@
 
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecommendationTemplatesResponseTypeDef = TypedDict(
     "ListRecommendationTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationTemplates": List[RecommendationTemplateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppAssessmentTypeDef = TypedDict(
     "_RequiredAppAssessmentTypeDef",
     {
         "assessmentArn": str,
@@ -2252,26 +2263,26 @@
 
 
 ListAppComponentRecommendationsResponseTypeDef = TypedDict(
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppAssessmentResponseTypeDef = TypedDict(
     "DescribeAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAppAssessmentResponseTypeDef = TypedDict(
     "StartAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub/type_defs.pyi` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for resiliencehub service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_resiliencehub.type_defs import RecommendationItemTypeDef
+    from types_aiobotocore_resiliencehub.type_defs import ResponseMetadataTypeDef
 
-    data: RecommendationItemTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
@@ -50,14 +50,15 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
@@ -67,34 +68,27 @@
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
-    "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppRequestRequestTypeDef",
-    "DeleteAppResponseTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
-    "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
-    "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    "DescribeAppVersionResponseTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
-    "DescribeAppVersionTemplateResponseTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
@@ -103,35 +97,42 @@
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
-    "PublishAppVersionResponseTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
-    "PutDraftAppVersionTemplateResponseTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
-    "ResolveAppVersionResourcesResponseTypeDef",
     "ResourceErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
+    "DeleteAppAssessmentResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteRecommendationTemplateResponseTypeDef",
+    "DeleteResiliencyPolicyResponseTypeDef",
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    "DescribeAppVersionResponseTypeDef",
+    "DescribeAppVersionTemplateResponseTypeDef",
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PublishAppVersionResponseTypeDef",
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
@@ -150,16 +151,16 @@
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
+    "EksSourceUnionTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
@@ -170,14 +171,15 @@
     "ListAppInputSourcesResponseTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
@@ -187,14 +189,25 @@
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
@@ -479,23 +492,14 @@
 
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
-DeleteAppAssessmentResponseTypeDef = TypedDict(
-    "DeleteAppAssessmentResponseTypeDef",
-    {
-        "assessmentArn": str,
-        "assessmentStatus": AssessmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalDeleteAppRequestRequestTypeDef = TypedDict(
@@ -508,22 +512,14 @@
 )
 
 class DeleteAppRequestRequestTypeDef(
     _RequiredDeleteAppRequestRequestTypeDef, _OptionalDeleteAppRequestRequestTypeDef
 ):
     pass
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
-    {
-        "appArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -557,23 +553,14 @@
 
 class DeleteRecommendationTemplateRequestRequestTypeDef(
     _RequiredDeleteRecommendationTemplateRequestRequestTypeDef,
     _OptionalDeleteRecommendationTemplateRequestRequestTypeDef,
 ):
     pass
 
-DeleteRecommendationTemplateResponseTypeDef = TypedDict(
-    "DeleteRecommendationTemplateResponseTypeDef",
-    {
-        "recommendationTemplateArn": str,
-        "status": RecommendationTemplateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -586,22 +573,14 @@
 
 class DeleteResiliencyPolicyRequestRequestTypeDef(
     _RequiredDeleteResiliencyPolicyRequestRequestTypeDef,
     _OptionalDeleteResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteResiliencyPolicyResponseTypeDef = TypedDict(
-    "DeleteResiliencyPolicyResponseTypeDef",
-    {
-        "policyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppAssessmentRequestRequestTypeDef = TypedDict(
     "DescribeAppAssessmentRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 
@@ -646,77 +625,41 @@
 
 class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(
     _RequiredDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     _OptionalDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
 ):
     pass
 
-DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppVersionResponseTypeDef = TypedDict(
-    "DescribeAppVersionResponseTypeDef",
-    {
-        "additionalInfo": Dict[str, List[str]],
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-DescribeAppVersionTemplateResponseTypeDef = TypedDict(
-    "DescribeAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appTemplateBody": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = TypedDict(
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
+    "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "status": ResourceImportStatusTypeType,
-        "statusChangeTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policyArn": str,
     },
 )
 
-DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
-    "DescribeResiliencyPolicyRequestRequestTypeDef",
+EksSourceOutputTypeDef = TypedDict(
+    "EksSourceOutputTypeDef",
     {
-        "policyArn": str,
+        "eksClusterArn": str,
+        "namespaces": List[str],
     },
 )
 
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
@@ -990,22 +933,14 @@
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
 _RequiredListTestRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListTestRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1070,40 +1005,22 @@
 PublishAppVersionRequestRequestTypeDef = TypedDict(
     "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-PublishAppVersionResponseTypeDef = TypedDict(
-    "PublishAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
 )
 
-PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -1130,63 +1047,32 @@
 
 class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(
     _RequiredRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
 ):
     pass
 
-RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResolveAppVersionResourcesRequestRequestTypeDef = TypedDict(
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-ResolveAppVersionResourcesResponseTypeDef = TypedDict(
-    "ResolveAppVersionResourcesResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceErrorTypeDef = TypedDict(
     "ResourceErrorTypeDef",
     {
         "logicalResourceId": str,
         "physicalResourceId": str,
         "reason": str,
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
 _RequiredStartAppAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartAppAssessmentRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
     },
@@ -1282,21 +1168,145 @@
 )
 
 class UpdateAppVersionRequestRequestTypeDef(
     _RequiredUpdateAppVersionRequestRequestTypeDef, _OptionalUpdateAppVersionRequestRequestTypeDef
 ):
     pass
 
+DeleteAppAssessmentResponseTypeDef = TypedDict(
+    "DeleteAppAssessmentResponseTypeDef",
+    {
+        "assessmentArn": str,
+        "assessmentStatus": AssessmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
+    {
+        "appArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRecommendationTemplateResponseTypeDef = TypedDict(
+    "DeleteRecommendationTemplateResponseTypeDef",
+    {
+        "recommendationTemplateArn": str,
+        "status": RecommendationTemplateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResiliencyPolicyResponseTypeDef = TypedDict(
+    "DeleteResiliencyPolicyResponseTypeDef",
+    {
+        "policyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResponseTypeDef = TypedDict(
+    "DescribeAppVersionResponseTypeDef",
+    {
+        "additionalInfo": Dict[str, List[str]],
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionTemplateResponseTypeDef = TypedDict(
+    "DescribeAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appTemplateBody": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "status": ResourceImportStatusTypeType,
+        "statusChangeTime": datetime,
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
+PublishAppVersionResponseTypeDef = TypedDict(
+    "PublishAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolveAppVersionResourcesResponseTypeDef = TypedDict(
+    "ResolveAppVersionResourcesResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateAppVersionResponseTypeDef = TypedDict(
     "UpdateAppVersionResponseTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appArn": str,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAlarmRecommendationTypeDef = TypedDict(
     "_RequiredAlarmRecommendationTypeDef",
     {
         "name": str,
@@ -1418,56 +1428,56 @@
 
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
     "CreateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionAppComponentResponseTypeDef = TypedDict(
     "DeleteAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionAppComponentResponseTypeDef = TypedDict(
     "DescribeAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionAppComponentsResponseTypeDef = TypedDict(
     "ListAppVersionAppComponentsResponseTypeDef",
     {
         "appArn": str,
         "appComponents": List[AppComponentTypeDef],
         "appVersion": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionAppComponentResponseTypeDef = TypedDict(
     "UpdateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppInputSourceTypeDef = TypedDict(
     "_RequiredAppInputSourceTypeDef",
     {
         "importType": ResourceMappingTypeType,
@@ -1512,48 +1522,48 @@
     pass
 
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppResponseTypeDef = TypedDict(
     "DescribeAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
@@ -1749,50 +1759,28 @@
 
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "eksSources": Sequence[EksSourceTypeDef],
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
 ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "eksSources": List[EksSourceTypeDef],
+        "eksSources": List[EksSourceOutputTypeDef],
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -1898,69 +1886,69 @@
 )
 
 ListAlarmRecommendationsResponseTypeDef = TypedDict(
     "ListAlarmRecommendationsResponseTypeDef",
     {
         "alarmRecommendations": List[AlarmRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSopRecommendationsResponseTypeDef = TypedDict(
     "ListSopRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "sopRecommendations": List[SopRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestRecommendationsResponseTypeDef = TypedDict(
     "ListTestRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "testRecommendations": List[TestRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppAssessmentsResponseTypeDef = TypedDict(
     "ListAppAssessmentsResponseTypeDef",
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppInputSourceResponseTypeDef = TypedDict(
     "DeleteAppInputSourceResponseTypeDef",
     {
         "appArn": str,
         "appInputSource": AppInputSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInputSourcesResponseTypeDef = TypedDict(
     "ListAppInputSourcesResponseTypeDef",
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
@@ -1969,99 +1957,122 @@
     },
 )
 
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResiliencyPolicyResponseTypeDef = TypedDict(
     "DescribeResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuggestedResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceUnionTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
     },
+    total=False,
 )
 
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionResourceResponseTypeDef = TypedDict(
     "DeleteAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionResourceResponseTypeDef = TypedDict(
     "DescribeAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourcesResponseTypeDef = TypedDict(
     "ListAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "physicalResources": List[PhysicalResourceTypeDef],
         "resolutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionResourceResponseTypeDef = TypedDict(
     "UpdateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     {
         "appArn": str,
@@ -2071,51 +2082,51 @@
 
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
         "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecommendationTemplatesResponseTypeDef = TypedDict(
     "ListRecommendationTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationTemplates": List[RecommendationTemplateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppAssessmentTypeDef = TypedDict(
     "_RequiredAppAssessmentTypeDef",
     {
         "assessmentArn": str,
@@ -2147,26 +2158,26 @@
     pass
 
 ListAppComponentRecommendationsResponseTypeDef = TypedDict(
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppAssessmentResponseTypeDef = TypedDict(
     "DescribeAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAppAssessmentResponseTypeDef = TypedDict(
     "StartAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/PKG-INFO` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resiliencehub
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResilienceHub 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resiliencehub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resiliencehub type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resiliencehub"></a>
 
 # types-aiobotocore-resiliencehub
 
 [![PyPI - types-aiobotocore-resiliencehub](https://img.shields.io/pypi/v/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resiliencehub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resiliencehub?color=blue)](https://pypistats.org/packages/types-aiobotocore-resiliencehub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resiliencehub)](https://pepy.tech/project/types-aiobotocore-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResilienceHub 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [types-aiobotocore-resiliencehub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -307,23 +306,24 @@
 )
 
 
 def check_value(value: AlarmTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resiliencehub.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_resiliencehub.type_defs import (
+    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
@@ -333,34 +333,27 @@
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
     DeleteAppRequestRequestTypeDef,
-    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceOutputTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
@@ -369,35 +362,42 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
-    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
-    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishAppVersionResponseTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
@@ -416,16 +416,16 @@
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
+    EksSourceUnionTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
@@ -436,14 +436,15 @@
     ListAppInputSourcesResponseTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
@@ -454,15 +455,15 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> RecommendationItemTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resiliencehub-2.5.2/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt` & `types-aiobotocore-resiliencehub-2.5.2.post1/types_aiobotocore_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-inspector-2.5.2.tar.gz` & `tmp/types-aiobotocore-inspector-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-inspector-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-inspector-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-inspector-2.5.2.tar` & `types-aiobotocore-inspector-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.426260 types-aiobotocore-inspector-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19242 2023-07-08 01:43:44.426260 types-aiobotocore-inspector-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.426260 types-aiobotocore-inspector-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.426260 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34033 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33978 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40530 2023-07-08 01:32:15.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-07-08 01:32:15.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:14.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.426260 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19242 2023-07-08 01:43:44.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:44.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:44.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:44.000000 types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.197569 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34033 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33978 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-08-02 14:40:14.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40508 2023-08-02 14:40:14.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40443 2023-08-02 14:40:14.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-inspector-2.5.2/LICENSE` & `types-aiobotocore-inspector-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/PKG-INFO` & `types-aiobotocore-inspector-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Inspector 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Inspector 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore inspector type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore inspector type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-inspector"></a>
 
 # types-aiobotocore-inspector
 
 [![PyPI - types-aiobotocore-inspector](https://img.shields.io/pypi/v/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-inspector?color=blue)](https://pypistats.org/packages/types-aiobotocore-inspector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector)](https://pepy.tech/project/types-aiobotocore-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Inspector 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [types-aiobotocore-inspector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/).
 
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
@@ -358,135 +357,136 @@
 )
 
 
 def check_value(value: AgentHealthCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_inspector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
+    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
-    TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
-    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
-    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
-    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
-    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
+    TimestampTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
+    CreateResourceGroupResponseTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssessmentReportResponseTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
-    AssessmentRunFilterTypeDef,
-    FindingFilterTypeDef,
     AssessmentRunTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
+    TimestampRangeTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
-    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
-    ListAssessmentRunsRequestRequestTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
     DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    AssessmentRunFilterTypeDef,
+    FindingFilterTypeDef,
     FindingTypeDef,
+    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
+    ListAssessmentRunsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-inspector-2.5.2/README.md` & `types-aiobotocore-inspector-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-inspector"></a>
 
 # types-aiobotocore-inspector
 
 [![PyPI - types-aiobotocore-inspector](https://img.shields.io/pypi/v/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-inspector?color=blue)](https://pypistats.org/packages/types-aiobotocore-inspector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector)](https://pepy.tech/project/types-aiobotocore-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Inspector 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [types-aiobotocore-inspector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/).
 
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
@@ -325,135 +325,136 @@
 )
 
 
 def check_value(value: AgentHealthCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_inspector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
+    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
-    TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
-    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
-    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
-    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
-    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
+    TimestampTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
+    CreateResourceGroupResponseTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssessmentReportResponseTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
-    AssessmentRunFilterTypeDef,
-    FindingFilterTypeDef,
     AssessmentRunTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
+    TimestampRangeTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
-    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
-    ListAssessmentRunsRequestRequestTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
     DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    AssessmentRunFilterTypeDef,
+    FindingFilterTypeDef,
     FindingTypeDef,
+    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
+    ListAssessmentRunsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-inspector-2.5.2/setup.py` & `types-aiobotocore-inspector-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-inspector",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Inspector 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore inspector type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore inspector type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_inspector": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/"
```

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/__init__.py` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/__init__.pyi` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/__main__.py` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Inspector 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Inspector 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/client.py` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/client.pyi` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/literals.py` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/literals.pyi` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/paginator.py` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,170 +67,159 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
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
 class ListAssessmentRunAgentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunagentspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
-
 class ListAssessmentRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunspaginator)
         """
 
-
 class ListAssessmentTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
         """
 
-
 class ListAssessmentTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
-
 class ListEventSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listeventsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listeventsubscriptionspaginator)
         """
 
-
 class ListExclusionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listexclusionspaginator)
     """
 
     def paginate(
-        self, *, assessmentRunArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assessmentRunArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExclusionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listexclusionspaginator)
         """
 
-
 class ListFindingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listfindingspaginator)
         """
 
-
 class ListRulesPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listrulespackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRulesPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listrulespackagespaginator)
         """
 
-
 class PreviewAgentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#previewagentspaginator)
     """
 
     def paginate(
-        self, *, previewAgentsArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, previewAgentsArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[PreviewAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#previewagentspaginator)
         """
```

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/paginator.pyi` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,159 +67,170 @@
     "ListEventSubscriptionsPaginator",
     "ListExclusionsPaginator",
     "ListFindingsPaginator",
     "ListRulesPackagesPaginator",
     "PreviewAgentsPaginator",
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
 class ListAssessmentRunAgentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunagentspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArn: str,
         filter: AgentFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentRunAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRunAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunagentspaginator)
         """
 
+
 class ListAssessmentRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTemplateArns: Sequence[str] = ...,
         filter: AssessmentRunFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmentrunspaginator)
         """
 
+
 class ListAssessmentTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         filter: AssessmentTargetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttargetspaginator)
         """
 
+
 class ListAssessmentTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentTargetArns: Sequence[str] = ...,
         filter: AssessmentTemplateFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssessmentTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListAssessmentTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listassessmenttemplatespaginator)
         """
 
+
 class ListEventSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listeventsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listeventsubscriptionspaginator)
         """
 
+
 class ListExclusionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listexclusionspaginator)
     """
 
     def paginate(
-        self, *, assessmentRunArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, assessmentRunArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExclusionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListExclusions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listexclusionspaginator)
         """
 
+
 class ListFindingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         assessmentRunArns: Sequence[str] = ...,
         filter: FindingFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listfindingspaginator)
         """
 
+
 class ListRulesPackagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listrulespackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRulesPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.ListRulesPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#listrulespackagespaginator)
         """
 
+
 class PreviewAgentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#previewagentspaginator)
     """
 
     def paginate(
-        self, *, previewAgentsArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, previewAgentsArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[PreviewAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector.Paginator.PreviewAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/paginators/#previewagentspaginator)
         """
```

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/type_defs.py` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_inspector.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -36,123 +36,123 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
-    "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
     "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
-    "CreateAssessmentTargetResponseTypeDef",
-    "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
-    "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
-    "CreateResourceGroupResponseTypeDef",
     "DeleteAssessmentRunRequestRequestTypeDef",
     "DeleteAssessmentTargetRequestRequestTypeDef",
     "DeleteAssessmentTemplateRequestRequestTypeDef",
     "DescribeAssessmentRunsRequestRequestTypeDef",
     "DescribeAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
     "DescribeExclusionsRequestRequestTypeDef",
     "DescribeFindingsRequestRequestTypeDef",
     "DescribeResourceGroupsRequestRequestTypeDef",
     "DescribeRulesPackagesRequestRequestTypeDef",
     "RulesPackageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionTypeDef",
     "ScopeTypeDef",
     "InspectorServiceAttributesTypeDef",
     "GetAssessmentReportRequestRequestTypeDef",
-    "GetAssessmentReportResponseTypeDef",
     "GetExclusionsPreviewRequestRequestTypeDef",
     "GetTelemetryMetadataRequestRequestTypeDef",
-    "ListAssessmentRunsResponseTypeDef",
-    "ListAssessmentTargetsResponseTypeDef",
-    "ListAssessmentTemplatesResponseTypeDef",
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventSubscriptionsRequestRequestTypeDef",
-    "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListExclusionsRequestRequestTypeDef",
-    "ListExclusionsResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "ListRulesPackagesRequestRequestTypeDef",
-    "ListRulesPackagesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
-    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
-    "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
     "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
+    "CreateAssessmentTargetResponseTypeDef",
+    "CreateAssessmentTemplateResponseTypeDef",
+    "CreateExclusionsPreviewResponseTypeDef",
+    "CreateResourceGroupResponseTypeDef",
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAssessmentReportResponseTypeDef",
+    "ListAssessmentRunsResponseTypeDef",
+    "ListAssessmentTargetsResponseTypeDef",
+    "ListAssessmentTemplatesResponseTypeDef",
+    "ListExclusionsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListRulesPackagesResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
-    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "StartAssessmentRunResponseTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
-    "AssessmentRunFilterTypeDef",
-    "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
     "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
+    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "ListExclusionsRequestListExclusionsPaginateTypeDef",
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
+    "TimestampRangeTypeDef",
     "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    "ListAssessmentRunsRequestRequestTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
     "DescribeResourceGroupsResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
+    "AssessmentRunFilterTypeDef",
+    "FindingFilterTypeDef",
     "FindingTypeDef",
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    "ListAssessmentRunsRequestRequestTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    "ListFindingsRequestRequestTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "key": str,
@@ -162,27 +162,36 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 FailedItemDetailsTypeDef = TypedDict(
     "FailedItemDetailsTypeDef",
     {
         "failureCode": FailedItemErrorCodeType,
         "retryable": bool,
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
 AgentFilterTypeDef = TypedDict(
     "AgentFilterTypeDef",
     {
         "agentHealths": Sequence[AgentHealthType],
         "agentHealthCodes": Sequence[AgentHealthCodeType],
     },
 )
@@ -203,19 +212,17 @@
         "operatingSystem": str,
         "kernelVersion": str,
         "ipv4Address": str,
     },
     total=False,
 )
 
-
 class AgentPreviewTypeDef(_RequiredAgentPreviewTypeDef, _OptionalAgentPreviewTypeDef):
     pass
 
-
 _RequiredTelemetryMetadataTypeDef = TypedDict(
     "_RequiredTelemetryMetadataTypeDef",
     {
         "messageType": str,
         "count": int,
     },
 )
@@ -223,39 +230,28 @@
     "_OptionalTelemetryMetadataTypeDef",
     {
         "dataSize": int,
     },
     total=False,
 )
 
-
 class TelemetryMetadataTypeDef(
     _RequiredTelemetryMetadataTypeDef, _OptionalTelemetryMetadataTypeDef
 ):
     pass
 
-
 DurationRangeTypeDef = TypedDict(
     "DurationRangeTypeDef",
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
 )
 
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "beginDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunNotificationTypeDef = TypedDict(
     "_RequiredAssessmentRunNotificationTypeDef",
     {
         "date": datetime,
         "event": InspectorEventType,
         "error": bool,
     },
@@ -266,21 +262,19 @@
         "message": str,
         "snsTopicArn": str,
         "snsPublishStatusCode": AssessmentRunNotificationSnsStatusCodeType,
     },
     total=False,
 )
 
-
 class AssessmentRunNotificationTypeDef(
     _RequiredAssessmentRunNotificationTypeDef, _OptionalAssessmentRunNotificationTypeDef
 ):
     pass
 
-
 AssessmentRunStateChangeTypeDef = TypedDict(
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
@@ -306,118 +300,78 @@
     "_OptionalAssessmentTargetTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
 )
 _OptionalCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class CreateAssessmentTargetRequestRequestTypeDef(
     _RequiredCreateAssessmentTargetRequestRequestTypeDef,
     _OptionalCreateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-
-CreateAssessmentTargetResponseTypeDef = TypedDict(
-    "CreateAssessmentTargetResponseTypeDef",
-    {
-        "assessmentTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssessmentTemplateResponseTypeDef = TypedDict(
-    "CreateAssessmentTemplateResponseTypeDef",
-    {
-        "assessmentTemplateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "CreateExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 
-CreateExclusionsPreviewResponseTypeDef = TypedDict(
-    "CreateExclusionsPreviewResponseTypeDef",
-    {
-        "previewToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredResourceGroupTagTypeDef = TypedDict(
     "_RequiredResourceGroupTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalResourceGroupTagTypeDef = TypedDict(
     "_OptionalResourceGroupTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class ResourceGroupTagTypeDef(_RequiredResourceGroupTagTypeDef, _OptionalResourceGroupTagTypeDef):
     pass
 
-
-CreateResourceGroupResponseTypeDef = TypedDict(
-    "CreateResourceGroupResponseTypeDef",
-    {
-        "resourceGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAssessmentRunRequestRequestTypeDef = TypedDict(
     "DeleteAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
@@ -452,67 +406,53 @@
 DescribeAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
     },
 )
 
-DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    {
-        "roleArn": str,
-        "valid": bool,
-        "registeredAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeExclusionsRequestRequestTypeDef",
     {
         "exclusionArns": Sequence[str],
     },
 )
 _OptionalDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeExclusionsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeExclusionsRequestRequestTypeDef(
     _RequiredDescribeExclusionsRequestRequestTypeDef,
     _OptionalDescribeExclusionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
     },
 )
 _OptionalDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFindingsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeFindingsRequestRequestTypeDef(
     _RequiredDescribeFindingsRequestRequestTypeDef, _OptionalDescribeFindingsRequestRequestTypeDef
 ):
     pass
 
-
 DescribeResourceGroupsRequestRequestTypeDef = TypedDict(
     "DescribeResourceGroupsRequestRequestTypeDef",
     {
         "resourceGroupArns": Sequence[str],
     },
 )
 
@@ -526,22 +466,20 @@
     "_OptionalDescribeRulesPackagesRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class DescribeRulesPackagesRequestRequestTypeDef(
     _RequiredDescribeRulesPackagesRequestRequestTypeDef,
     _OptionalDescribeRulesPackagesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRulesPackageTypeDef = TypedDict(
     "_RequiredRulesPackageTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "provider": str,
@@ -551,26 +489,17 @@
     "_OptionalRulesPackageTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class RulesPackageTypeDef(_RequiredRulesPackageTypeDef, _OptionalRulesPackageTypeDef):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "event": InspectorEventType,
         "subscribedAt": datetime,
     },
 )
@@ -595,39 +524,28 @@
     {
         "assessmentRunArn": str,
         "rulesPackageArn": str,
     },
     total=False,
 )
 
-
 class InspectorServiceAttributesTypeDef(
     _RequiredInspectorServiceAttributesTypeDef, _OptionalInspectorServiceAttributesTypeDef
 ):
     pass
 
-
 GetAssessmentReportRequestRequestTypeDef = TypedDict(
     "GetAssessmentReportRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
         "reportFileFormat": ReportFileFormatType,
         "reportType": ReportTypeType,
     },
 )
 
-GetAssessmentReportResponseTypeDef = TypedDict(
-    "GetAssessmentReportResponseTypeDef",
-    {
-        "status": ReportStatusType,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
         "previewToken": str,
     },
 )
@@ -637,97 +555,47 @@
         "nextToken": str,
         "maxResults": int,
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
-
 class GetExclusionsPreviewRequestRequestTypeDef(
     _RequiredGetExclusionsPreviewRequestRequestTypeDef,
     _OptionalGetExclusionsPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 GetTelemetryMetadataRequestRequestTypeDef = TypedDict(
     "GetTelemetryMetadataRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
-ListAssessmentRunsResponseTypeDef = TypedDict(
-    "ListAssessmentRunsResponseTypeDef",
-    {
-        "assessmentRunArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTargetsResponseTypeDef = TypedDict(
-    "ListAssessmentTargetsResponseTypeDef",
-    {
-        "assessmentTargetArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTemplatesResponseTypeDef = TypedDict(
-    "ListAssessmentTemplatesResponseTypeDef",
-    {
-        "assessmentTemplateArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "resourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEventSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListEventSubscriptionsRequestRequestTypeDef",
     {
         "resourceArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExclusionsRequestListExclusionsPaginateTypeDef(
-    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
-    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExclusionsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalListExclusionsRequestRequestTypeDef = TypedDict(
@@ -735,65 +603,28 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListExclusionsRequestRequestTypeDef(
     _RequiredListExclusionsRequestRequestTypeDef, _OptionalListExclusionsRequestRequestTypeDef
 ):
     pass
 
-
-ListExclusionsResponseTypeDef = TypedDict(
-    "ListExclusionsResponseTypeDef",
-    {
-        "exclusionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesPackagesRequestRequestTypeDef = TypedDict(
     "ListRulesPackagesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListRulesPackagesResponseTypeDef = TypedDict(
-    "ListRulesPackagesResponseTypeDef",
-    {
-        "rulesPackageArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -811,46 +642,14 @@
     {
         "groupName": str,
         "groupId": str,
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
-_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "previewAgentsArn": str,
-    },
-)
-_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
-    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredPreviewAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredPreviewAgentsRequestRequestTypeDef",
     {
         "previewAgentsArn": str,
     },
 )
 _OptionalPreviewAgentsRequestRequestTypeDef = TypedDict(
@@ -858,21 +657,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class PreviewAgentsRequestRequestTypeDef(
     _RequiredPreviewAgentsRequestRequestTypeDef, _OptionalPreviewAgentsRequestRequestTypeDef
 ):
     pass
 
-
 RegisterCrossAccountAccessRoleRequestRequestTypeDef = TypedDict(
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -880,85 +677,63 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
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
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunName": str,
     },
     total=False,
 )
 
-
 class StartAssessmentRunRequestRequestTypeDef(
     _RequiredStartAssessmentRunRequestRequestTypeDef,
     _OptionalStartAssessmentRunRequestRequestTypeDef,
 ):
     pass
 
-
-StartAssessmentRunResponseTypeDef = TypedDict(
-    "StartAssessmentRunResponseTypeDef",
-    {
-        "assessmentRunArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStopAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStopAssessmentRunRequestRequestTypeDef",
     {
         "stopAction": StopActionType,
     },
     total=False,
 )
 
-
 class StopAssessmentRunRequestRequestTypeDef(
     _RequiredStopAssessmentRunRequestRequestTypeDef, _OptionalStopAssessmentRunRequestRequestTypeDef
 ):
     pass
 
-
 SubscribeToEventRequestRequestTypeDef = TypedDict(
     "SubscribeToEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UnsubscribeFromEventRequestRequestTypeDef = TypedDict(
     "UnsubscribeFromEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -975,22 +750,20 @@
     "_OptionalUpdateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
-
 class UpdateAssessmentTargetRequestRequestTypeDef(
     _RequiredUpdateAssessmentTargetRequestRequestTypeDef,
     _OptionalUpdateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-
 AddAttributesToFindingsRequestRequestTypeDef = TypedDict(
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -1012,21 +785,19 @@
     "_OptionalAssessmentTemplateTypeDef",
     {
         "lastAssessmentRunArn": str,
     },
     total=False,
 )
 
-
 class AssessmentTemplateTypeDef(
     _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
 ):
     pass
 
-
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -1036,60 +807,155 @@
     "_OptionalCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "userAttributesForFindings": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateAssessmentTemplateRequestRequestTypeDef(
     _RequiredCreateAssessmentTemplateRequestRequestTypeDef,
     _OptionalCreateAssessmentTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 AddAttributesToFindingsResponseTypeDef = TypedDict(
     "AddAttributesToFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
-    "RemoveAttributesFromFindingsResponseTypeDef",
+CreateAssessmentTargetResponseTypeDef = TypedDict(
+    "CreateAssessmentTargetResponseTypeDef",
     {
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+CreateAssessmentTemplateResponseTypeDef = TypedDict(
+    "CreateAssessmentTemplateResponseTypeDef",
     {
-        "assessmentRunArn": str,
+        "assessmentTemplateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+
+CreateExclusionsPreviewResponseTypeDef = TypedDict(
+    "CreateExclusionsPreviewResponseTypeDef",
     {
-        "filter": AgentFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "previewToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateResourceGroupResponseTypeDef = TypedDict(
+    "CreateResourceGroupResponseTypeDef",
+    {
+        "resourceGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
-    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-):
-    pass
+DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    {
+        "roleArn": str,
+        "valid": bool,
+        "registeredAt": datetime,
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
+GetAssessmentReportResponseTypeDef = TypedDict(
+    "GetAssessmentReportResponseTypeDef",
+    {
+        "status": ReportStatusType,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListAssessmentRunsResponseTypeDef = TypedDict(
+    "ListAssessmentRunsResponseTypeDef",
+    {
+        "assessmentRunArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTargetsResponseTypeDef = TypedDict(
+    "ListAssessmentTargetsResponseTypeDef",
+    {
+        "assessmentTargetArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTemplatesResponseTypeDef = TypedDict(
+    "ListAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplateArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListExclusionsResponseTypeDef = TypedDict(
+    "ListExclusionsResponseTypeDef",
+    {
+        "exclusionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRulesPackagesResponseTypeDef = TypedDict(
+    "ListRulesPackagesResponseTypeDef",
+    {
+        "rulesPackageArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
+    "RemoveAttributesFromFindingsResponseTypeDef",
+    {
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAssessmentRunResponseTypeDef = TypedDict(
+    "StartAssessmentRunResponseTypeDef",
+    {
+        "assessmentRunArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredListAssessmentRunAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentRunAgentsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -1099,28 +965,26 @@
         "filter": AgentFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssessmentRunAgentsRequestRequestTypeDef(
     _RequiredListAssessmentRunAgentsRequestRequestTypeDef,
     _OptionalListAssessmentRunAgentsRequestRequestTypeDef,
 ):
     pass
 
-
 PreviewAgentsResponseTypeDef = TypedDict(
     "PreviewAgentsResponseTypeDef",
     {
         "agentPreviews": List[AgentPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssessmentRunAgentTypeDef = TypedDict(
     "_RequiredAssessmentRunAgentTypeDef",
     {
         "agentId": str,
@@ -1135,68 +999,37 @@
     {
         "agentHealthDetails": str,
         "autoScalingGroup": str,
     },
     total=False,
 )
 
-
 class AssessmentRunAgentTypeDef(
     _RequiredAssessmentRunAgentTypeDef, _OptionalAssessmentRunAgentTypeDef
 ):
     pass
 
-
 GetTelemetryMetadataResponseTypeDef = TypedDict(
     "GetTelemetryMetadataResponseTypeDef",
     {
         "telemetryMetadata": List[TelemetryMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTemplateFilterTypeDef = TypedDict(
     "AssessmentTemplateFilterTypeDef",
     {
         "namePattern": str,
         "durationRange": DurationRangeTypeDef,
         "rulesPackageArns": Sequence[str],
     },
     total=False,
 )
 
-AssessmentRunFilterTypeDef = TypedDict(
-    "AssessmentRunFilterTypeDef",
-    {
-        "namePattern": str,
-        "states": Sequence[AssessmentRunStateType],
-        "durationRange": DurationRangeTypeDef,
-        "rulesPackageArns": Sequence[str],
-        "startTimeRange": TimestampRangeTypeDef,
-        "completionTimeRange": TimestampRangeTypeDef,
-        "stateChangeTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
-FindingFilterTypeDef = TypedDict(
-    "FindingFilterTypeDef",
-    {
-        "agentIds": Sequence[str],
-        "autoScalingGroups": Sequence[str],
-        "ruleNames": Sequence[str],
-        "severities": Sequence[SeverityType],
-        "rulesPackageArns": Sequence[str],
-        "attributes": Sequence[AttributeTypeDef],
-        "userAttributes": Sequence[AttributeTypeDef],
-        "creationTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunTypeDef = TypedDict(
     "_RequiredAssessmentRunTypeDef",
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
@@ -1216,28 +1049,17 @@
     {
         "startedAt": datetime,
         "completedAt": datetime,
     },
     total=False,
 )
 
-
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
-
-ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    {
-        "filter": AssessmentTargetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAssessmentTargetsRequestRequestTypeDef = TypedDict(
     "ListAssessmentTargetsRequestRequestTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1245,23 +1067,23 @@
 )
 
 DescribeAssessmentTargetsResponseTypeDef = TypedDict(
     "DescribeAssessmentTargetsResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredSetTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1271,22 +1093,20 @@
     "_OptionalSetTagsForResourceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class SetTagsForResourceRequestRequestTypeDef(
     _RequiredSetTagsForResourceRequestRequestTypeDef,
     _OptionalSetTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
@@ -1300,15 +1120,15 @@
 )
 
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "resourceArn": str,
@@ -1330,19 +1150,17 @@
     "_OptionalExclusionPreviewTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
-
 _RequiredExclusionTypeDef = TypedDict(
     "_RequiredExclusionTypeDef",
     {
         "arn": str,
         "title": str,
         "description": str,
         "recommendation": str,
@@ -1353,18 +1171,103 @@
     "_OptionalExclusionTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
+_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "filter": AgentFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
+    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+):
+    pass
+
+ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    {
+        "filter": AssessmentTargetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExclusionsRequestListExclusionsPaginateTypeDef(
+    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
+    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
+):
+    pass
+
+ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "previewAgentsArn": str,
+    },
+)
+_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
+    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+):
+    pass
 
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "networkInterfaceId": str,
         "subnetId": str,
         "vpcId": str,
@@ -1375,38 +1278,47 @@
         "publicIp": str,
         "ipv6Addresses": List[str],
         "securityGroups": List[SecurityGroupTypeDef],
     },
     total=False,
 )
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "beginDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
     "DescribeAssessmentTemplatesResponseTypeDef",
     {
         "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     {
         "assessmentTargetArns": Sequence[str],
         "filter": AssessmentTemplateFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestRequestTypeDef",
     {
@@ -1414,99 +1326,57 @@
         "filter": AssessmentTemplateFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListAssessmentRunsRequestRequestTypeDef = TypedDict(
-    "ListAssessmentRunsRequestRequestTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListFindingsRequestRequestTypeDef = TypedDict(
-    "ListFindingsRequestRequestTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceGroupsResponseTypeDef = TypedDict(
     "DescribeResourceGroupsResponseTypeDef",
     {
         "resourceGroups": List[ResourceGroupTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
     {
         "subscriptions": List[SubscriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExclusionsPreviewResponseTypeDef = TypedDict(
     "GetExclusionsPreviewResponseTypeDef",
     {
         "previewStatus": PreviewStatusType,
         "exclusionPreviews": List[ExclusionPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExclusionsResponseTypeDef = TypedDict(
     "DescribeExclusionsResponseTypeDef",
     {
         "exclusions": Dict[str, ExclusionTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetAttributesTypeDef = TypedDict(
     "_RequiredAssetAttributesTypeDef",
     {
         "schemaVersion": int,
@@ -1522,18 +1392,45 @@
         "ipv4Addresses": List[str],
         "tags": List[TagTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
-
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
+AssessmentRunFilterTypeDef = TypedDict(
+    "AssessmentRunFilterTypeDef",
+    {
+        "namePattern": str,
+        "states": Sequence[AssessmentRunStateType],
+        "durationRange": DurationRangeTypeDef,
+        "rulesPackageArns": Sequence[str],
+        "startTimeRange": TimestampRangeTypeDef,
+        "completionTimeRange": TimestampRangeTypeDef,
+        "stateChangeTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
+FindingFilterTypeDef = TypedDict(
+    "FindingFilterTypeDef",
+    {
+        "agentIds": Sequence[str],
+        "autoScalingGroups": Sequence[str],
+        "ruleNames": Sequence[str],
+        "severities": Sequence[SeverityType],
+        "rulesPackageArns": Sequence[str],
+        "attributes": Sequence[AttributeTypeDef],
+        "userAttributes": Sequence[AttributeTypeDef],
+        "creationTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
         "attributes": List[AttributeTypeDef],
         "userAttributes": List[AttributeTypeDef],
@@ -1557,20 +1454,60 @@
         "numericSeverity": float,
         "confidence": int,
         "indicatorOfCompromise": bool,
     },
     total=False,
 )
 
-
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAssessmentRunsRequestRequestTypeDef = TypedDict(
+    "ListAssessmentRunsRequestRequestTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsRequestRequestTypeDef = TypedDict(
+    "ListFindingsRequestRequestTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
 
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector/type_defs.pyi` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_inspector.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -36,122 +36,124 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
-    "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
     "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
-    "CreateAssessmentTargetResponseTypeDef",
-    "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
-    "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
-    "CreateResourceGroupResponseTypeDef",
     "DeleteAssessmentRunRequestRequestTypeDef",
     "DeleteAssessmentTargetRequestRequestTypeDef",
     "DeleteAssessmentTemplateRequestRequestTypeDef",
     "DescribeAssessmentRunsRequestRequestTypeDef",
     "DescribeAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
     "DescribeExclusionsRequestRequestTypeDef",
     "DescribeFindingsRequestRequestTypeDef",
     "DescribeResourceGroupsRequestRequestTypeDef",
     "DescribeRulesPackagesRequestRequestTypeDef",
     "RulesPackageTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionTypeDef",
     "ScopeTypeDef",
     "InspectorServiceAttributesTypeDef",
     "GetAssessmentReportRequestRequestTypeDef",
-    "GetAssessmentReportResponseTypeDef",
     "GetExclusionsPreviewRequestRequestTypeDef",
     "GetTelemetryMetadataRequestRequestTypeDef",
-    "ListAssessmentRunsResponseTypeDef",
-    "ListAssessmentTargetsResponseTypeDef",
-    "ListAssessmentTemplatesResponseTypeDef",
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEventSubscriptionsRequestRequestTypeDef",
-    "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListExclusionsRequestRequestTypeDef",
-    "ListExclusionsResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "ListRulesPackagesRequestRequestTypeDef",
-    "ListRulesPackagesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
-    "PaginatorConfigTypeDef",
-    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
-    "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
     "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
+    "CreateAssessmentTargetResponseTypeDef",
+    "CreateAssessmentTemplateResponseTypeDef",
+    "CreateExclusionsPreviewResponseTypeDef",
+    "CreateResourceGroupResponseTypeDef",
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAssessmentReportResponseTypeDef",
+    "ListAssessmentRunsResponseTypeDef",
+    "ListAssessmentTargetsResponseTypeDef",
+    "ListAssessmentTemplatesResponseTypeDef",
+    "ListExclusionsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListRulesPackagesResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
-    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "StartAssessmentRunResponseTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
-    "AssessmentRunFilterTypeDef",
-    "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
     "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
+    "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    "ListExclusionsRequestListExclusionsPaginateTypeDef",
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
+    "TimestampRangeTypeDef",
     "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    "ListAssessmentRunsRequestRequestTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
     "DescribeResourceGroupsResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
+    "AssessmentRunFilterTypeDef",
+    "FindingFilterTypeDef",
     "FindingTypeDef",
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    "ListAssessmentRunsRequestRequestTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    "ListFindingsRequestRequestTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "key": str,
@@ -161,25 +163,38 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 FailedItemDetailsTypeDef = TypedDict(
     "FailedItemDetailsTypeDef",
     {
         "failureCode": FailedItemErrorCodeType,
         "retryable": bool,
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
 AgentFilterTypeDef = TypedDict(
     "AgentFilterTypeDef",
     {
         "agentHealths": Sequence[AgentHealthType],
         "agentHealthCodes": Sequence[AgentHealthCodeType],
     },
 )
@@ -200,17 +215,19 @@
         "operatingSystem": str,
         "kernelVersion": str,
         "ipv4Address": str,
     },
     total=False,
 )
 
+
 class AgentPreviewTypeDef(_RequiredAgentPreviewTypeDef, _OptionalAgentPreviewTypeDef):
     pass
 
+
 _RequiredTelemetryMetadataTypeDef = TypedDict(
     "_RequiredTelemetryMetadataTypeDef",
     {
         "messageType": str,
         "count": int,
     },
 )
@@ -218,37 +235,30 @@
     "_OptionalTelemetryMetadataTypeDef",
     {
         "dataSize": int,
     },
     total=False,
 )
 
+
 class TelemetryMetadataTypeDef(
     _RequiredTelemetryMetadataTypeDef, _OptionalTelemetryMetadataTypeDef
 ):
     pass
 
+
 DurationRangeTypeDef = TypedDict(
     "DurationRangeTypeDef",
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
 )
 
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "beginDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunNotificationTypeDef = TypedDict(
     "_RequiredAssessmentRunNotificationTypeDef",
     {
         "date": datetime,
         "event": InspectorEventType,
         "error": bool,
     },
@@ -259,19 +269,21 @@
         "message": str,
         "snsTopicArn": str,
         "snsPublishStatusCode": AssessmentRunNotificationSnsStatusCodeType,
     },
     total=False,
 )
 
+
 class AssessmentRunNotificationTypeDef(
     _RequiredAssessmentRunNotificationTypeDef, _OptionalAssessmentRunNotificationTypeDef
 ):
     pass
 
+
 AssessmentRunStateChangeTypeDef = TypedDict(
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
@@ -297,109 +309,85 @@
     "_OptionalAssessmentTargetTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
     "_OptionalTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
 )
 _OptionalCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class CreateAssessmentTargetRequestRequestTypeDef(
     _RequiredCreateAssessmentTargetRequestRequestTypeDef,
     _OptionalCreateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
-CreateAssessmentTargetResponseTypeDef = TypedDict(
-    "CreateAssessmentTargetResponseTypeDef",
-    {
-        "assessmentTargetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssessmentTemplateResponseTypeDef = TypedDict(
-    "CreateAssessmentTemplateResponseTypeDef",
-    {
-        "assessmentTemplateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "CreateExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 
-CreateExclusionsPreviewResponseTypeDef = TypedDict(
-    "CreateExclusionsPreviewResponseTypeDef",
-    {
-        "previewToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredResourceGroupTagTypeDef = TypedDict(
     "_RequiredResourceGroupTagTypeDef",
     {
         "key": str,
     },
 )
 _OptionalResourceGroupTagTypeDef = TypedDict(
     "_OptionalResourceGroupTagTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class ResourceGroupTagTypeDef(_RequiredResourceGroupTagTypeDef, _OptionalResourceGroupTagTypeDef):
     pass
 
-CreateResourceGroupResponseTypeDef = TypedDict(
-    "CreateResourceGroupResponseTypeDef",
-    {
-        "resourceGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteAssessmentRunRequestRequestTypeDef = TypedDict(
     "DeleteAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -435,63 +423,57 @@
 DescribeAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeAssessmentTemplatesRequestRequestTypeDef",
     {
         "assessmentTemplateArns": Sequence[str],
     },
 )
 
-DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
-    "DescribeCrossAccountAccessRoleResponseTypeDef",
-    {
-        "roleArn": str,
-        "valid": bool,
-        "registeredAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeExclusionsRequestRequestTypeDef",
     {
         "exclusionArns": Sequence[str],
     },
 )
 _OptionalDescribeExclusionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeExclusionsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeExclusionsRequestRequestTypeDef(
     _RequiredDescribeExclusionsRequestRequestTypeDef,
     _OptionalDescribeExclusionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
     },
 )
 _OptionalDescribeFindingsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeFindingsRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeFindingsRequestRequestTypeDef(
     _RequiredDescribeFindingsRequestRequestTypeDef, _OptionalDescribeFindingsRequestRequestTypeDef
 ):
     pass
 
+
 DescribeResourceGroupsRequestRequestTypeDef = TypedDict(
     "DescribeResourceGroupsRequestRequestTypeDef",
     {
         "resourceGroupArns": Sequence[str],
     },
 )
 
@@ -505,20 +487,22 @@
     "_OptionalDescribeRulesPackagesRequestRequestTypeDef",
     {
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class DescribeRulesPackagesRequestRequestTypeDef(
     _RequiredDescribeRulesPackagesRequestRequestTypeDef,
     _OptionalDescribeRulesPackagesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRulesPackageTypeDef = TypedDict(
     "_RequiredRulesPackageTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "provider": str,
@@ -528,23 +512,18 @@
     "_OptionalRulesPackageTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class RulesPackageTypeDef(_RequiredRulesPackageTypeDef, _OptionalRulesPackageTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 EventSubscriptionTypeDef = TypedDict(
     "EventSubscriptionTypeDef",
     {
         "event": InspectorEventType,
         "subscribedAt": datetime,
     },
@@ -570,37 +549,30 @@
     {
         "assessmentRunArn": str,
         "rulesPackageArn": str,
     },
     total=False,
 )
 
+
 class InspectorServiceAttributesTypeDef(
     _RequiredInspectorServiceAttributesTypeDef, _OptionalInspectorServiceAttributesTypeDef
 ):
     pass
 
+
 GetAssessmentReportRequestRequestTypeDef = TypedDict(
     "GetAssessmentReportRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
         "reportFileFormat": ReportFileFormatType,
         "reportType": ReportTypeType,
     },
 )
 
-GetAssessmentReportResponseTypeDef = TypedDict(
-    "GetAssessmentReportResponseTypeDef",
-    {
-        "status": ReportStatusType,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetExclusionsPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetExclusionsPreviewRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
         "previewToken": str,
     },
 )
@@ -610,93 +582,49 @@
         "nextToken": str,
         "maxResults": int,
         "locale": Literal["EN_US"],
     },
     total=False,
 )
 
+
 class GetExclusionsPreviewRequestRequestTypeDef(
     _RequiredGetExclusionsPreviewRequestRequestTypeDef,
     _OptionalGetExclusionsPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 GetTelemetryMetadataRequestRequestTypeDef = TypedDict(
     "GetTelemetryMetadataRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 
-ListAssessmentRunsResponseTypeDef = TypedDict(
-    "ListAssessmentRunsResponseTypeDef",
-    {
-        "assessmentRunArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTargetsResponseTypeDef = TypedDict(
-    "ListAssessmentTargetsResponseTypeDef",
-    {
-        "assessmentTargetArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAssessmentTemplatesResponseTypeDef = TypedDict(
-    "ListAssessmentTemplatesResponseTypeDef",
-    {
-        "assessmentTemplateArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
-    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "resourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEventSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListEventSubscriptionsRequestRequestTypeDef",
     {
         "resourceArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "assessmentRunArn": str,
-    },
-)
-_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
-    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExclusionsRequestListExclusionsPaginateTypeDef(
-    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
-    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExclusionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExclusionsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
 _OptionalListExclusionsRequestRequestTypeDef = TypedDict(
@@ -704,63 +632,30 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListExclusionsRequestRequestTypeDef(
     _RequiredListExclusionsRequestRequestTypeDef, _OptionalListExclusionsRequestRequestTypeDef
 ):
     pass
 
-ListExclusionsResponseTypeDef = TypedDict(
-    "ListExclusionsResponseTypeDef",
-    {
-        "exclusionArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
-    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListRulesPackagesRequestRequestTypeDef = TypedDict(
     "ListRulesPackagesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListRulesPackagesResponseTypeDef = TypedDict(
-    "ListRulesPackagesResponseTypeDef",
-    {
-        "rulesPackageArns": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -778,44 +673,14 @@
     {
         "groupName": str,
         "groupId": str,
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
-_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "previewAgentsArn": str,
-    },
-)
-_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
-    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
-    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
-):
-    pass
-
 _RequiredPreviewAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredPreviewAgentsRequestRequestTypeDef",
     {
         "previewAgentsArn": str,
     },
 )
 _OptionalPreviewAgentsRequestRequestTypeDef = TypedDict(
@@ -823,19 +688,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class PreviewAgentsRequestRequestTypeDef(
     _RequiredPreviewAgentsRequestRequestTypeDef, _OptionalPreviewAgentsRequestRequestTypeDef
 ):
     pass
 
+
 RegisterCrossAccountAccessRoleRequestRequestTypeDef = TypedDict(
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     {
         "roleArn": str,
     },
 )
 
@@ -843,52 +710,35 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
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
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunName": str,
     },
     total=False,
 )
 
+
 class StartAssessmentRunRequestRequestTypeDef(
     _RequiredStartAssessmentRunRequestRequestTypeDef,
     _OptionalStartAssessmentRunRequestRequestTypeDef,
 ):
     pass
 
-StartAssessmentRunResponseTypeDef = TypedDict(
-    "StartAssessmentRunResponseTypeDef",
-    {
-        "assessmentRunArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStopAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStopAssessmentRunRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -896,28 +746,31 @@
     "_OptionalStopAssessmentRunRequestRequestTypeDef",
     {
         "stopAction": StopActionType,
     },
     total=False,
 )
 
+
 class StopAssessmentRunRequestRequestTypeDef(
     _RequiredStopAssessmentRunRequestRequestTypeDef, _OptionalStopAssessmentRunRequestRequestTypeDef
 ):
     pass
 
+
 SubscribeToEventRequestRequestTypeDef = TypedDict(
     "SubscribeToEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UnsubscribeFromEventRequestRequestTypeDef = TypedDict(
     "UnsubscribeFromEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -934,20 +787,22 @@
     "_OptionalUpdateAssessmentTargetRequestRequestTypeDef",
     {
         "resourceGroupArn": str,
     },
     total=False,
 )
 
+
 class UpdateAssessmentTargetRequestRequestTypeDef(
     _RequiredUpdateAssessmentTargetRequestRequestTypeDef,
     _OptionalUpdateAssessmentTargetRequestRequestTypeDef,
 ):
     pass
 
+
 AddAttributesToFindingsRequestRequestTypeDef = TypedDict(
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
@@ -969,19 +824,21 @@
     "_OptionalAssessmentTemplateTypeDef",
     {
         "lastAssessmentRunArn": str,
     },
     total=False,
 )
 
+
 class AssessmentTemplateTypeDef(
     _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
 ):
     pass
 
+
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -991,56 +848,157 @@
     "_OptionalCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "userAttributesForFindings": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateAssessmentTemplateRequestRequestTypeDef(
     _RequiredCreateAssessmentTemplateRequestRequestTypeDef,
     _OptionalCreateAssessmentTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 AddAttributesToFindingsResponseTypeDef = TypedDict(
     "AddAttributesToFindingsResponseTypeDef",
     {
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
-    "RemoveAttributesFromFindingsResponseTypeDef",
+CreateAssessmentTargetResponseTypeDef = TypedDict(
+    "CreateAssessmentTargetResponseTypeDef",
     {
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentTargetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+CreateAssessmentTemplateResponseTypeDef = TypedDict(
+    "CreateAssessmentTemplateResponseTypeDef",
     {
-        "assessmentRunArn": str,
+        "assessmentTemplateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
-    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+
+CreateExclusionsPreviewResponseTypeDef = TypedDict(
+    "CreateExclusionsPreviewResponseTypeDef",
     {
-        "filter": AgentFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "previewToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
-    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
-):
-    pass
+CreateResourceGroupResponseTypeDef = TypedDict(
+    "CreateResourceGroupResponseTypeDef",
+    {
+        "resourceGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCrossAccountAccessRoleResponseTypeDef = TypedDict(
+    "DescribeCrossAccountAccessRoleResponseTypeDef",
+    {
+        "roleArn": str,
+        "valid": bool,
+        "registeredAt": datetime,
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
+GetAssessmentReportResponseTypeDef = TypedDict(
+    "GetAssessmentReportResponseTypeDef",
+    {
+        "status": ReportStatusType,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentRunsResponseTypeDef = TypedDict(
+    "ListAssessmentRunsResponseTypeDef",
+    {
+        "assessmentRunArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTargetsResponseTypeDef = TypedDict(
+    "ListAssessmentTargetsResponseTypeDef",
+    {
+        "assessmentTargetArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentTemplatesResponseTypeDef = TypedDict(
+    "ListAssessmentTemplatesResponseTypeDef",
+    {
+        "assessmentTemplateArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListExclusionsResponseTypeDef = TypedDict(
+    "ListExclusionsResponseTypeDef",
+    {
+        "exclusionArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRulesPackagesResponseTypeDef = TypedDict(
+    "ListRulesPackagesResponseTypeDef",
+    {
+        "rulesPackageArns": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveAttributesFromFindingsResponseTypeDef = TypedDict(
+    "RemoveAttributesFromFindingsResponseTypeDef",
+    {
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAssessmentRunResponseTypeDef = TypedDict(
+    "StartAssessmentRunResponseTypeDef",
+    {
+        "assessmentRunArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredListAssessmentRunAgentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentRunAgentsRequestRequestTypeDef",
     {
         "assessmentRunArn": str,
     },
 )
@@ -1050,26 +1008,28 @@
         "filter": AgentFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssessmentRunAgentsRequestRequestTypeDef(
     _RequiredListAssessmentRunAgentsRequestRequestTypeDef,
     _OptionalListAssessmentRunAgentsRequestRequestTypeDef,
 ):
     pass
 
+
 PreviewAgentsResponseTypeDef = TypedDict(
     "PreviewAgentsResponseTypeDef",
     {
         "agentPreviews": List[AgentPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssessmentRunAgentTypeDef = TypedDict(
     "_RequiredAssessmentRunAgentTypeDef",
     {
         "agentId": str,
@@ -1084,66 +1044,39 @@
     {
         "agentHealthDetails": str,
         "autoScalingGroup": str,
     },
     total=False,
 )
 
+
 class AssessmentRunAgentTypeDef(
     _RequiredAssessmentRunAgentTypeDef, _OptionalAssessmentRunAgentTypeDef
 ):
     pass
 
+
 GetTelemetryMetadataResponseTypeDef = TypedDict(
     "GetTelemetryMetadataResponseTypeDef",
     {
         "telemetryMetadata": List[TelemetryMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTemplateFilterTypeDef = TypedDict(
     "AssessmentTemplateFilterTypeDef",
     {
         "namePattern": str,
         "durationRange": DurationRangeTypeDef,
         "rulesPackageArns": Sequence[str],
     },
     total=False,
 )
 
-AssessmentRunFilterTypeDef = TypedDict(
-    "AssessmentRunFilterTypeDef",
-    {
-        "namePattern": str,
-        "states": Sequence[AssessmentRunStateType],
-        "durationRange": DurationRangeTypeDef,
-        "rulesPackageArns": Sequence[str],
-        "startTimeRange": TimestampRangeTypeDef,
-        "completionTimeRange": TimestampRangeTypeDef,
-        "stateChangeTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
-FindingFilterTypeDef = TypedDict(
-    "FindingFilterTypeDef",
-    {
-        "agentIds": Sequence[str],
-        "autoScalingGroups": Sequence[str],
-        "ruleNames": Sequence[str],
-        "severities": Sequence[SeverityType],
-        "rulesPackageArns": Sequence[str],
-        "attributes": Sequence[AttributeTypeDef],
-        "userAttributes": Sequence[AttributeTypeDef],
-        "creationTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunTypeDef = TypedDict(
     "_RequiredAssessmentRunTypeDef",
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
@@ -1163,25 +1096,18 @@
     {
         "startedAt": datetime,
         "completedAt": datetime,
     },
     total=False,
 )
 
+
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
-ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
-    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
-    {
-        "filter": AssessmentTargetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListAssessmentTargetsRequestRequestTypeDef = TypedDict(
     "ListAssessmentTargetsRequestRequestTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
@@ -1190,23 +1116,23 @@
 )
 
 DescribeAssessmentTargetsResponseTypeDef = TypedDict(
     "DescribeAssessmentTargetsResponseTypeDef",
     {
         "assessmentTargets": List[AssessmentTargetTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredSetTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1216,20 +1142,22 @@
     "_OptionalSetTagsForResourceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class SetTagsForResourceRequestRequestTypeDef(
     _RequiredSetTagsForResourceRequestRequestTypeDef,
     _OptionalSetTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
@@ -1243,15 +1171,15 @@
 )
 
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionTypeDef = TypedDict(
     "SubscriptionTypeDef",
     {
         "resourceArn": str,
@@ -1273,17 +1201,19 @@
     "_OptionalExclusionPreviewTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
+
 _RequiredExclusionTypeDef = TypedDict(
     "_RequiredExclusionTypeDef",
     {
         "arn": str,
         "title": str,
         "description": str,
         "recommendation": str,
@@ -1294,17 +1224,112 @@
     "_OptionalExclusionTypeDef",
     {
         "attributes": List[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
+
+_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef = TypedDict(
+    "_OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
+    {
+        "filter": AgentFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef(
+    _RequiredListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    _OptionalListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+):
+    pass
+
+
+ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
+    "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
+    {
+        "filter": AssessmentTargetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef = TypedDict(
+    "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_RequiredListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "assessmentRunArn": str,
+    },
+)
+_OptionalListExclusionsRequestListExclusionsPaginateTypeDef = TypedDict(
+    "_OptionalListExclusionsRequestListExclusionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExclusionsRequestListExclusionsPaginateTypeDef(
+    _RequiredListExclusionsRequestListExclusionsPaginateTypeDef,
+    _OptionalListExclusionsRequestListExclusionsPaginateTypeDef,
+):
+    pass
+
+
+ListRulesPackagesRequestListRulesPackagesPaginateTypeDef = TypedDict(
+    "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "previewAgentsArn": str,
+    },
+)
+_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef = TypedDict(
+    "_OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class PreviewAgentsRequestPreviewAgentsPaginateTypeDef(
+    _RequiredPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+    _OptionalPreviewAgentsRequestPreviewAgentsPaginateTypeDef,
+):
+    pass
+
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "networkInterfaceId": str,
         "subnetId": str,
         "vpcId": str,
         "privateDnsName": str,
@@ -1314,38 +1339,47 @@
         "publicIp": str,
         "ipv6Addresses": List[str],
         "securityGroups": List[SecurityGroupTypeDef],
     },
     total=False,
 )
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "beginDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
     "DescribeAssessmentTemplatesResponseTypeDef",
     {
         "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     {
         "assessmentTargetArns": Sequence[str],
         "filter": AssessmentTemplateFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAssessmentTemplatesRequestRequestTypeDef = TypedDict(
     "ListAssessmentTemplatesRequestRequestTypeDef",
     {
@@ -1353,99 +1387,57 @@
         "filter": AssessmentTemplateFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListAssessmentRunsRequestRequestTypeDef = TypedDict(
-    "ListAssessmentRunsRequestRequestTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListFindingsRequestRequestTypeDef = TypedDict(
-    "ListFindingsRequestRequestTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceGroupsResponseTypeDef = TypedDict(
     "DescribeResourceGroupsResponseTypeDef",
     {
         "resourceGroups": List[ResourceGroupTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
     {
         "subscriptions": List[SubscriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExclusionsPreviewResponseTypeDef = TypedDict(
     "GetExclusionsPreviewResponseTypeDef",
     {
         "previewStatus": PreviewStatusType,
         "exclusionPreviews": List[ExclusionPreviewTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExclusionsResponseTypeDef = TypedDict(
     "DescribeExclusionsResponseTypeDef",
     {
         "exclusions": Dict[str, ExclusionTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssetAttributesTypeDef = TypedDict(
     "_RequiredAssetAttributesTypeDef",
     {
         "schemaVersion": int,
@@ -1461,17 +1453,48 @@
         "ipv4Addresses": List[str],
         "tags": List[TagTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
+
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
+
+AssessmentRunFilterTypeDef = TypedDict(
+    "AssessmentRunFilterTypeDef",
+    {
+        "namePattern": str,
+        "states": Sequence[AssessmentRunStateType],
+        "durationRange": DurationRangeTypeDef,
+        "rulesPackageArns": Sequence[str],
+        "startTimeRange": TimestampRangeTypeDef,
+        "completionTimeRange": TimestampRangeTypeDef,
+        "stateChangeTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
+FindingFilterTypeDef = TypedDict(
+    "FindingFilterTypeDef",
+    {
+        "agentIds": Sequence[str],
+        "autoScalingGroups": Sequence[str],
+        "ruleNames": Sequence[str],
+        "severities": Sequence[SeverityType],
+        "rulesPackageArns": Sequence[str],
+        "attributes": Sequence[AttributeTypeDef],
+        "userAttributes": Sequence[AttributeTypeDef],
+        "creationTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
         "attributes": List[AttributeTypeDef],
         "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
@@ -1494,18 +1517,62 @@
         "numericSeverity": float,
         "confidence": int,
         "indicatorOfCompromise": bool,
     },
     total=False,
 )
 
+
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+
+ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAssessmentRunsRequestRequestTypeDef = TypedDict(
+    "ListAssessmentRunsRequestRequestTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsRequestRequestTypeDef = TypedDict(
+    "ListFindingsRequestRequestTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/PKG-INFO` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Inspector 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Inspector 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore inspector type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore inspector type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-inspector"></a>
 
 # types-aiobotocore-inspector
 
 [![PyPI - types-aiobotocore-inspector](https://img.shields.io/pypi/v/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-inspector?color=blue)](https://pypistats.org/packages/types-aiobotocore-inspector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector)](https://pepy.tech/project/types-aiobotocore-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Inspector 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [types-aiobotocore-inspector docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector/).
 
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
@@ -358,135 +357,136 @@
 )
 
 
 def check_value(value: AgentHealthCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_inspector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
+    ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
-    TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
-    CreateAssessmentTargetResponseTypeDef,
-    CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
-    CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
-    CreateResourceGroupResponseTypeDef,
     DeleteAssessmentRunRequestRequestTypeDef,
     DeleteAssessmentTargetRequestRequestTypeDef,
     DeleteAssessmentTemplateRequestRequestTypeDef,
     DescribeAssessmentRunsRequestRequestTypeDef,
     DescribeAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTemplatesRequestRequestTypeDef,
-    DescribeCrossAccountAccessRoleResponseTypeDef,
     DescribeExclusionsRequestRequestTypeDef,
     DescribeFindingsRequestRequestTypeDef,
     DescribeResourceGroupsRequestRequestTypeDef,
     DescribeRulesPackagesRequestRequestTypeDef,
     RulesPackageTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventSubscriptionTypeDef,
     ScopeTypeDef,
     InspectorServiceAttributesTypeDef,
     GetAssessmentReportRequestRequestTypeDef,
-    GetAssessmentReportResponseTypeDef,
     GetExclusionsPreviewRequestRequestTypeDef,
     GetTelemetryMetadataRequestRequestTypeDef,
-    ListAssessmentRunsResponseTypeDef,
-    ListAssessmentTargetsResponseTypeDef,
-    ListAssessmentTemplatesResponseTypeDef,
-    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEventSubscriptionsRequestRequestTypeDef,
-    ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListExclusionsRequestRequestTypeDef,
-    ListExclusionsResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     ListRulesPackagesRequestRequestTypeDef,
-    ListRulesPackagesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
-    PaginatorConfigTypeDef,
-    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
-    StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
+    TimestampTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
+    CreateAssessmentTargetResponseTypeDef,
+    CreateAssessmentTemplateResponseTypeDef,
+    CreateExclusionsPreviewResponseTypeDef,
+    CreateResourceGroupResponseTypeDef,
+    DescribeCrossAccountAccessRoleResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAssessmentReportResponseTypeDef,
+    ListAssessmentRunsResponseTypeDef,
+    ListAssessmentTargetsResponseTypeDef,
+    ListAssessmentTemplatesResponseTypeDef,
+    ListExclusionsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListRulesPackagesResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
-    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
-    AssessmentRunFilterTypeDef,
-    FindingFilterTypeDef,
     AssessmentRunTypeDef,
-    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
+    ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
+    ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
+    ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
+    ListExclusionsRequestListExclusionsPaginateTypeDef,
+    ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
+    PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
+    TimestampRangeTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
-    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
-    ListAssessmentRunsRequestRequestTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
     DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    AssessmentRunFilterTypeDef,
+    FindingFilterTypeDef,
     FindingTypeDef,
+    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
+    ListAssessmentRunsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-inspector-2.5.2/types_aiobotocore_inspector.egg-info/SOURCES.txt` & `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*


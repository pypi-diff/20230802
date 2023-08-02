# Comparing `tmp/mypy-boto3-resiliencehub-1.28.16.tar.gz` & `tmp/mypy-boto3-resiliencehub-1.28.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.28.16.tar", last modified: Tue Aug  1 11:37:40 2023, max compression
+gzip compressed data, was "mypy-boto3-resiliencehub-1.28.18.tar", last modified: Wed Aug  2 19:47:54 2023, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.28.16.tar` & `mypy-boto3-resiliencehub-1.28.18.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.264770 mypy-boto3-resiliencehub-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-08-01 11:37:40.260770 mypy-boto3-resiliencehub-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.248770 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39524 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-08-01 11:30:23.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-08-01 11:30:23.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61071 2023-08-01 11:30:24.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60966 2023-08-01 11:30:24.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.260770 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 11:37:40.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:40.264770 mypy-boto3-resiliencehub-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:54.560428 mypy-boto3-resiliencehub-1.28.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-08-02 19:47:54.560428 mypy-boto3-resiliencehub-1.28.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:54.552427 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41553 2023-08-02 19:47:14.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41493 2023-08-02 19:47:14.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-02 19:47:15.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-08-02 19:47:15.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68816 2023-08-02 19:47:16.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68695 2023-08-02 19:47:15.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:47:54.560428 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-08-02 19:47:54.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-02 19:47:54.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:47:54.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:47:54.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 19:47:54.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 19:47:54.000000 mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 19:47:54.560428 mypy-boto3-resiliencehub-1.28.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-02 19:47:13.000000 mypy-boto3-resiliencehub-1.28.18/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/LICENSE` & `mypy-boto3-resiliencehub-1.28.18/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.16/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.18/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.16
-Summary: Type annotations for boto3.ResilienceHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.18
+Summary: Type annotations for boto3.ResilienceHub 1.28.18 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -279,24 +279,31 @@
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_resiliencehub.literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
+    DifferenceTypeType,
     DisruptionTypeType,
+    DriftStatusType,
+    DriftTypeType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -332,18 +339,21 @@
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
     AppSummaryTypeDef,
-    AppTypeDef,
+    EventSubscriptionTypeDef,
+    PermissionModelOutputTypeDef,
     AppVersionSummaryTypeDef,
+    BatchUpdateRecommendationStatusFailedEntryTypeDef,
+    UpdateRecommendationStatusItemTypeDef,
     RecommendationDisruptionComplianceTypeDef,
-    CreateAppRequestRequestTypeDef,
+    PermissionModelTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
@@ -356,22 +366,23 @@
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceOutputTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
+    ListAppAssessmentComplianceDriftsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
     ListAppVersionResourcesRequestRequestTypeDef,
-    ListAppVersionsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
@@ -382,15 +393,14 @@
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
     ResourceErrorTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppResponseTypeDef,
     DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
@@ -403,49 +413,60 @@
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
+    ComplianceDriftTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
     DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DescribeAppResponseTypeDef,
-    UpdateAppResponseTypeDef,
+    AppTypeDef,
     ListAppVersionsResponseTypeDef,
+    BatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     ConfigRecommendationTypeDef,
+    CreateAppRequestRequestTypeDef,
+    PermissionModelUnionTypeDef,
+    UpdateAppRequestRequestTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     EksSourceUnionTypeDef,
+    ListAppVersionsRequestRequestTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DescribeAppResponseTypeDef,
+    UpdateAppResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
+    BatchUpdateRecommendationStatusRequestRequestTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     ImportResourcesToDraftAppVersionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/README.md` & `mypy-boto3-resiliencehub-1.28.18/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -247,24 +247,31 @@
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_resiliencehub.literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
+    DifferenceTypeType,
     DisruptionTypeType,
+    DriftStatusType,
+    DriftTypeType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -300,18 +307,21 @@
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
     AppSummaryTypeDef,
-    AppTypeDef,
+    EventSubscriptionTypeDef,
+    PermissionModelOutputTypeDef,
     AppVersionSummaryTypeDef,
+    BatchUpdateRecommendationStatusFailedEntryTypeDef,
+    UpdateRecommendationStatusItemTypeDef,
     RecommendationDisruptionComplianceTypeDef,
-    CreateAppRequestRequestTypeDef,
+    PermissionModelTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
@@ -324,22 +334,23 @@
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceOutputTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
+    ListAppAssessmentComplianceDriftsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
     ListAppVersionResourcesRequestRequestTypeDef,
-    ListAppVersionsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
@@ -350,15 +361,14 @@
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
     ResourceErrorTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppResponseTypeDef,
     DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
@@ -371,49 +381,60 @@
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
+    ComplianceDriftTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
     DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DescribeAppResponseTypeDef,
-    UpdateAppResponseTypeDef,
+    AppTypeDef,
     ListAppVersionsResponseTypeDef,
+    BatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     ConfigRecommendationTypeDef,
+    CreateAppRequestRequestTypeDef,
+    PermissionModelUnionTypeDef,
+    UpdateAppRequestRequestTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     EksSourceUnionTypeDef,
+    ListAppVersionsRequestRequestTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DescribeAppResponseTypeDef,
+    UpdateAppResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
+    BatchUpdateRecommendationStatusRequestRequestTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     ImportResourcesToDraftAppVersionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__main__.py` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResilienceHub 1.28.16\nVersion:         1.28.16\nBuilder"
+        "Type annotations for boto3.ResilienceHub 1.28.18\nVersion:         1.28.18\nBuilder"
         " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.18")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.py` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
@@ -51,17 +52,19 @@
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
     EksSourceUnionTypeDef,
+    EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -71,25 +74,28 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
+    PermissionModelUnionTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
 __all__ = ("ResilienceHubClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -134,14 +140,27 @@
         """
         Adds the resource mapping for the draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
 
+    def batch_update_recommendation_status(
+        self,
+        *,
+        appArn: str,
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+    ) -> BatchUpdateRecommendationStatusResponseTypeDef:
+        """
+        Enables you to include or exclude one or more operational recommendations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#batch_update_recommendation_status)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#can_paginate)
         """
@@ -157,14 +176,16 @@
     def create_app(
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelUnionTypeDef = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
@@ -466,14 +487,24 @@
         """
         Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_alarm_recommendations)
         """
 
+    def list_app_assessment_compliance_drifts(
+        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListAppAssessmentComplianceDriftsResponseTypeDef:
+        """
+        List of compliance drifts that were detected while running an assessment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessment_compliance_drifts)
+        """
+
     def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
@@ -552,15 +583,21 @@
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_resources)
         """
 
     def list_app_versions(
-        self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
+        self,
+        *,
+        appArn: str,
+        endTime: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        startTime: TimestampTypeDef = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_versions)
         """
@@ -654,15 +691,17 @@
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_unsupported_app_version_resources)
         """
 
-    def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
+    def publish_app_version(
+        self, *, appArn: str, versionName: str = ...
+    ) -> PublishAppVersionResponseTypeDef:
         """
         Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#publish_app_version)
         """
 
@@ -740,14 +779,16 @@
     def update_app(
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelUnionTypeDef = ...,
         policyArn: str = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app)
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.pyi` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStrategyTypeType,
     TemplateFormatType,
 )
 from .type_defs import (
     AddDraftAppVersionResourceMappingsResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
@@ -51,17 +52,19 @@
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
     EksSourceUnionTypeDef,
+    EventSubscriptionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
     ListAppsResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
@@ -71,25 +74,28 @@
     ListResiliencyPoliciesResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
     LogicalResourceIdTypeDef,
+    PermissionModelUnionTypeDef,
     PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateResponseTypeDef,
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     ResourceMappingTypeDef,
     StartAppAssessmentResponseTypeDef,
     TerraformSourceTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
 )
 
 __all__ = ("ResilienceHubClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -129,14 +135,26 @@
     ) -> AddDraftAppVersionResourceMappingsResponseTypeDef:
         """
         Adds the resource mapping for the draft application version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.add_draft_app_version_resource_mappings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#add_draft_app_version_resource_mappings)
         """
+    def batch_update_recommendation_status(
+        self,
+        *,
+        appArn: str,
+        requestEntries: Sequence[UpdateRecommendationStatusRequestEntryTypeDef]
+    ) -> BatchUpdateRecommendationStatusResponseTypeDef:
+        """
+        Enables you to include or exclude one or more operational recommendations.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.batch_update_recommendation_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#batch_update_recommendation_status)
+        """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#can_paginate)
         """
@@ -150,14 +168,16 @@
     def create_app(
         self,
         *,
         name: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clientToken: str = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelUnionTypeDef = ...,
         policyArn: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.create_app)
@@ -435,14 +455,23 @@
     ) -> ListAlarmRecommendationsResponseTypeDef:
         """
         Lists the alarm recommendations for an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_alarm_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_alarm_recommendations)
         """
+    def list_app_assessment_compliance_drifts(
+        self, *, assessmentArn: str, maxResults: int = ..., nextToken: str = ...
+    ) -> ListAppAssessmentComplianceDriftsResponseTypeDef:
+        """
+        List of compliance drifts that were detected while running an assessment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_assessment_compliance_drifts)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_assessment_compliance_drifts)
+        """
     def list_app_assessments(
         self,
         *,
         appArn: str = ...,
         assessmentName: str = ...,
         assessmentStatus: Sequence[AssessmentStatusType] = ...,
         complianceStatus: ComplianceStatusType = ...,
@@ -514,15 +543,21 @@
         """
         Lists all the resources in an Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_version_resources)
         """
     def list_app_versions(
-        self, *, appArn: str, maxResults: int = ..., nextToken: str = ...
+        self,
+        *,
+        appArn: str,
+        endTime: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        startTime: TimestampTypeDef = ...
     ) -> ListAppVersionsResponseTypeDef:
         """
         Lists the different versions for the Resilience Hub applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_app_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_app_versions)
         """
@@ -607,15 +642,17 @@
     ) -> ListUnsupportedAppVersionResourcesResponseTypeDef:
         """
         Lists the resources that are not currently supported in Resilience Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.list_unsupported_app_version_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#list_unsupported_app_version_resources)
         """
-    def publish_app_version(self, *, appArn: str) -> PublishAppVersionResponseTypeDef:
+    def publish_app_version(
+        self, *, appArn: str, versionName: str = ...
+    ) -> PublishAppVersionResponseTypeDef:
         """
         Publishes a new version of a specific Resilience Hub application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.publish_app_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#publish_app_version)
         """
     def put_draft_app_version_template(
@@ -686,14 +723,16 @@
     def update_app(
         self,
         *,
         appArn: str,
         assessmentSchedule: AppAssessmentScheduleTypeType = ...,
         clearResiliencyPolicyArn: bool = ...,
         description: str = ...,
+        eventSubscriptions: Sequence[EventSubscriptionTypeDef] = ...,
+        permissionModel: PermissionModelUnionTypeDef = ...,
         policyArn: str = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#update_app)
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.py` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/literals.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -14,29 +14,35 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
+    "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
     "AssessmentStatusType",
     "ComplianceStatusType",
     "ConfigRecommendationOptimizationTypeType",
     "CostFrequencyType",
     "DataLocationConstraintType",
+    "DifferenceTypeType",
     "DisruptionTypeType",
+    "DriftStatusType",
+    "DriftTypeType",
     "EstimatedCostTierType",
+    "EventTypeType",
+    "ExcludeRecommendationReasonType",
     "HaArchitectureType",
+    "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
@@ -49,47 +55,55 @@
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
+AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
 AssessmentInvokerType = Literal["System", "User"]
 AssessmentStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 ComplianceStatusType = Literal["PolicyBreached", "PolicyMet"]
 ConfigRecommendationOptimizationTypeType = Literal[
     "BestAZRecovery",
     "BestAttainable",
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
+DifferenceTypeType = Literal["NotEqual"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
+DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
+DriftTypeType = Literal["ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
+EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
+ExcludeRecommendationReasonType = Literal[
+    "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
+]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
+PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
-    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
+    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical", "NotApplicable"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.pyi` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/literals.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,28 +14,36 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AlarmTypeType",
     "AppAssessmentScheduleTypeType",
     "AppComplianceStatusTypeType",
+    "AppDriftStatusTypeType",
     "AppStatusTypeType",
     "AssessmentInvokerType",
     "AssessmentStatusType",
     "ComplianceStatusType",
     "ConfigRecommendationOptimizationTypeType",
     "CostFrequencyType",
     "DataLocationConstraintType",
+    "DifferenceTypeType",
     "DisruptionTypeType",
+    "DriftStatusType",
+    "DriftTypeType",
     "EstimatedCostTierType",
+    "EventTypeType",
+    "ExcludeRecommendationReasonType",
     "HaArchitectureType",
+    "PermissionModelTypeType",
     "PhysicalIdentifierTypeType",
     "RecommendationComplianceStatusType",
     "RecommendationTemplateStatusType",
     "RenderRecommendationTypeType",
     "ResiliencyPolicyTierType",
     "ResourceImportStatusTypeType",
     "ResourceImportStrategyTypeType",
@@ -48,46 +56,56 @@
     "TestTypeType",
     "ResilienceHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AlarmTypeType = Literal["Canary", "Composite", "Event", "Logs", "Metric"]
 AppAssessmentScheduleTypeType = Literal["Daily", "Disabled"]
 AppComplianceStatusTypeType = Literal[
     "ChangesDetected", "NotAssessed", "PolicyBreached", "PolicyMet"
 ]
+AppDriftStatusTypeType = Literal["Detected", "NotChecked", "NotDetected"]
 AppStatusTypeType = Literal["Active", "Deleting"]
 AssessmentInvokerType = Literal["System", "User"]
 AssessmentStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 ComplianceStatusType = Literal["PolicyBreached", "PolicyMet"]
 ConfigRecommendationOptimizationTypeType = Literal[
     "BestAZRecovery",
     "BestAttainable",
     "BestRegionRecovery",
     "LeastChange",
     "LeastCost",
     "LeastErrors",
 ]
 CostFrequencyType = Literal["Daily", "Hourly", "Monthly", "Yearly"]
 DataLocationConstraintType = Literal["AnyLocation", "SameContinent", "SameCountry"]
+DifferenceTypeType = Literal["NotEqual"]
 DisruptionTypeType = Literal["AZ", "Hardware", "Region", "Software"]
+DriftStatusType = Literal["Detected", "NotChecked", "NotDetected"]
+DriftTypeType = Literal["ApplicationCompliance"]
 EstimatedCostTierType = Literal["L1", "L2", "L3", "L4"]
+EventTypeType = Literal["DriftDetected", "ScheduledAssessmentFailure"]
+ExcludeRecommendationReasonType = Literal[
+    "AlreadyImplemented", "ComplexityOfImplementation", "NotRelevant"
+]
 HaArchitectureType = Literal[
     "BackupAndRestore", "MultiSite", "NoRecoveryPlan", "PilotLight", "WarmStandby"
 ]
+PermissionModelTypeType = Literal["LegacyIAMUser", "RoleBased"]
 PhysicalIdentifierTypeType = Literal["Arn", "Native"]
 RecommendationComplianceStatusType = Literal[
     "BreachedCanMeet", "BreachedUnattainable", "MetCanImprove"
 ]
 RecommendationTemplateStatusType = Literal["Failed", "InProgress", "Pending", "Success"]
 RenderRecommendationTypeType = Literal["Alarm", "Sop", "Test"]
 ResiliencyPolicyTierType = Literal[
-    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical"
+    "CoreServices", "Critical", "Important", "MissionCritical", "NonCritical", "NotApplicable"
 ]
 ResourceImportStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
 ResourceImportStrategyTypeType = Literal["AddOnly", "ReplaceAll"]
 ResourceMappingTypeType = Literal[
     "AppRegistryApp", "CfnStack", "EKS", "Resource", "ResourceGroup", "Terraform"
 ]
 ResourceResolutionStatusTypeType = Literal["Failed", "InProgress", "Pending", "Success"]
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.py` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,29 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
     DisruptionTypeType,
+    DriftStatusType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -60,18 +65,21 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
-    "AppTypeDef",
+    "EventSubscriptionTypeDef",
+    "PermissionModelOutputTypeDef",
     "AppVersionSummaryTypeDef",
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
-    "CreateAppRequestRequestTypeDef",
+    "PermissionModelTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -84,22 +92,23 @@
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
+    "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
-    "ListAppVersionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
@@ -110,15 +119,14 @@
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
     "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppResponseTypeDef",
     "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
@@ -131,49 +139,60 @@
     "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
+    "ComplianceDriftTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DescribeAppResponseTypeDef",
-    "UpdateAppResponseTypeDef",
+    "AppTypeDef",
     "ListAppVersionsResponseTypeDef",
+    "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "PermissionModelUnionTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     "EksSourceUnionTypeDef",
+    "ListAppVersionsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DeleteAppInputSourceResponseTypeDef",
     "ListAppInputSourcesResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DescribeAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
@@ -205,14 +224,16 @@
     },
 )
 
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
+        "excludeReason": ExcludeRecommendationReasonType,
+        "excluded": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
     },
     total=False,
 )
 
@@ -308,60 +329,110 @@
 )
 _OptionalAppSummaryTypeDef = TypedDict(
     "_OptionalAppSummaryTypeDef",
     {
         "assessmentSchedule": AppAssessmentScheduleTypeType,
         "complianceStatus": AppComplianceStatusTypeType,
         "description": str,
+        "driftStatus": AppDriftStatusTypeType,
         "resiliencyScore": float,
         "status": AppStatusTypeType,
     },
     total=False,
 )
 
 
 class AppSummaryTypeDef(_RequiredAppSummaryTypeDef, _OptionalAppSummaryTypeDef):
     pass
 
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
+_RequiredEventSubscriptionTypeDef = TypedDict(
+    "_RequiredEventSubscriptionTypeDef",
     {
-        "appArn": str,
-        "creationTime": datetime,
+        "eventType": EventTypeType,
         "name": str,
     },
 )
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
+_OptionalEventSubscriptionTypeDef = TypedDict(
+    "_OptionalEventSubscriptionTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "complianceStatus": AppComplianceStatusTypeType,
-        "description": str,
-        "lastAppComplianceEvaluationTime": datetime,
-        "lastResiliencyScoreEvaluationTime": datetime,
-        "policyArn": str,
-        "resiliencyScore": float,
-        "status": AppStatusTypeType,
-        "tags": Dict[str, str],
+        "snsTopicArn": str,
     },
     total=False,
 )
 
 
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+class EventSubscriptionTypeDef(
+    _RequiredEventSubscriptionTypeDef, _OptionalEventSubscriptionTypeDef
+):
     pass
 
 
-AppVersionSummaryTypeDef = TypedDict(
-    "AppVersionSummaryTypeDef",
+_RequiredPermissionModelOutputTypeDef = TypedDict(
+    "_RequiredPermissionModelOutputTypeDef",
+    {
+        "type": PermissionModelTypeType,
+    },
+)
+_OptionalPermissionModelOutputTypeDef = TypedDict(
+    "_OptionalPermissionModelOutputTypeDef",
+    {
+        "crossAccountRoleArns": List[str],
+        "invokerRoleName": str,
+    },
+    total=False,
+)
+
+
+class PermissionModelOutputTypeDef(
+    _RequiredPermissionModelOutputTypeDef, _OptionalPermissionModelOutputTypeDef
+):
+    pass
+
+
+_RequiredAppVersionSummaryTypeDef = TypedDict(
+    "_RequiredAppVersionSummaryTypeDef",
     {
         "appVersion": str,
     },
 )
+_OptionalAppVersionSummaryTypeDef = TypedDict(
+    "_OptionalAppVersionSummaryTypeDef",
+    {
+        "creationTime": datetime,
+        "identifier": int,
+        "versionName": str,
+    },
+    total=False,
+)
+
+
+class AppVersionSummaryTypeDef(
+    _RequiredAppVersionSummaryTypeDef, _OptionalAppVersionSummaryTypeDef
+):
+    pass
+
+
+BatchUpdateRecommendationStatusFailedEntryTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    {
+        "entryId": str,
+        "errorMessage": str,
+    },
+)
+
+UpdateRecommendationStatusItemTypeDef = TypedDict(
+    "UpdateRecommendationStatusItemTypeDef",
+    {
+        "resourceId": str,
+        "targetAccountId": str,
+        "targetRegion": str,
+    },
+    total=False,
+)
 
 _RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
     "_RequiredRecommendationDisruptionComplianceTypeDef",
     {
         "expectedComplianceStatus": ComplianceStatusType,
     },
 )
@@ -380,36 +451,31 @@
 class RecommendationDisruptionComplianceTypeDef(
     _RequiredRecommendationDisruptionComplianceTypeDef,
     _OptionalRecommendationDisruptionComplianceTypeDef,
 ):
     pass
 
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
+_RequiredPermissionModelTypeDef = TypedDict(
+    "_RequiredPermissionModelTypeDef",
     {
-        "name": str,
+        "type": PermissionModelTypeType,
     },
 )
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
+_OptionalPermissionModelTypeDef = TypedDict(
+    "_OptionalPermissionModelTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clientToken": str,
-        "description": str,
-        "policyArn": str,
-        "tags": Mapping[str, str],
+        "crossAccountRoleArns": Sequence[str],
+        "invokerRoleName": str,
     },
     total=False,
 )
 
 
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
+class PermissionModelTypeDef(_RequiredPermissionModelTypeDef, _OptionalPermissionModelTypeDef):
     pass
 
 
 _RequiredCreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
@@ -717,14 +783,37 @@
 class ListAlarmRecommendationsRequestRequestTypeDef(
     _RequiredListAlarmRecommendationsRequestRequestTypeDef,
     _OptionalListAlarmRecommendationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "assessmentArn": str,
+    },
+)
+_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(
+    _RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+    _OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+):
+    pass
+
+
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": str,
         "assessmentName": str,
         "assessmentStatus": Sequence[AssessmentStatusType],
         "complianceStatus": ComplianceStatusType,
@@ -875,36 +964,15 @@
 class ListAppVersionResourcesRequestRequestTypeDef(
     _RequiredListAppVersionResourcesRequestRequestTypeDef,
     _OptionalListAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppVersionsRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppVersionsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListAppVersionsRequestRequestTypeDef(
-    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appArn": str,
         "maxResults": int,
         "name": str,
         "nextToken": str,
@@ -1055,20 +1123,34 @@
 
 class PhysicalResourceIdTypeDef(
     _RequiredPhysicalResourceIdTypeDef, _OptionalPhysicalResourceIdTypeDef
 ):
     pass
 
 
-PublishAppVersionRequestRequestTypeDef = TypedDict(
-    "PublishAppVersionRequestRequestTypeDef",
+_RequiredPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
+_OptionalPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishAppVersionRequestRequestTypeDef",
+    {
+        "versionName": str,
+    },
+    total=False,
+)
+
+
+class PublishAppVersionRequestRequestTypeDef(
+    _RequiredPublishAppVersionRequestRequestTypeDef, _OptionalPublishAppVersionRequestRequestTypeDef
+):
+    pass
+
 
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
@@ -1165,38 +1247,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clearResiliencyPolicyArn": bool,
-        "description": str,
-        "policyArn": str,
-    },
-    total=False,
-)
-
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -1326,14 +1384,16 @@
 )
 
 PublishAppVersionResponseTypeDef = TypedDict(
     "PublishAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
+        "identifier": int,
+        "versionName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
     "PutDraftAppVersionTemplateResponseTypeDef",
     {
@@ -1382,14 +1442,15 @@
         "type": AlarmTypeType,
     },
 )
 _OptionalAlarmRecommendationTypeDef = TypedDict(
     "_OptionalAlarmRecommendationTypeDef",
     {
         "appComponentName": str,
+        "appComponentNames": List[str],
         "description": str,
         "items": List[RecommendationItemTypeDef],
         "prerequisite": str,
     },
     total=False,
 )
 
@@ -1468,30 +1529,49 @@
     "_OptionalAppAssessmentSummaryTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "invoker": AssessmentInvokerType,
         "message": str,
         "resiliencyScore": float,
         "startTime": datetime,
+        "versionName": str,
     },
     total=False,
 )
 
 
 class AppAssessmentSummaryTypeDef(
     _RequiredAppAssessmentSummaryTypeDef, _OptionalAppAssessmentSummaryTypeDef
 ):
     pass
 
 
+ComplianceDriftTypeDef = TypedDict(
+    "ComplianceDriftTypeDef",
+    {
+        "actualReferenceId": str,
+        "actualValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+        "appId": str,
+        "appVersion": str,
+        "diffType": Literal["NotEqual"],
+        "driftType": Literal["ApplicationCompliance"],
+        "entityId": str,
+        "entityType": str,
+        "expectedReferenceId": str,
+        "expectedValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+    },
+    total=False,
+)
+
 AppComponentComplianceTypeDef = TypedDict(
     "AppComponentComplianceTypeDef",
     {
         "appComponentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "cost": CostTypeDef,
         "message": str,
@@ -1605,47 +1685,106 @@
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "appArn": str,
+        "creationTime": datetime,
+        "name": str,
     },
 )
-
-DescribeAppResponseTypeDef = TypedDict(
-    "DescribeAppResponseTypeDef",
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "complianceStatus": AppComplianceStatusTypeType,
+        "description": str,
+        "driftStatus": AppDriftStatusTypeType,
+        "eventSubscriptions": List[EventSubscriptionTypeDef],
+        "lastAppComplianceEvaluationTime": datetime,
+        "lastDriftEvaluationTime": datetime,
+        "lastResiliencyScoreEvaluationTime": datetime,
+        "permissionModel": PermissionModelOutputTypeDef,
+        "policyArn": str,
+        "resiliencyScore": float,
+        "status": AppStatusTypeType,
+        "tags": Dict[str, str],
     },
+    total=False,
 )
 
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+
+class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(
+    _RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    _OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+):
+    pass
+
+
+_RequiredUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_RequiredUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_OptionalUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+
+class UpdateRecommendationStatusRequestEntryTypeDef(
+    _RequiredUpdateRecommendationStatusRequestEntryTypeDef,
+    _OptionalUpdateRecommendationStatusRequestEntryTypeDef,
+):
+    pass
+
+
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
         "optimizationType": ConfigRecommendationOptimizationTypeType,
         "referenceId": str,
     },
@@ -1669,14 +1808,68 @@
 
 class ConfigRecommendationTypeDef(
     _RequiredConfigRecommendationTypeDef, _OptionalConfigRecommendationTypeDef
 ):
     pass
 
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clientToken": str,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+
+PermissionModelUnionTypeDef = Union[PermissionModelTypeDef, PermissionModelOutputTypeDef]
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clearResiliencyPolicyArn": bool,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "appComponents": Sequence[str],
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": str,
@@ -1866,14 +2059,38 @@
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
+_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppVersionsRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppVersionsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAppVersionsRequestRequestTypeDef(
+    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2018,14 +2235,23 @@
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAppAssessmentComplianceDriftsResponseTypeDef = TypedDict(
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
+    {
+        "complianceDrifts": List[ComplianceDriftTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2045,14 +2271,56 @@
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppResponseTypeDef = TypedDict(
+    "DescribeAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusResponseTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "failedEntries": List[BatchUpdateRecommendationStatusFailedEntryTypeDef],
+        "successfulEntries": List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusRequestRequestTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "requestEntries": Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
+    },
+)
+
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
@@ -2242,21 +2510,23 @@
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "message": str,
         "policy": ResiliencyPolicyTypeDef,
         "resiliencyScore": ResiliencyScoreTypeDef,
         "resourceErrorsDetails": ResourceErrorsDetailsTypeDef,
         "startTime": datetime,
         "tags": Dict[str, str],
+        "versionName": str,
     },
     total=False,
 )
 
 
 class AppAssessmentTypeDef(_RequiredAppAssessmentTypeDef, _OptionalAppAssessmentTypeDef):
     pass
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,29 @@
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
     DisruptionTypeType,
+    DriftStatusType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -59,18 +64,21 @@
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
     "EksSourceClusterNamespaceTypeDef",
     "TerraformSourceTypeDef",
     "AppSummaryTypeDef",
-    "AppTypeDef",
+    "EventSubscriptionTypeDef",
+    "PermissionModelOutputTypeDef",
     "AppVersionSummaryTypeDef",
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    "UpdateRecommendationStatusItemTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
-    "CreateAppRequestRequestTypeDef",
+    "PermissionModelTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
@@ -83,22 +91,23 @@
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
     "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
+    "ListAppAssessmentComplianceDriftsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
     "ListAppVersionResourcesRequestRequestTypeDef",
-    "ListAppVersionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
@@ -109,15 +118,14 @@
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     "ResourceErrorTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
     "DeleteAppAssessmentResponseTypeDef",
     "DeleteAppResponseTypeDef",
     "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
@@ -130,49 +138,60 @@
     "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
+    "ComplianceDriftTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
     "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
-    "CreateAppResponseTypeDef",
-    "DescribeAppResponseTypeDef",
-    "UpdateAppResponseTypeDef",
+    "AppTypeDef",
     "ListAppVersionsResponseTypeDef",
+    "BatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    "UpdateRecommendationStatusRequestEntryTypeDef",
     "ConfigRecommendationTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "PermissionModelUnionTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
     "EksSourceUnionTypeDef",
+    "ListAppVersionsRequestRequestTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
     "DeleteAppInputSourceResponseTypeDef",
     "ListAppInputSourcesResponseTypeDef",
+    "CreateAppResponseTypeDef",
+    "DescribeAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
@@ -204,14 +223,16 @@
     },
 )
 
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
+        "excludeReason": ExcludeRecommendationReasonType,
+        "excluded": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
     },
     total=False,
 )
 
@@ -303,56 +324,102 @@
 )
 _OptionalAppSummaryTypeDef = TypedDict(
     "_OptionalAppSummaryTypeDef",
     {
         "assessmentSchedule": AppAssessmentScheduleTypeType,
         "complianceStatus": AppComplianceStatusTypeType,
         "description": str,
+        "driftStatus": AppDriftStatusTypeType,
         "resiliencyScore": float,
         "status": AppStatusTypeType,
     },
     total=False,
 )
 
 class AppSummaryTypeDef(_RequiredAppSummaryTypeDef, _OptionalAppSummaryTypeDef):
     pass
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
+_RequiredEventSubscriptionTypeDef = TypedDict(
+    "_RequiredEventSubscriptionTypeDef",
     {
-        "appArn": str,
-        "creationTime": datetime,
+        "eventType": EventTypeType,
         "name": str,
     },
 )
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
+_OptionalEventSubscriptionTypeDef = TypedDict(
+    "_OptionalEventSubscriptionTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "complianceStatus": AppComplianceStatusTypeType,
-        "description": str,
-        "lastAppComplianceEvaluationTime": datetime,
-        "lastResiliencyScoreEvaluationTime": datetime,
-        "policyArn": str,
-        "resiliencyScore": float,
-        "status": AppStatusTypeType,
-        "tags": Dict[str, str],
+        "snsTopicArn": str,
     },
     total=False,
 )
 
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+class EventSubscriptionTypeDef(
+    _RequiredEventSubscriptionTypeDef, _OptionalEventSubscriptionTypeDef
+):
     pass
 
-AppVersionSummaryTypeDef = TypedDict(
-    "AppVersionSummaryTypeDef",
+_RequiredPermissionModelOutputTypeDef = TypedDict(
+    "_RequiredPermissionModelOutputTypeDef",
+    {
+        "type": PermissionModelTypeType,
+    },
+)
+_OptionalPermissionModelOutputTypeDef = TypedDict(
+    "_OptionalPermissionModelOutputTypeDef",
+    {
+        "crossAccountRoleArns": List[str],
+        "invokerRoleName": str,
+    },
+    total=False,
+)
+
+class PermissionModelOutputTypeDef(
+    _RequiredPermissionModelOutputTypeDef, _OptionalPermissionModelOutputTypeDef
+):
+    pass
+
+_RequiredAppVersionSummaryTypeDef = TypedDict(
+    "_RequiredAppVersionSummaryTypeDef",
     {
         "appVersion": str,
     },
 )
+_OptionalAppVersionSummaryTypeDef = TypedDict(
+    "_OptionalAppVersionSummaryTypeDef",
+    {
+        "creationTime": datetime,
+        "identifier": int,
+        "versionName": str,
+    },
+    total=False,
+)
+
+class AppVersionSummaryTypeDef(
+    _RequiredAppVersionSummaryTypeDef, _OptionalAppVersionSummaryTypeDef
+):
+    pass
+
+BatchUpdateRecommendationStatusFailedEntryTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusFailedEntryTypeDef",
+    {
+        "entryId": str,
+        "errorMessage": str,
+    },
+)
+
+UpdateRecommendationStatusItemTypeDef = TypedDict(
+    "UpdateRecommendationStatusItemTypeDef",
+    {
+        "resourceId": str,
+        "targetAccountId": str,
+        "targetRegion": str,
+    },
+    total=False,
+)
 
 _RequiredRecommendationDisruptionComplianceTypeDef = TypedDict(
     "_RequiredRecommendationDisruptionComplianceTypeDef",
     {
         "expectedComplianceStatus": ComplianceStatusType,
     },
 )
@@ -369,35 +436,30 @@
 
 class RecommendationDisruptionComplianceTypeDef(
     _RequiredRecommendationDisruptionComplianceTypeDef,
     _OptionalRecommendationDisruptionComplianceTypeDef,
 ):
     pass
 
-_RequiredCreateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppRequestRequestTypeDef",
+_RequiredPermissionModelTypeDef = TypedDict(
+    "_RequiredPermissionModelTypeDef",
     {
-        "name": str,
+        "type": PermissionModelTypeType,
     },
 )
-_OptionalCreateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppRequestRequestTypeDef",
+_OptionalPermissionModelTypeDef = TypedDict(
+    "_OptionalPermissionModelTypeDef",
     {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clientToken": str,
-        "description": str,
-        "policyArn": str,
-        "tags": Mapping[str, str],
+        "crossAccountRoleArns": Sequence[str],
+        "invokerRoleName": str,
     },
     total=False,
 )
 
-class CreateAppRequestRequestTypeDef(
-    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
-):
+class PermissionModelTypeDef(_RequiredPermissionModelTypeDef, _OptionalPermissionModelTypeDef):
     pass
 
 _RequiredCreateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "name": str,
@@ -684,14 +746,35 @@
 
 class ListAlarmRecommendationsRequestRequestTypeDef(
     _RequiredListAlarmRecommendationsRequestRequestTypeDef,
     _OptionalListAlarmRecommendationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "assessmentArn": str,
+    },
+)
+_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListAppAssessmentComplianceDriftsRequestRequestTypeDef(
+    _RequiredListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+    _OptionalListAppAssessmentComplianceDriftsRequestRequestTypeDef,
+):
+    pass
+
 ListAppAssessmentsRequestRequestTypeDef = TypedDict(
     "ListAppAssessmentsRequestRequestTypeDef",
     {
         "appArn": str,
         "assessmentName": str,
         "assessmentStatus": Sequence[AssessmentStatusType],
         "complianceStatus": ComplianceStatusType,
@@ -830,34 +913,15 @@
 
 class ListAppVersionResourcesRequestRequestTypeDef(
     _RequiredListAppVersionResourcesRequestRequestTypeDef,
     _OptionalListAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAppVersionsRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAppVersionsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListAppVersionsRequestRequestTypeDef(
-    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appArn": str,
         "maxResults": int,
         "name": str,
         "nextToken": str,
@@ -998,20 +1062,32 @@
 )
 
 class PhysicalResourceIdTypeDef(
     _RequiredPhysicalResourceIdTypeDef, _OptionalPhysicalResourceIdTypeDef
 ):
     pass
 
-PublishAppVersionRequestRequestTypeDef = TypedDict(
-    "PublishAppVersionRequestRequestTypeDef",
+_RequiredPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredPublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
+_OptionalPublishAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalPublishAppVersionRequestRequestTypeDef",
+    {
+        "versionName": str,
+    },
+    total=False,
+)
+
+class PublishAppVersionRequestRequestTypeDef(
+    _RequiredPublishAppVersionRequestRequestTypeDef, _OptionalPublishAppVersionRequestRequestTypeDef
+):
+    pass
 
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
@@ -1104,36 +1180,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppRequestRequestTypeDef",
-    {
-        "assessmentSchedule": AppAssessmentScheduleTypeType,
-        "clearResiliencyPolicyArn": bool,
-        "description": str,
-        "policyArn": str,
-    },
-    total=False,
-)
-
-class UpdateAppRequestRequestTypeDef(
-    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -1259,14 +1313,16 @@
 )
 
 PublishAppVersionResponseTypeDef = TypedDict(
     "PublishAppVersionResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
+        "identifier": int,
+        "versionName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
     "PutDraftAppVersionTemplateResponseTypeDef",
     {
@@ -1315,14 +1371,15 @@
         "type": AlarmTypeType,
     },
 )
 _OptionalAlarmRecommendationTypeDef = TypedDict(
     "_OptionalAlarmRecommendationTypeDef",
     {
         "appComponentName": str,
+        "appComponentNames": List[str],
         "description": str,
         "items": List[RecommendationItemTypeDef],
         "prerequisite": str,
     },
     total=False,
 )
 
@@ -1395,28 +1452,47 @@
     "_OptionalAppAssessmentSummaryTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "invoker": AssessmentInvokerType,
         "message": str,
         "resiliencyScore": float,
         "startTime": datetime,
+        "versionName": str,
     },
     total=False,
 )
 
 class AppAssessmentSummaryTypeDef(
     _RequiredAppAssessmentSummaryTypeDef, _OptionalAppAssessmentSummaryTypeDef
 ):
     pass
 
+ComplianceDriftTypeDef = TypedDict(
+    "ComplianceDriftTypeDef",
+    {
+        "actualReferenceId": str,
+        "actualValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+        "appId": str,
+        "appVersion": str,
+        "diffType": Literal["NotEqual"],
+        "driftType": Literal["ApplicationCompliance"],
+        "entityId": str,
+        "entityType": str,
+        "expectedReferenceId": str,
+        "expectedValue": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
+    },
+    total=False,
+)
+
 AppComponentComplianceTypeDef = TypedDict(
     "AppComponentComplianceTypeDef",
     {
         "appComponentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "cost": CostTypeDef,
         "message": str,
@@ -1526,47 +1602,100 @@
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "appArn": str,
+        "creationTime": datetime,
+        "name": str,
     },
 )
-
-DescribeAppResponseTypeDef = TypedDict(
-    "DescribeAppResponseTypeDef",
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
     {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "complianceStatus": AppComplianceStatusTypeType,
+        "description": str,
+        "driftStatus": AppDriftStatusTypeType,
+        "eventSubscriptions": List[EventSubscriptionTypeDef],
+        "lastAppComplianceEvaluationTime": datetime,
+        "lastDriftEvaluationTime": datetime,
+        "lastResiliencyScoreEvaluationTime": datetime,
+        "permissionModel": PermissionModelOutputTypeDef,
+        "policyArn": str,
+        "resiliencyScore": float,
+        "status": AppStatusTypeType,
+        "tags": Dict[str, str],
     },
+    total=False,
 )
 
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
-    {
-        "app": AppTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef = TypedDict(
+    "_OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+class BatchUpdateRecommendationStatusSuccessfulEntryTypeDef(
+    _RequiredBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    _OptionalBatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+):
+    pass
+
+_RequiredUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_RequiredUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "entryId": str,
+        "excluded": bool,
+        "item": UpdateRecommendationStatusItemTypeDef,
+        "referenceId": str,
+    },
+)
+_OptionalUpdateRecommendationStatusRequestEntryTypeDef = TypedDict(
+    "_OptionalUpdateRecommendationStatusRequestEntryTypeDef",
+    {
+        "excludeReason": ExcludeRecommendationReasonType,
+    },
+    total=False,
+)
+
+class UpdateRecommendationStatusRequestEntryTypeDef(
+    _RequiredUpdateRecommendationStatusRequestEntryTypeDef,
+    _OptionalUpdateRecommendationStatusRequestEntryTypeDef,
+):
+    pass
+
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
         "optimizationType": ConfigRecommendationOptimizationTypeType,
         "referenceId": str,
     },
@@ -1588,14 +1717,64 @@
 )
 
 class ConfigRecommendationTypeDef(
     _RequiredConfigRecommendationTypeDef, _OptionalConfigRecommendationTypeDef
 ):
     pass
 
+_RequiredCreateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clientToken": str,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateAppRequestRequestTypeDef(
+    _RequiredCreateAppRequestRequestTypeDef, _OptionalCreateAppRequestRequestTypeDef
+):
+    pass
+
+PermissionModelUnionTypeDef = Union[PermissionModelTypeDef, PermissionModelOutputTypeDef]
+_RequiredUpdateAppRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalUpdateAppRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppRequestRequestTypeDef",
+    {
+        "assessmentSchedule": AppAssessmentScheduleTypeType,
+        "clearResiliencyPolicyArn": bool,
+        "description": str,
+        "eventSubscriptions": Sequence[EventSubscriptionTypeDef],
+        "permissionModel": PermissionModelTypeDef,
+        "policyArn": str,
+    },
+    total=False,
+)
+
+class UpdateAppRequestRequestTypeDef(
+    _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateAppVersionResourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppVersionResourceRequestRequestTypeDef",
     {
         "appArn": str,
         "appComponents": Sequence[str],
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": str,
@@ -1773,14 +1952,36 @@
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
+_RequiredListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAppVersionsRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalListAppVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAppVersionsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class ListAppVersionsRequestRequestTypeDef(
+    _RequiredListAppVersionsRequestRequestTypeDef, _OptionalListAppVersionsRequestRequestTypeDef
+):
+    pass
+
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -1917,14 +2118,23 @@
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAppAssessmentComplianceDriftsResponseTypeDef = TypedDict(
+    "ListAppAssessmentComplianceDriftsResponseTypeDef",
+    {
+        "complianceDrifts": List[ComplianceDriftTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1944,14 +2154,56 @@
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppResponseTypeDef = TypedDict(
+    "DescribeAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
+    {
+        "app": AppTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusResponseTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "failedEntries": List[BatchUpdateRecommendationStatusFailedEntryTypeDef],
+        "successfulEntries": List[BatchUpdateRecommendationStatusSuccessfulEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdateRecommendationStatusRequestRequestTypeDef = TypedDict(
+    "BatchUpdateRecommendationStatusRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "requestEntries": Sequence[UpdateRecommendationStatusRequestEntryTypeDef],
+    },
+)
+
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
         "configRecommendations": List[ConfigRecommendationTypeDef],
         "recommendationStatus": RecommendationComplianceStatusType,
     },
@@ -2139,21 +2391,23 @@
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
         "compliance": Dict[DisruptionTypeType, DisruptionComplianceTypeDef],
         "complianceStatus": ComplianceStatusType,
         "cost": CostTypeDef,
+        "driftStatus": DriftStatusType,
         "endTime": datetime,
         "message": str,
         "policy": ResiliencyPolicyTypeDef,
         "resiliencyScore": ResiliencyScoreTypeDef,
         "resourceErrorsDetails": ResourceErrorsDetailsTypeDef,
         "startTime": datetime,
         "tags": Dict[str, str],
+        "versionName": str,
     },
     total=False,
 )
 
 class AppAssessmentTypeDef(_RequiredAppAssessmentTypeDef, _OptionalAppAssessmentTypeDef):
     pass
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.16
-Summary: Type annotations for boto3.ResilienceHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.18
+Summary: Type annotations for boto3.ResilienceHub 1.28.18 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -279,24 +279,31 @@
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_resiliencehub.literals import (
     AlarmTypeType,
     AppAssessmentScheduleTypeType,
     AppComplianceStatusTypeType,
+    AppDriftStatusTypeType,
     AppStatusTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
     ComplianceStatusType,
     ConfigRecommendationOptimizationTypeType,
     CostFrequencyType,
     DataLocationConstraintType,
+    DifferenceTypeType,
     DisruptionTypeType,
+    DriftStatusType,
+    DriftTypeType,
     EstimatedCostTierType,
+    EventTypeType,
+    ExcludeRecommendationReasonType,
     HaArchitectureType,
+    PermissionModelTypeType,
     PhysicalIdentifierTypeType,
     RecommendationComplianceStatusType,
     RecommendationTemplateStatusType,
     RenderRecommendationTypeType,
     ResiliencyPolicyTierType,
     ResourceImportStatusTypeType,
     ResourceImportStrategyTypeType,
@@ -332,18 +339,21 @@
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
     EksSourceClusterNamespaceTypeDef,
     TerraformSourceTypeDef,
     AppSummaryTypeDef,
-    AppTypeDef,
+    EventSubscriptionTypeDef,
+    PermissionModelOutputTypeDef,
     AppVersionSummaryTypeDef,
+    BatchUpdateRecommendationStatusFailedEntryTypeDef,
+    UpdateRecommendationStatusItemTypeDef,
     RecommendationDisruptionComplianceTypeDef,
-    CreateAppRequestRequestTypeDef,
+    PermissionModelTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
@@ -356,22 +366,23 @@
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
     EksSourceOutputTypeDef,
     EksSourceTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
+    ListAppAssessmentComplianceDriftsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
     ListAppVersionResourcesRequestRequestTypeDef,
-    ListAppVersionsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
@@ -382,15 +393,14 @@
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
     ResourceErrorTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
     DeleteAppAssessmentResponseTypeDef,
     DeleteAppResponseTypeDef,
     DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
@@ -403,49 +413,60 @@
     RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
+    ComplianceDriftTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
     DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
-    CreateAppResponseTypeDef,
-    DescribeAppResponseTypeDef,
-    UpdateAppResponseTypeDef,
+    AppTypeDef,
     ListAppVersionsResponseTypeDef,
+    BatchUpdateRecommendationStatusSuccessfulEntryTypeDef,
+    UpdateRecommendationStatusRequestEntryTypeDef,
     ConfigRecommendationTypeDef,
+    CreateAppRequestRequestTypeDef,
+    PermissionModelUnionTypeDef,
+    UpdateAppRequestRequestTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     EksSourceUnionTypeDef,
+    ListAppVersionsRequestRequestTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
+    ListAppAssessmentComplianceDriftsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     DeleteAppInputSourceResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
+    CreateAppResponseTypeDef,
+    DescribeAppResponseTypeDef,
+    UpdateAppResponseTypeDef,
+    BatchUpdateRecommendationStatusResponseTypeDef,
+    BatchUpdateRecommendationStatusRequestRequestTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     ImportResourcesToDraftAppVersionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy-boto3-resiliencehub-1.28.18/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.16/setup.py` & `mypy-boto3-resiliencehub-1.28.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.28.16",
+    version="1.28.18",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResilienceHub 1.28.16 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.ResilienceHub 1.28.18 service generated with mypy-boto3-builder"
         " 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


# Comparing `tmp/types-aiobotocore-codebuild-2.5.2.tar.gz` & `tmp/types-aiobotocore-codebuild-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codebuild-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codebuild-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codebuild-2.5.2.tar` & `types-aiobotocore-codebuild-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.729867 types-aiobotocore-codebuild-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-08 01:43:23.729867 types-aiobotocore-codebuild-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19942 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.729867 types-aiobotocore-codebuild-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.729867 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43759 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43693 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-08 01:27:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-07-08 01:27:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57301 2023-07-08 01:27:24.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57242 2023-07-08 01:27:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:22.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.729867 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-08 01:43:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:23.000000 types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20233 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.433626 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43834 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43768 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-02 14:34:56.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59885 2023-08-02 14:34:57.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59822 2023-08-02 14:34:56.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codebuild-2.5.2/LICENSE` & `types-aiobotocore-codebuild-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2/PKG-INFO` & `types-aiobotocore-codebuild-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codebuild
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codebuild type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codebuild type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codebuild"></a>
 
 # types-aiobotocore-codebuild
 
 [![PyPI - types-aiobotocore-codebuild](https://img.shields.io/pypi/v/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codebuild?color=blue)](https://pypistats.org/packages/types-aiobotocore-codebuild)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeBuild 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [types-aiobotocore-codebuild docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/).
 
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
@@ -396,145 +395,154 @@
 )
 
 
 def check_value(value: ArtifactNamespaceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codebuild.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
+    BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
-    ProjectCacheTypeDef,
+    ProjectCacheOutputTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceVersionTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
+    ProjectCacheTypeDef,
     TagTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
-    GetResourcePolicyOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
-    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
     S3LogsConfigTypeDef,
-    PaginatorConfigTypeDef,
     ProjectBadgeTypeDef,
     RegistryCredentialTypeDef,
     SourceAuthTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
+    GetResourcePolicyOutputTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsOutputTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
+    ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
+    ProjectCacheUnionTypeDef,
+    VpcConfigUnionTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     LogsLocationTypeDef,
+    ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
     ProjectSourceTypeDef,
     ReportExportConfigTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
     BuildGroupTypeDef,
     CreateWebhookOutputTypeDef,
     UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
     ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
     CreateReportGroupInputRequestTypeDef,
@@ -557,15 +565,15 @@
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteBuildsInputRequestTypeDef:
+def get_value() -> BatchDeleteBuildsInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codebuild-2.5.2/README.md` & `types-aiobotocore-codebuild-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codebuild"></a>
 
 # types-aiobotocore-codebuild
 
 [![PyPI - types-aiobotocore-codebuild](https://img.shields.io/pypi/v/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codebuild?color=blue)](https://pypistats.org/packages/types-aiobotocore-codebuild)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeBuild 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [types-aiobotocore-codebuild docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/).
 
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
@@ -363,145 +363,154 @@
 )
 
 
 def check_value(value: ArtifactNamespaceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codebuild.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
+    BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
-    ProjectCacheTypeDef,
+    ProjectCacheOutputTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceVersionTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
+    ProjectCacheTypeDef,
     TagTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
-    GetResourcePolicyOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
-    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
     S3LogsConfigTypeDef,
-    PaginatorConfigTypeDef,
     ProjectBadgeTypeDef,
     RegistryCredentialTypeDef,
     SourceAuthTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
+    GetResourcePolicyOutputTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsOutputTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
+    ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
+    ProjectCacheUnionTypeDef,
+    VpcConfigUnionTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     LogsLocationTypeDef,
+    ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
     ProjectSourceTypeDef,
     ReportExportConfigTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
     BuildGroupTypeDef,
     CreateWebhookOutputTypeDef,
     UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
     ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
     CreateReportGroupInputRequestTypeDef,
@@ -524,15 +533,15 @@
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteBuildsInputRequestTypeDef:
+def get_value() -> BatchDeleteBuildsInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codebuild-2.5.2/setup.py` & `types-aiobotocore-codebuild-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codebuild",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore codebuild type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codebuild type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codebuild": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/"
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/__init__.py` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/__init__.pyi` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/__main__.py` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeBuild 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeBuild 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/client.py` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     ListReportsForReportGroupOutputTypeDef,
     ListReportsOutputTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     ProjectArtifactsTypeDef,
-    ProjectBuildBatchConfigTypeDef,
-    ProjectCacheTypeDef,
-    ProjectEnvironmentTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
+    ProjectCacheUnionTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceTypeDef,
     ProjectSourceVersionTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegistryCredentialTypeDef,
     ReportExportConfigTypeDef,
     ReportFilterTypeDef,
@@ -106,15 +106,15 @@
     StopBuildOutputTypeDef,
     TagTypeDef,
     TestCaseFilterTypeDef,
     UpdateProjectOutputTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     UpdateWebhookOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
     WebhookFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -227,31 +227,31 @@
 
     async def create_project(
         self,
         *,
         name: str,
         source: ProjectSourceTypeDef,
         artifacts: ProjectArtifactsTypeDef,
-        environment: ProjectEnvironmentTypeDef,
+        environment: ProjectEnvironmentUnionTypeDef,
         serviceRole: str,
         description: str = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheTypeDef = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigTypeDef = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_project)
@@ -657,15 +657,15 @@
         insecureSslOverride: bool = ...,
         reportBuildStatusOverride: bool = ...,
         buildStatusConfigOverride: BuildStatusConfigTypeDef = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheTypeDef = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
@@ -698,25 +698,25 @@
         buildspecOverride: str = ...,
         insecureSslOverride: bool = ...,
         reportBuildBatchStatusOverride: bool = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheTypeDef = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         buildTimeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        buildBatchConfigOverride: ProjectBuildBatchConfigTypeDef = ...,
+        buildBatchConfigOverride: ProjectBuildBatchConfigUnionTypeDef = ...,
         debugSessionEnabled: bool = ...
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build_batch)
@@ -745,26 +745,26 @@
         description: str = ...,
         source: ProjectSourceTypeDef = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         artifacts: ProjectArtifactsTypeDef = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheTypeDef = ...,
-        environment: ProjectEnvironmentTypeDef = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
+        environment: ProjectEnvironmentUnionTypeDef = ...,
         serviceRole: str = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigTypeDef = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project)
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/client.pyi` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     ListReportsForReportGroupOutputTypeDef,
     ListReportsOutputTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     ProjectArtifactsTypeDef,
-    ProjectBuildBatchConfigTypeDef,
-    ProjectCacheTypeDef,
-    ProjectEnvironmentTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
+    ProjectCacheUnionTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceTypeDef,
     ProjectSourceVersionTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegistryCredentialTypeDef,
     ReportExportConfigTypeDef,
     ReportFilterTypeDef,
@@ -106,15 +106,15 @@
     StopBuildOutputTypeDef,
     TagTypeDef,
     TestCaseFilterTypeDef,
     UpdateProjectOutputTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     UpdateWebhookOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
     WebhookFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -214,31 +214,31 @@
         """
     async def create_project(
         self,
         *,
         name: str,
         source: ProjectSourceTypeDef,
         artifacts: ProjectArtifactsTypeDef,
-        environment: ProjectEnvironmentTypeDef,
+        environment: ProjectEnvironmentUnionTypeDef,
         serviceRole: str,
         description: str = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheTypeDef = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigTypeDef = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_project)
@@ -612,15 +612,15 @@
         insecureSslOverride: bool = ...,
         reportBuildStatusOverride: bool = ...,
         buildStatusConfigOverride: BuildStatusConfigTypeDef = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheTypeDef = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
@@ -652,25 +652,25 @@
         buildspecOverride: str = ...,
         insecureSslOverride: bool = ...,
         reportBuildBatchStatusOverride: bool = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheTypeDef = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         buildTimeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        buildBatchConfigOverride: ProjectBuildBatchConfigTypeDef = ...,
+        buildBatchConfigOverride: ProjectBuildBatchConfigUnionTypeDef = ...,
         debugSessionEnabled: bool = ...
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build_batch)
@@ -696,26 +696,26 @@
         description: str = ...,
         source: ProjectSourceTypeDef = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         artifacts: ProjectArtifactsTypeDef = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheTypeDef = ...,
-        environment: ProjectEnvironmentTypeDef = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
+        environment: ProjectEnvironmentUnionTypeDef = ...,
         serviceRole: str = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigTypeDef = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project)
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/literals.py` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/literals.pyi` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/paginator.py` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 
@@ -128,15 +128,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describetestcasespaginator)
         """
 
 
@@ -147,15 +147,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 
@@ -167,33 +167,30 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 
 class ListBuildsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sortOrder: SortOrderTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildspaginator)
         """
 
 
@@ -204,15 +201,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 
@@ -223,15 +220,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listprojectspaginator)
         """
 
 
@@ -242,15 +239,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportgroupspaginator)
         """
 
 
@@ -261,15 +258,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportspaginator)
         """
 
 
@@ -281,15 +278,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 
@@ -300,15 +297,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 
@@ -319,13 +316,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/paginator.pyi` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         self,
         *,
         reportArn: str,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportCodeCoverageSortByTypeType = ...,
         minLineCoveragePercentage: float = ...,
         maxLineCoveragePercentage: float = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCodeCoveragesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeCodeCoverages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describecodecoveragespaginator)
         """
 
 class DescribeTestCasesPaginator(AioPaginator):
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         reportArn: str,
         filter: TestCaseFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTestCasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.DescribeTestCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#describetestcasespaginator)
         """
 
 class ListBuildBatchesPaginator(AioPaginator):
@@ -142,15 +142,15 @@
     """
 
     def paginate(
         self,
         *,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildBatchesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchespaginator)
         """
 
 class ListBuildBatchesForProjectPaginator(AioPaginator):
@@ -161,32 +161,29 @@
 
     def paginate(
         self,
         *,
         projectName: str = ...,
         filter: BuildBatchFilterTypeDef = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildBatchesForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildBatchesForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildbatchesforprojectpaginator)
         """
 
 class ListBuildsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sortOrder: SortOrderTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuilds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildspaginator)
         """
 
 class ListBuildsForProjectPaginator(AioPaginator):
@@ -196,15 +193,15 @@
     """
 
     def paginate(
         self,
         *,
         projectName: str,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBuildsForProjectOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListBuildsForProject.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listbuildsforprojectpaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
@@ -214,15 +211,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: ProjectSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listprojectspaginator)
         """
 
 class ListReportGroupsPaginator(AioPaginator):
@@ -232,15 +229,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: ReportGroupSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportgroupspaginator)
         """
 
 class ListReportsPaginator(AioPaginator):
@@ -250,15 +247,15 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportspaginator)
         """
 
 class ListReportsForReportGroupPaginator(AioPaginator):
@@ -269,15 +266,15 @@
 
     def paginate(
         self,
         *,
         reportGroupArn: str,
         sortOrder: SortOrderTypeType = ...,
         filter: ReportFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportsForReportGroupOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListReportsForReportGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listreportsforreportgrouppaginator)
         """
 
 class ListSharedProjectsPaginator(AioPaginator):
@@ -287,15 +284,15 @@
     """
 
     def paginate(
         self,
         *,
         sortBy: SharedResourceSortByTypeType = ...,
         sortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSharedProjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedprojectspaginator)
         """
 
 class ListSharedReportGroupsPaginator(AioPaginator):
@@ -305,13 +302,13 @@
     """
 
     def paginate(
         self,
         *,
         sortOrder: SortOrderTypeType = ...,
         sortBy: SharedResourceSortByTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSharedReportGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Paginator.ListSharedReportGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/paginators/#listsharedreportgroupspaginator)
         """
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/type_defs.py` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef
 
-    data: BatchDeleteBuildsInputRequestTypeDef = {...}
+    data: BatchDeleteBuildsInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ArtifactNamespaceType,
     ArtifactPackagingType,
     ArtifactsTypeType,
     AuthTypeType,
     BatchReportModeTypeType,
@@ -58,138 +58,146 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
+    "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
-    "ProjectCacheTypeDef",
+    "ProjectCacheOutputTypeDef",
     "ProjectFileSystemLocationTypeDef",
     "ProjectSourceVersionTypeDef",
-    "VpcConfigTypeDef",
+    "VpcConfigOutputTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
+    "ProjectCacheTypeDef",
     "TagTypeDef",
+    "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
-    "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
-    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
-    "GetResourcePolicyOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
-    "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
-    "ListBuildBatchesForProjectOutputTypeDef",
-    "ListBuildBatchesOutputTypeDef",
-    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
     "ListBuildsForProjectInputRequestTypeDef",
-    "ListBuildsForProjectOutputTypeDef",
-    "ListBuildsInputListBuildsPaginateTypeDef",
     "ListBuildsInputRequestTypeDef",
-    "ListBuildsOutputTypeDef",
-    "ListProjectsInputListProjectsPaginateTypeDef",
     "ListProjectsInputRequestTypeDef",
-    "ListProjectsOutputTypeDef",
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
     "ListReportGroupsInputRequestTypeDef",
-    "ListReportGroupsOutputTypeDef",
     "ReportFilterTypeDef",
-    "ListReportsForReportGroupOutputTypeDef",
-    "ListReportsOutputTypeDef",
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
-    "ListSharedProjectsOutputTypeDef",
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
-    "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
     "S3LogsConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectBadgeTypeDef",
     "RegistryCredentialTypeDef",
     "SourceAuthTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
-    "PutResourcePolicyOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
-    "UpdateProjectVisibilityOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
+    "DeleteSourceCredentialsOutputTypeDef",
+    "GetResourcePolicyOutputTypeDef",
+    "ImportSourceCredentialsOutputTypeDef",
+    "ListBuildBatchesForProjectOutputTypeDef",
+    "ListBuildBatchesOutputTypeDef",
+    "ListBuildsForProjectOutputTypeDef",
+    "ListBuildsOutputTypeDef",
+    "ListProjectsOutputTypeDef",
+    "ListReportGroupsOutputTypeDef",
+    "ListReportsForReportGroupOutputTypeDef",
+    "ListReportsOutputTypeDef",
+    "ListSharedProjectsOutputTypeDef",
+    "ListSharedReportGroupsOutputTypeDef",
+    "PutResourcePolicyOutputTypeDef",
+    "UpdateProjectVisibilityOutputTypeDef",
+    "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
+    "ProjectCacheUnionTypeDef",
+    "VpcConfigUnionTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
+    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
     "LogsConfigTypeDef",
     "LogsLocationTypeDef",
+    "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
     "ProjectSourceTypeDef",
     "ReportExportConfigTypeDef",
+    "ProjectBuildBatchConfigUnionTypeDef",
     "BuildGroupTypeDef",
     "CreateWebhookOutputTypeDef",
     "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
+    "ProjectEnvironmentUnionTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
     "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
     "CreateReportGroupInputRequestTypeDef",
@@ -227,14 +235,25 @@
     {
         "id": str,
         "statusCode": str,
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
 BatchGetBuildBatchesInputRequestTypeDef = TypedDict(
     "BatchGetBuildBatchesInputRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -262,19 +281,28 @@
 BatchGetReportsInputRequestTypeDef = TypedDict(
     "BatchGetReportsInputRequestTypeDef",
     {
         "reportArns": Sequence[str],
     },
 )
 
+BatchRestrictionsOutputTypeDef = TypedDict(
+    "BatchRestrictionsOutputTypeDef",
+    {
+        "maximumBuildsAllowed": int,
+        "computeTypesAllowed": List[str],
+    },
+    total=False,
+)
+
 BatchRestrictionsTypeDef = TypedDict(
     "BatchRestrictionsTypeDef",
     {
         "maximumBuildsAllowed": int,
-        "computeTypesAllowed": List[str],
+        "computeTypesAllowed": Sequence[str],
     },
     total=False,
 )
 
 BuildArtifactsTypeDef = TypedDict(
     "BuildArtifactsTypeDef",
     {
@@ -302,34 +330,34 @@
     {
         "statusCode": str,
         "message": str,
     },
     total=False,
 )
 
-_RequiredProjectCacheTypeDef = TypedDict(
-    "_RequiredProjectCacheTypeDef",
+_RequiredProjectCacheOutputTypeDef = TypedDict(
+    "_RequiredProjectCacheOutputTypeDef",
     {
         "type": CacheTypeType,
     },
 )
-_OptionalProjectCacheTypeDef = TypedDict(
-    "_OptionalProjectCacheTypeDef",
+_OptionalProjectCacheOutputTypeDef = TypedDict(
+    "_OptionalProjectCacheOutputTypeDef",
     {
         "location": str,
         "modes": List[CacheModeType],
     },
     total=False,
 )
 
-
-class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+class ProjectCacheOutputTypeDef(
+    _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
+):
     pass
 
-
 ProjectFileSystemLocationTypeDef = TypedDict(
     "ProjectFileSystemLocationTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
@@ -342,16 +370,16 @@
     "ProjectSourceVersionTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
@@ -413,21 +441,19 @@
     {
         "groupName": str,
         "streamName": str,
     },
     total=False,
 )
 
-
 class CloudWatchLogsConfigTypeDef(
     _RequiredCloudWatchLogsConfigTypeDef, _OptionalCloudWatchLogsConfigTypeDef
 ):
     pass
 
-
 CodeCoverageReportSummaryTypeDef = TypedDict(
     "CodeCoverageReportSummaryTypeDef",
     {
         "lineCoveragePercentage": float,
         "linesCovered": int,
         "linesMissed": int,
         "branchCoveragePercentage": float,
@@ -472,28 +498,54 @@
         "encryptionDisabled": bool,
         "artifactIdentifier": str,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
-
 class ProjectArtifactsTypeDef(_RequiredProjectArtifactsTypeDef, _OptionalProjectArtifactsTypeDef):
     pass
 
+_RequiredProjectCacheTypeDef = TypedDict(
+    "_RequiredProjectCacheTypeDef",
+    {
+        "type": CacheTypeType,
+    },
+)
+_OptionalProjectCacheTypeDef = TypedDict(
+    "_OptionalProjectCacheTypeDef",
+    {
+        "location": str,
+        "modes": Sequence[CacheModeType],
+    },
+    total=False,
+)
+
+class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+    pass
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "vpcId": str,
+        "subnets": Sequence[str],
+        "securityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredWebhookFilterTypeDef = TypedDict(
     "_RequiredWebhookFilterTypeDef",
     {
         "type": WebhookFilterTypeType,
         "pattern": str,
     },
 )
@@ -501,19 +553,17 @@
     "_OptionalWebhookFilterTypeDef",
     {
         "excludeMatchedPattern": bool,
     },
     total=False,
 )
 
-
 class WebhookFilterTypeDef(_RequiredWebhookFilterTypeDef, _OptionalWebhookFilterTypeDef):
     pass
 
-
 DeleteBuildBatchInputRequestTypeDef = TypedDict(
     "DeleteBuildBatchInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -534,21 +584,19 @@
     "_OptionalDeleteReportGroupInputRequestTypeDef",
     {
         "deleteReports": bool,
     },
     total=False,
 )
 
-
 class DeleteReportGroupInputRequestTypeDef(
     _RequiredDeleteReportGroupInputRequestTypeDef, _OptionalDeleteReportGroupInputRequestTypeDef
 ):
     pass
 
-
 DeleteReportInputRequestTypeDef = TypedDict(
     "DeleteReportInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -562,55 +610,31 @@
 DeleteSourceCredentialsInputRequestTypeDef = TypedDict(
     "DeleteSourceCredentialsInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteSourceCredentialsOutputTypeDef = TypedDict(
-    "DeleteSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebhookInputRequestTypeDef = TypedDict(
     "DeleteWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "reportArn": str,
-    },
-)
-_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportCodeCoverageSortByTypeType,
-        "minLineCoveragePercentage": float,
-        "maxLineCoveragePercentage": float,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
-    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCodeCoveragesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
@@ -622,22 +646,20 @@
         "sortBy": ReportCodeCoverageSortByTypeType,
         "minLineCoveragePercentage": float,
         "maxLineCoveragePercentage": float,
     },
     total=False,
 )
 
-
 class DescribeCodeCoveragesInputRequestTypeDef(
     _RequiredDescribeCodeCoveragesInputRequestTypeDef,
     _OptionalDescribeCodeCoveragesInputRequestTypeDef,
 ):
     pass
 
-
 TestCaseFilterTypeDef = TypedDict(
     "TestCaseFilterTypeDef",
     {
         "status": str,
         "keyword": str,
     },
     total=False,
@@ -679,21 +701,19 @@
     "_OptionalEnvironmentVariableTypeDef",
     {
         "type": EnvironmentVariableTypeType,
     },
     total=False,
 )
 
-
 class EnvironmentVariableTypeDef(
     _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
-
 _RequiredGetReportGroupTrendInputRequestTypeDef = TypedDict(
     "_RequiredGetReportGroupTrendInputRequestTypeDef",
     {
         "reportGroupArn": str,
         "trendField": ReportGroupTrendFieldTypeType,
     },
 )
@@ -701,21 +721,19 @@
     "_OptionalGetReportGroupTrendInputRequestTypeDef",
     {
         "numOfReports": int,
     },
     total=False,
 )
 
-
 class GetReportGroupTrendInputRequestTypeDef(
     _RequiredGetReportGroupTrendInputRequestTypeDef, _OptionalGetReportGroupTrendInputRequestTypeDef
 ):
     pass
 
-
 ReportGroupTrendStatsTypeDef = TypedDict(
     "ReportGroupTrendStatsTypeDef",
     {
         "average": str,
         "max": str,
         "min": str,
     },
@@ -734,22 +752,14 @@
 GetResourcePolicyInputRequestTypeDef = TypedDict(
     "GetResourcePolicyInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyOutputTypeDef = TypedDict(
-    "GetResourcePolicyOutputTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -766,78 +776,27 @@
     {
         "username": str,
         "shouldOverwrite": bool,
     },
     total=False,
 )
 
-
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
-
-ImportSourceCredentialsOutputTypeDef = TypedDict(
-    "ImportSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-ListBuildBatchesForProjectOutputTypeDef = TypedDict(
-    "ListBuildBatchesForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildBatchesOutputTypeDef = TypedDict(
-    "ListBuildBatchesOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
-    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBuildsForProjectInputRequestTypeDef = TypedDict(
     "_RequiredListBuildsForProjectInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListBuildsForProjectInputRequestTypeDef = TypedDict(
@@ -845,203 +804,80 @@
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
-
-ListBuildsForProjectOutputTypeDef = TypedDict(
-    "ListBuildsForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildsOutputTypeDef = TypedDict(
-    "ListBuildsOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    {
-        "sortBy": ProjectSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "sortBy": ProjectSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsOutputTypeDef = TypedDict(
-    "ListProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportGroupSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReportGroupsInputRequestTypeDef = TypedDict(
     "ListReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": ReportGroupSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListReportGroupsOutputTypeDef = TypedDict(
-    "ListReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportFilterTypeDef = TypedDict(
     "ReportFilterTypeDef",
     {
         "status": ReportStatusTypeType,
     },
     total=False,
 )
 
-ListReportsForReportGroupOutputTypeDef = TypedDict(
-    "ListReportsForReportGroupOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportsOutputTypeDef = TypedDict(
-    "ListReportsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    {
-        "sortBy": SharedResourceSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedProjectsInputRequestTypeDef = TypedDict(
     "ListSharedProjectsInputRequestTypeDef",
     {
         "sortBy": SharedResourceSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSharedProjectsOutputTypeDef = TypedDict(
-    "ListSharedProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": SharedResourceSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedReportGroupsInputRequestTypeDef = TypedDict(
     "ListSharedReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": SharedResourceSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListSharedReportGroupsOutputTypeDef = TypedDict(
-    "ListSharedReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCredentialsInfoTypeDef = TypedDict(
     "SourceCredentialsInfoTypeDef",
     {
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
@@ -1060,29 +896,17 @@
         "location": str,
         "encryptionDisabled": bool,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
-
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
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
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
@@ -1106,35 +930,25 @@
     "_OptionalSourceAuthTypeDef",
     {
         "resource": str,
     },
     total=False,
 )
 
-
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
-
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -1149,25 +963,14 @@
     {
         "total": int,
         "statusCounts": Dict[str, int],
         "durationInNanoSeconds": int,
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
 RetryBuildBatchInputRequestTypeDef = TypedDict(
     "RetryBuildBatchInputRequestTypeDef",
     {
         "id": str,
         "idempotencyToken": str,
         "retryType": RetryBuildBatchTypeType,
     },
@@ -1208,70 +1011,191 @@
     "_OptionalUpdateProjectVisibilityInputRequestTypeDef",
     {
         "resourceAccessRole": str,
     },
     total=False,
 )
 
-
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
-
-UpdateProjectVisibilityOutputTypeDef = TypedDict(
-    "UpdateProjectVisibilityOutputTypeDef",
-    {
-        "projectArn": str,
-        "publicProjectAlias": str,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBuildBatchOutputTypeDef = TypedDict(
     "DeleteBuildBatchOutputTypeDef",
     {
         "statusCode": str,
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectBuildBatchConfigTypeDef = TypedDict(
-    "ProjectBuildBatchConfigTypeDef",
+DeleteSourceCredentialsOutputTypeDef = TypedDict(
+    "DeleteSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyOutputTypeDef = TypedDict(
+    "GetResourcePolicyOutputTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSourceCredentialsOutputTypeDef = TypedDict(
+    "ImportSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildBatchesForProjectOutputTypeDef = TypedDict(
+    "ListBuildBatchesForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildBatchesOutputTypeDef = TypedDict(
+    "ListBuildBatchesOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsForProjectOutputTypeDef = TypedDict(
+    "ListBuildsForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsOutputTypeDef = TypedDict(
+    "ListBuildsOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsOutputTypeDef = TypedDict(
+    "ListProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportGroupsOutputTypeDef = TypedDict(
+    "ListReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsForReportGroupOutputTypeDef = TypedDict(
+    "ListReportsForReportGroupOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsOutputTypeDef = TypedDict(
+    "ListReportsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedProjectsOutputTypeDef = TypedDict(
+    "ListSharedProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedReportGroupsOutputTypeDef = TypedDict(
+    "ListSharedReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectVisibilityOutputTypeDef = TypedDict(
+    "UpdateProjectVisibilityOutputTypeDef",
+    {
+        "projectArn": str,
+        "publicProjectAlias": str,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProjectBuildBatchConfigOutputTypeDef = TypedDict(
+    "ProjectBuildBatchConfigOutputTypeDef",
     {
         "serviceRole": str,
         "combineArtifacts": bool,
-        "restrictions": BatchRestrictionsTypeDef,
+        "restrictions": BatchRestrictionsOutputTypeDef,
         "timeoutInMins": int,
         "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
-ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+ProjectBuildBatchConfigTypeDef = TypedDict(
+    "ProjectBuildBatchConfigTypeDef",
     {
-        "projectName": str,
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "serviceRole": str,
+        "combineArtifacts": bool,
+        "restrictions": BatchRestrictionsTypeDef,
+        "timeoutInMins": int,
+        "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
 ListBuildBatchesForProjectInputRequestTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputRequestTypeDef",
     {
@@ -1280,24 +1204,14 @@
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    {
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildBatchesInputRequestTypeDef = TypedDict(
     "ListBuildBatchesInputRequestTypeDef",
     {
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
@@ -1344,18 +1258,20 @@
 )
 
 DescribeCodeCoveragesOutputTypeDef = TypedDict(
     "DescribeCodeCoveragesOutputTypeDef",
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ProjectCacheUnionTypeDef = Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef]
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalCreateWebhookInputRequestTypeDef = TypedDict(
@@ -1364,21 +1280,19 @@
         "branchFilter": str,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
-
 class CreateWebhookInputRequestTypeDef(
     _RequiredCreateWebhookInputRequestTypeDef, _OptionalCreateWebhookInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateWebhookInputRequestTypeDef = TypedDict(
@@ -1388,58 +1302,169 @@
         "rotateSecret": bool,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
-
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
-
 WebhookTypeDef = TypedDict(
     "WebhookTypeDef",
     {
         "url": str,
         "payloadUrl": str,
         "secret": str,
         "branchFilter": str,
         "filterGroups": List[List[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
         "lastModifiedSecret": datetime,
     },
     total=False,
 )
 
+_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "reportArn": str,
+    },
+)
+_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportCodeCoverageSortByTypeType,
+        "minLineCoveragePercentage": float,
+        "maxLineCoveragePercentage": float,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
+    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+):
+    pass
+
+ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    {
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
+    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+):
+    pass
+
+ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    {
+        "sortBy": ProjectSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportGroupSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    {
+        "sortBy": SharedResourceSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": SharedResourceSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "filter": TestCaseFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTestCasesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputRequestTypeDef = TypedDict(
@@ -1448,27 +1473,25 @@
         "nextToken": str,
         "maxResults": int,
         "filter": TestCaseFilterTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTestCasesInputRequestTypeDef(
     _RequiredDescribeTestCasesInputRequestTypeDef, _OptionalDescribeTestCasesInputRequestTypeDef
 ):
     pass
 
-
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentLanguageTypeDef = TypedDict(
     "EnvironmentLanguageTypeDef",
     {
         "language": LanguageTypeType,
@@ -1478,42 +1501,40 @@
 )
 
 GetReportGroupTrendOutputTypeDef = TypedDict(
     "GetReportGroupTrendOutputTypeDef",
     {
         "stats": ReportGroupTrendStatsTypeDef,
         "rawData": List[ReportWithRawDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListReportsForReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputRequestTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputRequestTypeDef = TypedDict(
@@ -1523,28 +1544,26 @@
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "filter": ReportFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListReportsForReportGroupInputRequestTypeDef(
     _RequiredListReportsForReportGroupInputRequestTypeDef,
     _OptionalListReportsForReportGroupInputRequestTypeDef,
 ):
     pass
 
-
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListReportsInputRequestTypeDef = TypedDict(
     "ListReportsInputRequestTypeDef",
     {
@@ -1556,15 +1575,15 @@
     total=False,
 )
 
 ListSourceCredentialsOutputTypeDef = TypedDict(
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LogsConfigTypeDef = TypedDict(
     "LogsConfigTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
@@ -1584,41 +1603,64 @@
         "s3LogsArn": str,
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredProjectEnvironmentOutputTypeDef = TypedDict(
+    "_RequiredProjectEnvironmentOutputTypeDef",
+    {
+        "type": EnvironmentTypeType,
+        "image": str,
+        "computeType": ComputeTypeType,
+    },
+)
+_OptionalProjectEnvironmentOutputTypeDef = TypedDict(
+    "_OptionalProjectEnvironmentOutputTypeDef",
+    {
+        "environmentVariables": List[EnvironmentVariableTypeDef],
+        "privilegedMode": bool,
+        "certificate": str,
+        "registryCredential": RegistryCredentialTypeDef,
+        "imagePullCredentialsType": ImagePullCredentialsTypeType,
+    },
+    total=False,
+)
+
+class ProjectEnvironmentOutputTypeDef(
+    _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
+):
+    pass
+
 _RequiredProjectEnvironmentTypeDef = TypedDict(
     "_RequiredProjectEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentTypeDef = TypedDict(
     "_OptionalProjectEnvironmentTypeDef",
     {
-        "environmentVariables": List[EnvironmentVariableTypeDef],
+        "environmentVariables": Sequence[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
         "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
-
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
-
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1633,28 +1675,29 @@
         "buildStatusConfig": BuildStatusConfigTypeDef,
         "insecureSsl": bool,
         "sourceIdentifier": str,
     },
     total=False,
 )
 
-
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
-
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
+ProjectBuildBatchConfigUnionTypeDef = Union[
+    ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
+]
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
@@ -1663,35 +1706,36 @@
     total=False,
 )
 
 CreateWebhookOutputTypeDef = TypedDict(
     "CreateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWebhookOutputTypeDef = TypedDict(
     "UpdateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
 )
 
+ProjectEnvironmentUnionTypeDef = Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "id": str,
         "arn": str,
         "buildNumber": int,
         "startTime": datetime,
@@ -1703,23 +1747,23 @@
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "buildComplete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
@@ -1756,48 +1800,46 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
-
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
-
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "sourceVersion": str,
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": ProjectArtifactsTypeDef,
         "secondaryArtifacts": List[ProjectArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "encryptionKey": str,
         "tags": List[TagTypeDef],
         "created": datetime,
         "lastModified": datetime,
         "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "badge": ProjectBadgeTypeDef,
         "logsConfig": LogsConfigTypeDef,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "concurrentBuildLimit": int,
         "projectVisibility": ProjectVisibilityTypeType,
         "publicProjectAlias": str,
         "resourceAccessRole": str,
     },
     total=False,
 )
@@ -1841,21 +1883,19 @@
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "buildBatchConfigOverride": ProjectBuildBatchConfigTypeDef,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
-
 class StartBuildBatchInputRequestTypeDef(
     _RequiredStartBuildBatchInputRequestTypeDef, _OptionalStartBuildBatchInputRequestTypeDef
 ):
     pass
 
-
 _RequiredStartBuildInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildInputRequestTypeDef = TypedDict(
@@ -1891,21 +1931,19 @@
         "registryCredentialOverride": RegistryCredentialTypeDef,
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
-
 class StartBuildInputRequestTypeDef(
     _RequiredStartBuildInputRequestTypeDef, _OptionalStartBuildInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateProjectInputRequestTypeDef = TypedDict(
@@ -1931,21 +1969,19 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
-
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportGroupInputRequestTypeDef",
     {
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
     },
@@ -1954,21 +1990,19 @@
     "_OptionalCreateReportGroupInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateReportGroupInputRequestTypeDef(
     _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
 ):
     pass
 
-
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
@@ -2010,21 +2044,19 @@
     {
         "exportConfig": ReportExportConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
-
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
@@ -2035,158 +2067,158 @@
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logConfig": LogsConfigTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
     "ListCuratedEnvironmentImagesOutputTypeDef",
     {
         "platforms": List[EnvironmentPlatformTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildsOutputTypeDef = TypedDict(
     "BatchGetBuildsOutputTypeDef",
     {
         "builds": List[BuildTypeDef],
         "buildsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildOutputTypeDef = TypedDict(
     "RetryBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildOutputTypeDef = TypedDict(
     "StartBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildOutputTypeDef = TypedDict(
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetProjectsOutputTypeDef = TypedDict(
     "BatchGetProjectsOutputTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "projectsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectOutputTypeDef = TypedDict(
     "CreateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectOutputTypeDef = TypedDict(
     "UpdateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportGroupsOutputTypeDef = TypedDict(
     "BatchGetReportGroupsOutputTypeDef",
     {
         "reportGroups": List[ReportGroupTypeDef],
         "reportGroupsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReportGroupOutputTypeDef = TypedDict(
     "CreateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportGroupOutputTypeDef = TypedDict(
     "UpdateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportsOutputTypeDef = TypedDict(
     "BatchGetReportsOutputTypeDef",
     {
         "reports": List[ReportTypeDef],
         "reportsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
         "buildBatches": List[BuildBatchTypeDef],
         "buildBatchesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildBatchOutputTypeDef = TypedDict(
     "RetryBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildBatchOutputTypeDef = TypedDict(
     "StartBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildBatchOutputTypeDef = TypedDict(
     "StopBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild/type_defs.pyi` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef
 
-    data: BatchDeleteBuildsInputRequestTypeDef = {...}
+    data: BatchDeleteBuildsInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ArtifactNamespaceType,
     ArtifactPackagingType,
     ArtifactsTypeType,
     AuthTypeType,
     BatchReportModeTypeType,
@@ -58,137 +58,147 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
+    "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
-    "ProjectCacheTypeDef",
+    "ProjectCacheOutputTypeDef",
     "ProjectFileSystemLocationTypeDef",
     "ProjectSourceVersionTypeDef",
-    "VpcConfigTypeDef",
+    "VpcConfigOutputTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
+    "ProjectCacheTypeDef",
     "TagTypeDef",
+    "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
-    "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
-    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
-    "GetResourcePolicyOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
-    "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
-    "ListBuildBatchesForProjectOutputTypeDef",
-    "ListBuildBatchesOutputTypeDef",
-    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
     "ListBuildsForProjectInputRequestTypeDef",
-    "ListBuildsForProjectOutputTypeDef",
-    "ListBuildsInputListBuildsPaginateTypeDef",
     "ListBuildsInputRequestTypeDef",
-    "ListBuildsOutputTypeDef",
-    "ListProjectsInputListProjectsPaginateTypeDef",
     "ListProjectsInputRequestTypeDef",
-    "ListProjectsOutputTypeDef",
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
     "ListReportGroupsInputRequestTypeDef",
-    "ListReportGroupsOutputTypeDef",
     "ReportFilterTypeDef",
-    "ListReportsForReportGroupOutputTypeDef",
-    "ListReportsOutputTypeDef",
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
-    "ListSharedProjectsOutputTypeDef",
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
-    "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
     "S3LogsConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectBadgeTypeDef",
     "RegistryCredentialTypeDef",
     "SourceAuthTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
-    "PutResourcePolicyOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
-    "UpdateProjectVisibilityOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
+    "DeleteSourceCredentialsOutputTypeDef",
+    "GetResourcePolicyOutputTypeDef",
+    "ImportSourceCredentialsOutputTypeDef",
+    "ListBuildBatchesForProjectOutputTypeDef",
+    "ListBuildBatchesOutputTypeDef",
+    "ListBuildsForProjectOutputTypeDef",
+    "ListBuildsOutputTypeDef",
+    "ListProjectsOutputTypeDef",
+    "ListReportGroupsOutputTypeDef",
+    "ListReportsForReportGroupOutputTypeDef",
+    "ListReportsOutputTypeDef",
+    "ListSharedProjectsOutputTypeDef",
+    "ListSharedReportGroupsOutputTypeDef",
+    "PutResourcePolicyOutputTypeDef",
+    "UpdateProjectVisibilityOutputTypeDef",
+    "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
+    "ProjectCacheUnionTypeDef",
+    "VpcConfigUnionTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
+    "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
     "LogsConfigTypeDef",
     "LogsLocationTypeDef",
+    "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
     "ProjectSourceTypeDef",
     "ReportExportConfigTypeDef",
+    "ProjectBuildBatchConfigUnionTypeDef",
     "BuildGroupTypeDef",
     "CreateWebhookOutputTypeDef",
     "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
+    "ProjectEnvironmentUnionTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
     "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
     "CreateReportGroupInputRequestTypeDef",
@@ -226,14 +236,25 @@
     {
         "id": str,
         "statusCode": str,
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
 BatchGetBuildBatchesInputRequestTypeDef = TypedDict(
     "BatchGetBuildBatchesInputRequestTypeDef",
     {
         "ids": Sequence[str],
     },
 )
 
@@ -261,19 +282,28 @@
 BatchGetReportsInputRequestTypeDef = TypedDict(
     "BatchGetReportsInputRequestTypeDef",
     {
         "reportArns": Sequence[str],
     },
 )
 
+BatchRestrictionsOutputTypeDef = TypedDict(
+    "BatchRestrictionsOutputTypeDef",
+    {
+        "maximumBuildsAllowed": int,
+        "computeTypesAllowed": List[str],
+    },
+    total=False,
+)
+
 BatchRestrictionsTypeDef = TypedDict(
     "BatchRestrictionsTypeDef",
     {
         "maximumBuildsAllowed": int,
-        "computeTypesAllowed": List[str],
+        "computeTypesAllowed": Sequence[str],
     },
     total=False,
 )
 
 BuildArtifactsTypeDef = TypedDict(
     "BuildArtifactsTypeDef",
     {
@@ -301,32 +331,36 @@
     {
         "statusCode": str,
         "message": str,
     },
     total=False,
 )
 
-_RequiredProjectCacheTypeDef = TypedDict(
-    "_RequiredProjectCacheTypeDef",
+_RequiredProjectCacheOutputTypeDef = TypedDict(
+    "_RequiredProjectCacheOutputTypeDef",
     {
         "type": CacheTypeType,
     },
 )
-_OptionalProjectCacheTypeDef = TypedDict(
-    "_OptionalProjectCacheTypeDef",
+_OptionalProjectCacheOutputTypeDef = TypedDict(
+    "_OptionalProjectCacheOutputTypeDef",
     {
         "location": str,
         "modes": List[CacheModeType],
     },
     total=False,
 )
 
-class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+
+class ProjectCacheOutputTypeDef(
+    _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
+):
     pass
 
+
 ProjectFileSystemLocationTypeDef = TypedDict(
     "ProjectFileSystemLocationTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
@@ -339,16 +373,16 @@
     "ProjectSourceVersionTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
@@ -410,19 +444,21 @@
     {
         "groupName": str,
         "streamName": str,
     },
     total=False,
 )
 
+
 class CloudWatchLogsConfigTypeDef(
     _RequiredCloudWatchLogsConfigTypeDef, _OptionalCloudWatchLogsConfigTypeDef
 ):
     pass
 
+
 CodeCoverageReportSummaryTypeDef = TypedDict(
     "CodeCoverageReportSummaryTypeDef",
     {
         "lineCoveragePercentage": float,
         "linesCovered": int,
         "linesMissed": int,
         "branchCoveragePercentage": float,
@@ -467,26 +503,58 @@
         "encryptionDisabled": bool,
         "artifactIdentifier": str,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
+
 class ProjectArtifactsTypeDef(_RequiredProjectArtifactsTypeDef, _OptionalProjectArtifactsTypeDef):
     pass
 
+
+_RequiredProjectCacheTypeDef = TypedDict(
+    "_RequiredProjectCacheTypeDef",
+    {
+        "type": CacheTypeType,
+    },
+)
+_OptionalProjectCacheTypeDef = TypedDict(
+    "_OptionalProjectCacheTypeDef",
+    {
+        "location": str,
+        "modes": Sequence[CacheModeType],
+    },
+    total=False,
+)
+
+
+class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+    pass
+
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "vpcId": str,
+        "subnets": Sequence[str],
+        "securityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredWebhookFilterTypeDef = TypedDict(
     "_RequiredWebhookFilterTypeDef",
     {
         "type": WebhookFilterTypeType,
         "pattern": str,
     },
 )
@@ -494,17 +562,19 @@
     "_OptionalWebhookFilterTypeDef",
     {
         "excludeMatchedPattern": bool,
     },
     total=False,
 )
 
+
 class WebhookFilterTypeDef(_RequiredWebhookFilterTypeDef, _OptionalWebhookFilterTypeDef):
     pass
 
+
 DeleteBuildBatchInputRequestTypeDef = TypedDict(
     "DeleteBuildBatchInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -525,19 +595,21 @@
     "_OptionalDeleteReportGroupInputRequestTypeDef",
     {
         "deleteReports": bool,
     },
     total=False,
 )
 
+
 class DeleteReportGroupInputRequestTypeDef(
     _RequiredDeleteReportGroupInputRequestTypeDef, _OptionalDeleteReportGroupInputRequestTypeDef
 ):
     pass
 
+
 DeleteReportInputRequestTypeDef = TypedDict(
     "DeleteReportInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -551,53 +623,31 @@
 DeleteSourceCredentialsInputRequestTypeDef = TypedDict(
     "DeleteSourceCredentialsInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteSourceCredentialsOutputTypeDef = TypedDict(
-    "DeleteSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWebhookInputRequestTypeDef = TypedDict(
     "DeleteWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
-    {
-        "reportArn": str,
-    },
-)
-_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportCodeCoverageSortByTypeType,
-        "minLineCoveragePercentage": float,
-        "maxLineCoveragePercentage": float,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
-    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeCodeCoveragesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeCodeCoveragesInputRequestTypeDef = TypedDict(
@@ -609,20 +659,22 @@
         "sortBy": ReportCodeCoverageSortByTypeType,
         "minLineCoveragePercentage": float,
         "maxLineCoveragePercentage": float,
     },
     total=False,
 )
 
+
 class DescribeCodeCoveragesInputRequestTypeDef(
     _RequiredDescribeCodeCoveragesInputRequestTypeDef,
     _OptionalDescribeCodeCoveragesInputRequestTypeDef,
 ):
     pass
 
+
 TestCaseFilterTypeDef = TypedDict(
     "TestCaseFilterTypeDef",
     {
         "status": str,
         "keyword": str,
     },
     total=False,
@@ -664,19 +716,21 @@
     "_OptionalEnvironmentVariableTypeDef",
     {
         "type": EnvironmentVariableTypeType,
     },
     total=False,
 )
 
+
 class EnvironmentVariableTypeDef(
     _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
+
 _RequiredGetReportGroupTrendInputRequestTypeDef = TypedDict(
     "_RequiredGetReportGroupTrendInputRequestTypeDef",
     {
         "reportGroupArn": str,
         "trendField": ReportGroupTrendFieldTypeType,
     },
 )
@@ -684,19 +738,21 @@
     "_OptionalGetReportGroupTrendInputRequestTypeDef",
     {
         "numOfReports": int,
     },
     total=False,
 )
 
+
 class GetReportGroupTrendInputRequestTypeDef(
     _RequiredGetReportGroupTrendInputRequestTypeDef, _OptionalGetReportGroupTrendInputRequestTypeDef
 ):
     pass
 
+
 ReportGroupTrendStatsTypeDef = TypedDict(
     "ReportGroupTrendStatsTypeDef",
     {
         "average": str,
         "max": str,
         "min": str,
     },
@@ -715,22 +771,14 @@
 GetResourcePolicyInputRequestTypeDef = TypedDict(
     "GetResourcePolicyInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyOutputTypeDef = TypedDict(
-    "GetResourcePolicyOutputTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -747,74 +795,29 @@
     {
         "username": str,
         "shouldOverwrite": bool,
     },
     total=False,
 )
 
+
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
-ImportSourceCredentialsOutputTypeDef = TypedDict(
-    "ImportSourceCredentialsOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-ListBuildBatchesForProjectOutputTypeDef = TypedDict(
-    "ListBuildBatchesForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildBatchesOutputTypeDef = TypedDict(
-    "ListBuildBatchesOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
-    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
-    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
-):
-    pass
-
 _RequiredListBuildsForProjectInputRequestTypeDef = TypedDict(
     "_RequiredListBuildsForProjectInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListBuildsForProjectInputRequestTypeDef = TypedDict(
@@ -822,201 +825,82 @@
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
-ListBuildsForProjectOutputTypeDef = TypedDict(
-    "ListBuildsForProjectOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
-    "ListBuildsInputListBuildsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildsOutputTypeDef = TypedDict(
-    "ListBuildsOutputTypeDef",
-    {
-        "ids": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsInputListProjectsPaginateTypeDef",
-    {
-        "sortBy": ProjectSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsInputRequestTypeDef = TypedDict(
     "ListProjectsInputRequestTypeDef",
     {
         "sortBy": ProjectSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsOutputTypeDef = TypedDict(
-    "ListProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
-    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": ReportGroupSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReportGroupsInputRequestTypeDef = TypedDict(
     "ListReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": ReportGroupSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListReportGroupsOutputTypeDef = TypedDict(
-    "ListReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReportFilterTypeDef = TypedDict(
     "ReportFilterTypeDef",
     {
         "status": ReportStatusTypeType,
     },
     total=False,
 )
 
-ListReportsForReportGroupOutputTypeDef = TypedDict(
-    "ListReportsForReportGroupOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportsOutputTypeDef = TypedDict(
-    "ListReportsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
-    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
-    {
-        "sortBy": SharedResourceSortByTypeType,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedProjectsInputRequestTypeDef = TypedDict(
     "ListSharedProjectsInputRequestTypeDef",
     {
         "sortBy": SharedResourceSortByTypeType,
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSharedProjectsOutputTypeDef = TypedDict(
-    "ListSharedProjectsOutputTypeDef",
-    {
-        "nextToken": str,
-        "projects": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
-    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
-    {
-        "sortOrder": SortOrderTypeType,
-        "sortBy": SharedResourceSortByTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSharedReportGroupsInputRequestTypeDef = TypedDict(
     "ListSharedReportGroupsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "sortBy": SharedResourceSortByTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListSharedReportGroupsOutputTypeDef = TypedDict(
-    "ListSharedReportGroupsOutputTypeDef",
-    {
-        "nextToken": str,
-        "reportGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCredentialsInfoTypeDef = TypedDict(
     "SourceCredentialsInfoTypeDef",
     {
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
@@ -1035,26 +919,18 @@
         "location": str,
         "encryptionDisabled": bool,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
+
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
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
 
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
@@ -1079,33 +955,27 @@
     "_OptionalSourceAuthTypeDef",
     {
         "resource": str,
     },
     total=False,
 )
 
+
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
+
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -1120,25 +990,14 @@
     {
         "total": int,
         "statusCounts": Dict[str, int],
         "durationInNanoSeconds": int,
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
 RetryBuildBatchInputRequestTypeDef = TypedDict(
     "RetryBuildBatchInputRequestTypeDef",
     {
         "id": str,
         "idempotencyToken": str,
         "retryType": RetryBuildBatchTypeType,
     },
@@ -1179,68 +1038,193 @@
     "_OptionalUpdateProjectVisibilityInputRequestTypeDef",
     {
         "resourceAccessRole": str,
     },
     total=False,
 )
 
+
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
-UpdateProjectVisibilityOutputTypeDef = TypedDict(
-    "UpdateProjectVisibilityOutputTypeDef",
-    {
-        "projectArn": str,
-        "publicProjectAlias": str,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBuildBatchOutputTypeDef = TypedDict(
     "DeleteBuildBatchOutputTypeDef",
     {
         "statusCode": str,
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectBuildBatchConfigTypeDef = TypedDict(
-    "ProjectBuildBatchConfigTypeDef",
+DeleteSourceCredentialsOutputTypeDef = TypedDict(
+    "DeleteSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyOutputTypeDef = TypedDict(
+    "GetResourcePolicyOutputTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSourceCredentialsOutputTypeDef = TypedDict(
+    "ImportSourceCredentialsOutputTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildBatchesForProjectOutputTypeDef = TypedDict(
+    "ListBuildBatchesForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildBatchesOutputTypeDef = TypedDict(
+    "ListBuildBatchesOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsForProjectOutputTypeDef = TypedDict(
+    "ListBuildsForProjectOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBuildsOutputTypeDef = TypedDict(
+    "ListBuildsOutputTypeDef",
+    {
+        "ids": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsOutputTypeDef = TypedDict(
+    "ListProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportGroupsOutputTypeDef = TypedDict(
+    "ListReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsForReportGroupOutputTypeDef = TypedDict(
+    "ListReportsForReportGroupOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportsOutputTypeDef = TypedDict(
+    "ListReportsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedProjectsOutputTypeDef = TypedDict(
+    "ListSharedProjectsOutputTypeDef",
+    {
+        "nextToken": str,
+        "projects": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSharedReportGroupsOutputTypeDef = TypedDict(
+    "ListSharedReportGroupsOutputTypeDef",
+    {
+        "nextToken": str,
+        "reportGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectVisibilityOutputTypeDef = TypedDict(
+    "UpdateProjectVisibilityOutputTypeDef",
+    {
+        "projectArn": str,
+        "publicProjectAlias": str,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProjectBuildBatchConfigOutputTypeDef = TypedDict(
+    "ProjectBuildBatchConfigOutputTypeDef",
     {
         "serviceRole": str,
         "combineArtifacts": bool,
-        "restrictions": BatchRestrictionsTypeDef,
+        "restrictions": BatchRestrictionsOutputTypeDef,
         "timeoutInMins": int,
         "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
-ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
-    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+ProjectBuildBatchConfigTypeDef = TypedDict(
+    "ProjectBuildBatchConfigTypeDef",
     {
-        "projectName": str,
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "serviceRole": str,
+        "combineArtifacts": bool,
+        "restrictions": BatchRestrictionsTypeDef,
+        "timeoutInMins": int,
+        "batchReportMode": BatchReportModeTypeType,
     },
     total=False,
 )
 
 ListBuildBatchesForProjectInputRequestTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputRequestTypeDef",
     {
@@ -1249,24 +1233,14 @@
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
-    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
-    {
-        "filter": BuildBatchFilterTypeDef,
-        "sortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBuildBatchesInputRequestTypeDef = TypedDict(
     "ListBuildBatchesInputRequestTypeDef",
     {
         "filter": BuildBatchFilterTypeDef,
         "maxResults": int,
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
@@ -1313,18 +1287,20 @@
 )
 
 DescribeCodeCoveragesOutputTypeDef = TypedDict(
     "DescribeCodeCoveragesOutputTypeDef",
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ProjectCacheUnionTypeDef = Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef]
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalCreateWebhookInputRequestTypeDef = TypedDict(
@@ -1333,19 +1309,21 @@
         "branchFilter": str,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
+
 class CreateWebhookInputRequestTypeDef(
     _RequiredCreateWebhookInputRequestTypeDef, _OptionalCreateWebhookInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateWebhookInputRequestTypeDef = TypedDict(
@@ -1355,54 +1333,177 @@
         "rotateSecret": bool,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
+
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
+
 WebhookTypeDef = TypedDict(
     "WebhookTypeDef",
     {
         "url": str,
         "payloadUrl": str,
         "secret": str,
         "branchFilter": str,
         "filterGroups": List[List[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
         "lastModifiedSecret": datetime,
     },
     total=False,
 )
 
+_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "reportArn": str,
+    },
+)
+_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportCodeCoverageSortByTypeType,
+        "minLineCoveragePercentage": float,
+        "maxLineCoveragePercentage": float,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
+    _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+):
+    pass
+
+
+ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
+    "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBuildBatchesInputListBuildBatchesPaginateTypeDef = TypedDict(
+    "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
+    {
+        "filter": BuildBatchFilterTypeDef,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef = TypedDict(
+    "_OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
+    _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+):
+    pass
+
+
+ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
+    "ListBuildsInputListBuildsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsInputListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsInputListProjectsPaginateTypeDef",
+    {
+        "sortBy": ProjectSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReportGroupsInputListReportGroupsPaginateTypeDef = TypedDict(
+    "ListReportGroupsInputListReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": ReportGroupSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedProjectsInputListSharedProjectsPaginateTypeDef = TypedDict(
+    "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
+    {
+        "sortBy": SharedResourceSortByTypeType,
+        "sortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef = TypedDict(
+    "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
+    {
+        "sortOrder": SortOrderTypeType,
+        "sortBy": SharedResourceSortByTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "filter": TestCaseFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTestCasesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputRequestTypeDef = TypedDict(
@@ -1411,25 +1512,27 @@
         "nextToken": str,
         "maxResults": int,
         "filter": TestCaseFilterTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTestCasesInputRequestTypeDef(
     _RequiredDescribeTestCasesInputRequestTypeDef, _OptionalDescribeTestCasesInputRequestTypeDef
 ):
     pass
 
+
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentLanguageTypeDef = TypedDict(
     "EnvironmentLanguageTypeDef",
     {
         "language": LanguageTypeType,
@@ -1439,40 +1542,42 @@
 )
 
 GetReportGroupTrendOutputTypeDef = TypedDict(
     "GetReportGroupTrendOutputTypeDef",
     {
         "stats": ReportGroupTrendStatsTypeDef,
         "rawData": List[ReportWithRawDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef = TypedDict(
     "_OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListReportsForReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputRequestTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputRequestTypeDef = TypedDict(
@@ -1482,26 +1587,28 @@
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "filter": ReportFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListReportsForReportGroupInputRequestTypeDef(
     _RequiredListReportsForReportGroupInputRequestTypeDef,
     _OptionalListReportsForReportGroupInputRequestTypeDef,
 ):
     pass
 
+
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListReportsInputRequestTypeDef = TypedDict(
     "ListReportsInputRequestTypeDef",
     {
@@ -1513,15 +1620,15 @@
     total=False,
 )
 
 ListSourceCredentialsOutputTypeDef = TypedDict(
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LogsConfigTypeDef = TypedDict(
     "LogsConfigTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
@@ -1541,39 +1648,68 @@
         "s3LogsArn": str,
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredProjectEnvironmentOutputTypeDef = TypedDict(
+    "_RequiredProjectEnvironmentOutputTypeDef",
+    {
+        "type": EnvironmentTypeType,
+        "image": str,
+        "computeType": ComputeTypeType,
+    },
+)
+_OptionalProjectEnvironmentOutputTypeDef = TypedDict(
+    "_OptionalProjectEnvironmentOutputTypeDef",
+    {
+        "environmentVariables": List[EnvironmentVariableTypeDef],
+        "privilegedMode": bool,
+        "certificate": str,
+        "registryCredential": RegistryCredentialTypeDef,
+        "imagePullCredentialsType": ImagePullCredentialsTypeType,
+    },
+    total=False,
+)
+
+
+class ProjectEnvironmentOutputTypeDef(
+    _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
+):
+    pass
+
+
 _RequiredProjectEnvironmentTypeDef = TypedDict(
     "_RequiredProjectEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentTypeDef = TypedDict(
     "_OptionalProjectEnvironmentTypeDef",
     {
-        "environmentVariables": List[EnvironmentVariableTypeDef],
+        "environmentVariables": Sequence[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
         "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
+
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
+
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1588,26 +1724,31 @@
         "buildStatusConfig": BuildStatusConfigTypeDef,
         "insecureSsl": bool,
         "sourceIdentifier": str,
     },
     total=False,
 )
 
+
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
+
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
+ProjectBuildBatchConfigUnionTypeDef = Union[
+    ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
+]
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
@@ -1616,35 +1757,36 @@
     total=False,
 )
 
 CreateWebhookOutputTypeDef = TypedDict(
     "CreateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWebhookOutputTypeDef = TypedDict(
     "UpdateWebhookOutputTypeDef",
     {
         "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
 )
 
+ProjectEnvironmentUnionTypeDef = Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "id": str,
         "arn": str,
         "buildNumber": int,
         "startTime": datetime,
@@ -1656,23 +1798,23 @@
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "buildComplete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
@@ -1709,46 +1851,48 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
+
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
+
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "sourceVersion": str,
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": ProjectArtifactsTypeDef,
         "secondaryArtifacts": List[ProjectArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "encryptionKey": str,
         "tags": List[TagTypeDef],
         "created": datetime,
         "lastModified": datetime,
         "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "badge": ProjectBadgeTypeDef,
         "logsConfig": LogsConfigTypeDef,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "concurrentBuildLimit": int,
         "projectVisibility": ProjectVisibilityTypeType,
         "publicProjectAlias": str,
         "resourceAccessRole": str,
     },
     total=False,
 )
@@ -1792,19 +1936,21 @@
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "buildBatchConfigOverride": ProjectBuildBatchConfigTypeDef,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
+
 class StartBuildBatchInputRequestTypeDef(
     _RequiredStartBuildBatchInputRequestTypeDef, _OptionalStartBuildBatchInputRequestTypeDef
 ):
     pass
 
+
 _RequiredStartBuildInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildInputRequestTypeDef = TypedDict(
@@ -1840,19 +1986,21 @@
         "registryCredentialOverride": RegistryCredentialTypeDef,
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
+
 class StartBuildInputRequestTypeDef(
     _RequiredStartBuildInputRequestTypeDef, _OptionalStartBuildInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateProjectInputRequestTypeDef = TypedDict(
@@ -1878,19 +2026,21 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
+
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportGroupInputRequestTypeDef",
     {
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
     },
@@ -1899,19 +2049,21 @@
     "_OptionalCreateReportGroupInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateReportGroupInputRequestTypeDef(
     _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
 ):
     pass
 
+
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
@@ -1953,19 +2105,21 @@
     {
         "exportConfig": ReportExportConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
+
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
@@ -1976,158 +2130,158 @@
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logConfig": LogsConfigTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
     "ListCuratedEnvironmentImagesOutputTypeDef",
     {
         "platforms": List[EnvironmentPlatformTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildsOutputTypeDef = TypedDict(
     "BatchGetBuildsOutputTypeDef",
     {
         "builds": List[BuildTypeDef],
         "buildsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildOutputTypeDef = TypedDict(
     "RetryBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildOutputTypeDef = TypedDict(
     "StartBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildOutputTypeDef = TypedDict(
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetProjectsOutputTypeDef = TypedDict(
     "BatchGetProjectsOutputTypeDef",
     {
         "projects": List[ProjectTypeDef],
         "projectsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectOutputTypeDef = TypedDict(
     "CreateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectOutputTypeDef = TypedDict(
     "UpdateProjectOutputTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportGroupsOutputTypeDef = TypedDict(
     "BatchGetReportGroupsOutputTypeDef",
     {
         "reportGroups": List[ReportGroupTypeDef],
         "reportGroupsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReportGroupOutputTypeDef = TypedDict(
     "CreateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportGroupOutputTypeDef = TypedDict(
     "UpdateReportGroupOutputTypeDef",
     {
         "reportGroup": ReportGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetReportsOutputTypeDef = TypedDict(
     "BatchGetReportsOutputTypeDef",
     {
         "reports": List[ReportTypeDef],
         "reportsNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
         "buildBatches": List[BuildBatchTypeDef],
         "buildBatchesNotFound": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RetryBuildBatchOutputTypeDef = TypedDict(
     "RetryBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBuildBatchOutputTypeDef = TypedDict(
     "StartBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBuildBatchOutputTypeDef = TypedDict(
     "StopBuildBatchOutputTypeDef",
     {
         "buildBatch": BuildBatchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/PKG-INFO` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codebuild
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codebuild type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codebuild type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codebuild"></a>
 
 # types-aiobotocore-codebuild
 
 [![PyPI - types-aiobotocore-codebuild](https://img.shields.io/pypi/v/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codebuild.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codebuild)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codebuild?color=blue)](https://pypistats.org/packages/types-aiobotocore-codebuild)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codebuild)](https://pepy.tech/project/types-aiobotocore-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeBuild 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [types-aiobotocore-codebuild docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/).
 
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
@@ -396,145 +395,154 @@
 )
 
 
 def check_value(value: ArtifactNamespaceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codebuild.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
+    BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
-    ProjectCacheTypeDef,
+    ProjectCacheOutputTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceVersionTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
+    ProjectCacheTypeDef,
     TagTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
-    DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
-    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
-    GetResourcePolicyOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
-    ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
-    ListBuildBatchesForProjectOutputTypeDef,
-    ListBuildBatchesOutputTypeDef,
-    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     ListBuildsForProjectInputRequestTypeDef,
-    ListBuildsForProjectOutputTypeDef,
-    ListBuildsInputListBuildsPaginateTypeDef,
     ListBuildsInputRequestTypeDef,
-    ListBuildsOutputTypeDef,
-    ListProjectsInputListProjectsPaginateTypeDef,
     ListProjectsInputRequestTypeDef,
-    ListProjectsOutputTypeDef,
-    ListReportGroupsInputListReportGroupsPaginateTypeDef,
     ListReportGroupsInputRequestTypeDef,
-    ListReportGroupsOutputTypeDef,
     ReportFilterTypeDef,
-    ListReportsForReportGroupOutputTypeDef,
-    ListReportsOutputTypeDef,
-    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
-    ListSharedProjectsOutputTypeDef,
-    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
-    ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
     S3LogsConfigTypeDef,
-    PaginatorConfigTypeDef,
     ProjectBadgeTypeDef,
     RegistryCredentialTypeDef,
     SourceAuthTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
-    ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
-    UpdateProjectVisibilityOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    DeleteSourceCredentialsOutputTypeDef,
+    GetResourcePolicyOutputTypeDef,
+    ImportSourceCredentialsOutputTypeDef,
+    ListBuildBatchesForProjectOutputTypeDef,
+    ListBuildBatchesOutputTypeDef,
+    ListBuildsForProjectOutputTypeDef,
+    ListBuildsOutputTypeDef,
+    ListProjectsOutputTypeDef,
+    ListReportGroupsOutputTypeDef,
+    ListReportsForReportGroupOutputTypeDef,
+    ListReportsOutputTypeDef,
+    ListSharedProjectsOutputTypeDef,
+    ListSharedReportGroupsOutputTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    UpdateProjectVisibilityOutputTypeDef,
+    ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
-    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
-    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
+    ProjectCacheUnionTypeDef,
+    VpcConfigUnionTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
+    DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
+    ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
+    ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
+    ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
+    ListBuildsInputListBuildsPaginateTypeDef,
+    ListProjectsInputListProjectsPaginateTypeDef,
+    ListReportGroupsInputListReportGroupsPaginateTypeDef,
+    ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
+    ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     LogsLocationTypeDef,
+    ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
     ProjectSourceTypeDef,
     ReportExportConfigTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
     BuildGroupTypeDef,
     CreateWebhookOutputTypeDef,
     UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
     ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
     CreateReportGroupInputRequestTypeDef,
@@ -557,15 +565,15 @@
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteBuildsInputRequestTypeDef:
+def get_value() -> BatchDeleteBuildsInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codebuild-2.5.2/types_aiobotocore_codebuild.egg-info/SOURCES.txt` & `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*


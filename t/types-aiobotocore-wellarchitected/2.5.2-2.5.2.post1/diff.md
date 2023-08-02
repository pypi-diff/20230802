# Comparing `tmp/types-aiobotocore-wellarchitected-2.5.2.tar.gz` & `tmp/types-aiobotocore-wellarchitected-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wellarchitected-2.5.2.tar", last modified: Sat Jul  8 01:44:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-wellarchitected-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
```

## Comparing `types-aiobotocore-wellarchitected-2.5.2.tar` & `types-aiobotocore-wellarchitected-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.143046 types-aiobotocore-wellarchitected-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-07-08 01:44:28.143046 types-aiobotocore-wellarchitected-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:28.143046 types-aiobotocore-wellarchitected-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.135046 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40458 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40394 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53133 2023-07-08 01:42:36.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53076 2023-07-08 01:42:35.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:32.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:28.143046 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-07-08 01:44:27.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:44:27.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:27.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:44:27.000000 types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40473 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40409 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53538 2023-08-02 14:51:11.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53481 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/LICENSE` & `types-aiobotocore-wellarchitected-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wellarchitected-2.5.2/PKG-INFO` & `types-aiobotocore-wellarchitected-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wellarchitected
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WellArchitected 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WellArchitected 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore wellarchitected type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-wellarchitected"></a>
 
 # types-aiobotocore-wellarchitected
 
 [![PyPI - types-aiobotocore-wellarchitected](https://img.shields.io/pypi/v/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wellarchitected?color=blue)](https://pypistats.org/packages/types-aiobotocore-wellarchitected)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wellarchitected)](https://pepy.tech/project/types-aiobotocore-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WellArchitected 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [types-aiobotocore-wellarchitected docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/).
 
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
@@ -310,71 +309,62 @@
 )
 
 
 def check_value(value: AdditionalResourceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wellarchitected.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
     AssociateProfilesInputRequestTypeDef,
     BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
-    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    CreateMilestoneOutputTypeDef,
     ProfileQuestionUpdateTypeDef,
-    CreateProfileOutputTypeDef,
     CreateProfileShareInputRequestTypeDef,
-    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
-    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
-    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteProfileInputRequestTypeDef,
     DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     DisassociateProfilesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
-    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
     GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
     GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    ImportLensOutputTypeDef,
     WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
@@ -390,94 +380,105 @@
     ListProfileSharesInputRequestTypeDef,
     ProfileShareSummaryTypeDef,
     ListProfilesInputRequestTypeDef,
     ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
     QuestionDifferenceTypeDef,
     ProfileChoiceTypeDef,
     ProfileTemplateChoiceTypeDef,
-    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     UpgradeProfileVersionInputRequestTypeDef,
+    WorkloadDiscoveryConfigOutputTypeDef,
     AdditionalResourcesTypeDef,
     QuestionMetricTypeDef,
-    ListCheckDetailsOutputTypeDef,
-    ListCheckSummariesOutputTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
+    CreateLensShareOutputTypeDef,
+    CreateLensVersionOutputTypeDef,
+    CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
+    CreateWorkloadOutputTypeDef,
+    CreateWorkloadShareOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportLensOutputTypeDef,
+    ImportLensOutputTypeDef,
+    ListCheckDetailsOutputTypeDef,
+    ListCheckSummariesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateProfileInputRequestTypeDef,
     UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     LensReviewSummaryTypeDef,
     WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
     ListProfileNotificationsOutputTypeDef,
     ListProfileSharesOutputTypeDef,
     ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
+    WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
-    GetWorkloadOutputTypeDef,
-    MilestoneTypeDef,
-    UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     VersionDifferencesTypeDef,
     ProfileTypeDef,
     ProfileTemplateTypeDef,
+    GetWorkloadOutputTypeDef,
+    MilestoneTypeDef,
+    UpdateWorkloadOutputTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
     LensMetricTypeDef,
     ListMilestonesOutputTypeDef,
-    GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetProfileOutputTypeDef,
     UpdateProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
+    GetMilestoneOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
 
 
-def get_structure() -> ChoiceContentTypeDef:
+def get_value() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/README.md` & `types-aiobotocore-wellarchitected-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-wellarchitected"></a>
 
 # types-aiobotocore-wellarchitected
 
 [![PyPI - types-aiobotocore-wellarchitected](https://img.shields.io/pypi/v/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wellarchitected?color=blue)](https://pypistats.org/packages/types-aiobotocore-wellarchitected)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wellarchitected)](https://pepy.tech/project/types-aiobotocore-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WellArchitected 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [types-aiobotocore-wellarchitected docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/).
 
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
@@ -277,71 +277,62 @@
 )
 
 
 def check_value(value: AdditionalResourceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wellarchitected.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
     AssociateProfilesInputRequestTypeDef,
     BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
-    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    CreateMilestoneOutputTypeDef,
     ProfileQuestionUpdateTypeDef,
-    CreateProfileOutputTypeDef,
     CreateProfileShareInputRequestTypeDef,
-    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
-    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
-    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteProfileInputRequestTypeDef,
     DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     DisassociateProfilesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
-    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
     GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
     GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    ImportLensOutputTypeDef,
     WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
@@ -357,94 +348,105 @@
     ListProfileSharesInputRequestTypeDef,
     ProfileShareSummaryTypeDef,
     ListProfilesInputRequestTypeDef,
     ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
     QuestionDifferenceTypeDef,
     ProfileChoiceTypeDef,
     ProfileTemplateChoiceTypeDef,
-    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     UpgradeProfileVersionInputRequestTypeDef,
+    WorkloadDiscoveryConfigOutputTypeDef,
     AdditionalResourcesTypeDef,
     QuestionMetricTypeDef,
-    ListCheckDetailsOutputTypeDef,
-    ListCheckSummariesOutputTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
+    CreateLensShareOutputTypeDef,
+    CreateLensVersionOutputTypeDef,
+    CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
+    CreateWorkloadOutputTypeDef,
+    CreateWorkloadShareOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportLensOutputTypeDef,
+    ImportLensOutputTypeDef,
+    ListCheckDetailsOutputTypeDef,
+    ListCheckSummariesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateProfileInputRequestTypeDef,
     UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     LensReviewSummaryTypeDef,
     WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
     ListProfileNotificationsOutputTypeDef,
     ListProfileSharesOutputTypeDef,
     ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
+    WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
-    GetWorkloadOutputTypeDef,
-    MilestoneTypeDef,
-    UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     VersionDifferencesTypeDef,
     ProfileTypeDef,
     ProfileTemplateTypeDef,
+    GetWorkloadOutputTypeDef,
+    MilestoneTypeDef,
+    UpdateWorkloadOutputTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
     LensMetricTypeDef,
     ListMilestonesOutputTypeDef,
-    GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetProfileOutputTypeDef,
     UpdateProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
+    GetMilestoneOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
 
 
-def get_structure() -> ChoiceContentTypeDef:
+def get_value() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/setup.py` & `types-aiobotocore-wellarchitected-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wellarchitected",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WellArchitected 2.5.2 service generated with"
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
-    keywords="aiobotocore wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore wellarchitected type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_wellarchitected": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/"
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/__main__.py` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WellArchitected 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.WellArchitected 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
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

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/client.py` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
-    WorkloadDiscoveryConfigTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -233,15 +233,15 @@
         PillarPriorities: Sequence[str] = ...,
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
@@ -815,15 +815,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_workload)
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/client.pyi` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
-    WorkloadDiscoveryConfigTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -220,15 +220,15 @@
         PillarPriorities: Sequence[str] = ...,
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
@@ -756,15 +756,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
         Applications: Sequence[str] = ...
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_workload)
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/literals.py` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/literals.pyi` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/type_defs.py` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_wellarchitected.type_defs import ChoiceContentTypeDef
 
-    data: ChoiceContentTypeDef = {...}
+    data: ChoiceContentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
@@ -64,51 +64,42 @@
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
-    "CreateLensShareOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
-    "CreateLensVersionOutputTypeDef",
     "CreateMilestoneInputRequestTypeDef",
-    "CreateMilestoneOutputTypeDef",
     "ProfileQuestionUpdateTypeDef",
-    "CreateProfileOutputTypeDef",
     "CreateProfileShareInputRequestTypeDef",
-    "CreateProfileShareOutputTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
-    "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
-    "CreateWorkloadShareOutputTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteProfileInputRequestTypeDef",
     "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
     "DisassociateProfilesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportLensInputRequestTypeDef",
-    "ExportLensOutputTypeDef",
     "GetAnswerInputRequestTypeDef",
     "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
     "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "ImportLensOutputTypeDef",
     "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
@@ -124,85 +115,96 @@
     "ListProfileSharesInputRequestTypeDef",
     "ProfileShareSummaryTypeDef",
     "ListProfilesInputRequestTypeDef",
     "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
     "QuestionDifferenceTypeDef",
     "ProfileChoiceTypeDef",
     "ProfileTemplateChoiceTypeDef",
-    "ResponseMetadataTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
+    "WorkloadDiscoveryConfigOutputTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
-    "ListCheckDetailsOutputTypeDef",
-    "ListCheckSummariesOutputTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
+    "CreateLensShareOutputTypeDef",
+    "CreateLensVersionOutputTypeDef",
+    "CreateMilestoneOutputTypeDef",
+    "CreateProfileOutputTypeDef",
+    "CreateProfileShareOutputTypeDef",
+    "CreateWorkloadOutputTypeDef",
+    "CreateWorkloadShareOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportLensOutputTypeDef",
+    "ImportLensOutputTypeDef",
+    "ListCheckDetailsOutputTypeDef",
+    "ListCheckSummariesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "CreateProfileInputRequestTypeDef",
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadDiscoveryConfigUnionTypeDef",
+    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "LensMetricTypeDef",
     "ListMilestonesOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
@@ -334,19 +336,22 @@
     {
         "LensAlias": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateLensShareOutputTypeDef = TypedDict(
-    "CreateLensShareOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLensVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
@@ -365,114 +370,60 @@
 
 class CreateLensVersionInputRequestTypeDef(
     _RequiredCreateLensVersionInputRequestTypeDef, _OptionalCreateLensVersionInputRequestTypeDef
 ):
     pass
 
 
-CreateLensVersionOutputTypeDef = TypedDict(
-    "CreateLensVersionOutputTypeDef",
-    {
-        "LensArn": str,
-        "LensVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMilestoneInputRequestTypeDef = TypedDict(
     "CreateMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateMilestoneOutputTypeDef = TypedDict(
-    "CreateMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ProfileQuestionUpdateTypeDef = TypedDict(
     "ProfileQuestionUpdateTypeDef",
     {
         "QuestionId": str,
         "SelectedChoiceIds": Sequence[str],
     },
     total=False,
 )
 
-CreateProfileOutputTypeDef = TypedDict(
-    "CreateProfileOutputTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProfileShareInputRequestTypeDef = TypedDict(
     "CreateProfileShareInputRequestTypeDef",
     {
         "ProfileArn": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateProfileShareOutputTypeDef = TypedDict(
-    "CreateProfileShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
         "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
-CreateWorkloadOutputTypeDef = TypedDict(
-    "CreateWorkloadOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
     },
 )
 
-CreateWorkloadShareOutputTypeDef = TypedDict(
-    "CreateWorkloadShareOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLensInputRequestTypeDef = TypedDict(
     "DeleteLensInputRequestTypeDef",
     {
         "LensAlias": str,
         "ClientRequestToken": str,
         "LensStatus": LensStatusTypeType,
     },
@@ -533,21 +484,14 @@
     "DisassociateProfilesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ProfileArns": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
@@ -561,22 +505,14 @@
 
 class ExportLensInputRequestTypeDef(
     _RequiredExportLensInputRequestTypeDef, _OptionalExportLensInputRequestTypeDef
 ):
     pass
 
 
-ExportLensOutputTypeDef = TypedDict(
-    "ExportLensOutputTypeDef",
-    {
-        "LensJSON": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetAnswerInputRequestTypeDef = TypedDict(
     "_RequiredGetAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "QuestionId": str,
     },
@@ -787,23 +723,14 @@
 
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
 
-ImportLensOutputTypeDef = TypedDict(
-    "ImportLensOutputTypeDef",
-    {
-        "LensArn": str,
-        "Status": ImportLensStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadProfileTypeDef = TypedDict(
     "WorkloadProfileTypeDef",
     {
         "ProfileArn": str,
         "ProfileVersion": str,
     },
     total=False,
@@ -1176,22 +1103,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWorkloadSharesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkloadSharesInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListWorkloadSharesInputRequestTypeDef = TypedDict(
@@ -1260,25 +1179,14 @@
         "ChoiceId": str,
         "ChoiceTitle": str,
         "ChoiceDescription": str,
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
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
@@ -1410,14 +1318,23 @@
 class UpgradeProfileVersionInputRequestTypeDef(
     _RequiredUpgradeProfileVersionInputRequestTypeDef,
     _OptionalUpgradeProfileVersionInputRequestTypeDef,
 ):
     pass
 
 
+WorkloadDiscoveryConfigOutputTypeDef = TypedDict(
+    "WorkloadDiscoveryConfigOutputTypeDef",
+    {
+        "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
+        "WorkloadResourceDefinition": List[DefinitionTypeType],
+    },
+    total=False,
+)
+
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
@@ -1429,32 +1346,14 @@
         "QuestionId": str,
         "Risk": RiskType,
         "BestPractices": List[BestPracticeTypeDef],
     },
     total=False,
 )
 
-ListCheckDetailsOutputTypeDef = TypedDict(
-    "ListCheckDetailsOutputTypeDef",
-    {
-        "CheckDetails": List[CheckDetailTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCheckSummariesOutputTypeDef = TypedDict(
-    "ListCheckSummariesOutputTypeDef",
-    {
-        "CheckSummaries": List[CheckSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1487,14 +1386,126 @@
 
 class UpdateAnswerInputRequestTypeDef(
     _RequiredUpdateAnswerInputRequestTypeDef, _OptionalUpdateAnswerInputRequestTypeDef
 ):
     pass
 
 
+CreateLensShareOutputTypeDef = TypedDict(
+    "CreateLensShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLensVersionOutputTypeDef = TypedDict(
+    "CreateLensVersionOutputTypeDef",
+    {
+        "LensArn": str,
+        "LensVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMilestoneOutputTypeDef = TypedDict(
+    "CreateMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileOutputTypeDef = TypedDict(
+    "CreateProfileOutputTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileShareOutputTypeDef = TypedDict(
+    "CreateProfileShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadOutputTypeDef = TypedDict(
+    "CreateWorkloadOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadShareOutputTypeDef = TypedDict(
+    "CreateWorkloadShareOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "ShareId": str,
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
+ExportLensOutputTypeDef = TypedDict(
+    "ExportLensOutputTypeDef",
+    {
+        "LensJSON": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportLensOutputTypeDef = TypedDict(
+    "ImportLensOutputTypeDef",
+    {
+        "LensArn": str,
+        "Status": ImportLensStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckDetailsOutputTypeDef = TypedDict(
+    "ListCheckDetailsOutputTypeDef",
+    {
+        "CheckDetails": List[CheckDetailTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckSummariesOutputTypeDef = TypedDict(
+    "ListCheckSummariesOutputTypeDef",
+    {
+        "CheckSummaries": List[CheckSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateProfileInputRequestTypeDef = TypedDict(
     "_RequiredCreateProfileInputRequestTypeDef",
     {
         "ProfileName": str,
         "ProfileDescription": str,
         "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
         "ClientRequestToken": str,
@@ -1610,25 +1621,25 @@
     pass
 
 
 GetLensOutputTypeDef = TypedDict(
     "GetLensOutputTypeDef",
     {
         "Lens": LensTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensReviewReportOutputTypeDef = TypedDict(
     "GetLensReviewReportOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LensReviewSummaryTypeDef = TypedDict(
     "LensReviewSummaryTypeDef",
     {
         "LensAlias": str,
@@ -1657,48 +1668,14 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "Profiles": List[WorkloadProfileTypeDef],
         "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Description": str,
-        "Environment": WorkloadEnvironmentType,
-        "UpdatedAt": datetime,
-        "AccountIds": List[str],
-        "AwsRegions": List[str],
-        "NonAwsRegions": List[str],
-        "ArchitecturalDesign": str,
-        "ReviewOwner": str,
-        "ReviewRestrictionDate": datetime,
-        "IsReviewOwnerUpdateAcknowledged": bool,
-        "IndustryType": str,
-        "Industry": str,
-        "Notes": str,
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "RiskCounts": Dict[RiskType, int],
-        "PillarPriorities": List[str],
-        "Lenses": List[str],
-        "Owner": str,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
-        "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
-        "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
@@ -1715,24 +1692,24 @@
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensesOutputTypeDef = TypedDict(
     "ListLensesOutputTypeDef",
     {
         "LensSummaries": List[LensSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationSummaryTypeDef = TypedDict(
     "NotificationSummaryTypeDef",
     {
         "Type": NotificationTypeType,
@@ -1742,52 +1719,52 @@
 )
 
 ListProfileNotificationsOutputTypeDef = TypedDict(
     "ListProfileNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileSharesOutputTypeDef = TypedDict(
     "ListProfileSharesOutputTypeDef",
     {
         "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesOutputTypeDef = TypedDict(
     "ListProfilesOutputTypeDef",
     {
         "ProfileSummaries": List[ProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadSharesOutputTypeDef = TypedDict(
     "ListWorkloadSharesOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PillarDifferenceTypeDef = TypedDict(
     "PillarDifferenceTypeDef",
     {
         "PillarId": str,
@@ -1825,25 +1802,62 @@
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
         "ShareInvitation": ShareInvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkloadShareOutputTypeDef = TypedDict(
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WorkloadDiscoveryConfigUnionTypeDef = Union[
+    WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
+]
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Description": str,
+        "Environment": WorkloadEnvironmentType,
+        "UpdatedAt": datetime,
+        "AccountIds": List[str],
+        "AwsRegions": List[str],
+        "NonAwsRegions": List[str],
+        "ArchitecturalDesign": str,
+        "ReviewOwner": str,
+        "ReviewRestrictionDate": datetime,
+        "IsReviewOwnerUpdateAcknowledged": bool,
+        "IndustryType": str,
+        "Industry": str,
+        "Notes": str,
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "RiskCounts": Dict[RiskType, int],
+        "PillarPriorities": List[str],
+        "Lenses": List[str],
+        "Owner": str,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+        "DiscoveryConfig": WorkloadDiscoveryConfigOutputTypeDef,
+        "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
+    total=False,
 )
 
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
         "Title": str,
@@ -1870,101 +1884,74 @@
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensReviewsOutputTypeDef = TypedDict(
     "ListLensReviewsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewSummaries": List[LensReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadsOutputTypeDef = TypedDict(
     "ListWorkloadsOutputTypeDef",
     {
         "WorkloadSummaries": List[WorkloadSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MilestoneSummaryTypeDef = TypedDict(
     "MilestoneSummaryTypeDef",
     {
         "MilestoneNumber": int,
         "MilestoneName": str,
         "RecordedAt": datetime,
         "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "Workload": WorkloadTypeDef,
-    },
-    total=False,
-)
-
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLensReviewOutputTypeDef = TypedDict(
     "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VersionDifferencesTypeDef = TypedDict(
     "VersionDifferencesTypeDef",
     {
         "PillarDifferences": List[PillarDifferenceTypeDef],
@@ -1996,14 +1983,41 @@
         "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "Workload": WorkloadTypeDef,
+    },
+    total=False,
+)
+
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
@@ -2050,97 +2064,97 @@
 
 ListMilestonesOutputTypeDef = TypedDict(
     "ListMilestonesOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneSummaries": List[MilestoneSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileOutputTypeDef = TypedDict(
     "GetProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfileOutputTypeDef = TypedDict(
     "UpdateProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileTemplateOutputTypeDef = TypedDict(
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "AnswerSummaries": List[AnswerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnswerOutputTypeDef = TypedDict(
     "GetAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnswerOutputTypeDef = TypedDict(
     "UpdateAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConsolidatedReportMetricTypeDef = TypedDict(
     "ConsolidatedReportMetricTypeDef",
     {
         "MetricType": Literal["WORKLOAD"],
@@ -2157,10 +2171,10 @@
 
 GetConsolidatedReportOutputTypeDef = TypedDict(
     "GetConsolidatedReportOutputTypeDef",
     {
         "Metrics": List[ConsolidatedReportMetricTypeDef],
         "NextToken": str,
         "Base64String": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected/type_defs.pyi` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_wellarchitected.type_defs import ChoiceContentTypeDef
 
-    data: ChoiceContentTypeDef = {...}
+    data: ChoiceContentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
@@ -63,51 +63,42 @@
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
-    "CreateLensShareOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
-    "CreateLensVersionOutputTypeDef",
     "CreateMilestoneInputRequestTypeDef",
-    "CreateMilestoneOutputTypeDef",
     "ProfileQuestionUpdateTypeDef",
-    "CreateProfileOutputTypeDef",
     "CreateProfileShareInputRequestTypeDef",
-    "CreateProfileShareOutputTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
-    "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
-    "CreateWorkloadShareOutputTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteProfileInputRequestTypeDef",
     "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
     "DisassociateProfilesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportLensInputRequestTypeDef",
-    "ExportLensOutputTypeDef",
     "GetAnswerInputRequestTypeDef",
     "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
     "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "ImportLensOutputTypeDef",
     "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
@@ -123,85 +114,96 @@
     "ListProfileSharesInputRequestTypeDef",
     "ProfileShareSummaryTypeDef",
     "ListProfilesInputRequestTypeDef",
     "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
     "QuestionDifferenceTypeDef",
     "ProfileChoiceTypeDef",
     "ProfileTemplateChoiceTypeDef",
-    "ResponseMetadataTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
+    "WorkloadDiscoveryConfigOutputTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
-    "ListCheckDetailsOutputTypeDef",
-    "ListCheckSummariesOutputTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
+    "CreateLensShareOutputTypeDef",
+    "CreateLensVersionOutputTypeDef",
+    "CreateMilestoneOutputTypeDef",
+    "CreateProfileOutputTypeDef",
+    "CreateProfileShareOutputTypeDef",
+    "CreateWorkloadOutputTypeDef",
+    "CreateWorkloadShareOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportLensOutputTypeDef",
+    "ImportLensOutputTypeDef",
+    "ListCheckDetailsOutputTypeDef",
+    "ListCheckSummariesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "CreateProfileInputRequestTypeDef",
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadDiscoveryConfigUnionTypeDef",
+    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "LensMetricTypeDef",
     "ListMilestonesOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
@@ -331,19 +333,22 @@
     {
         "LensAlias": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateLensShareOutputTypeDef = TypedDict(
-    "CreateLensShareOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLensVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
@@ -360,114 +365,60 @@
 )
 
 class CreateLensVersionInputRequestTypeDef(
     _RequiredCreateLensVersionInputRequestTypeDef, _OptionalCreateLensVersionInputRequestTypeDef
 ):
     pass
 
-CreateLensVersionOutputTypeDef = TypedDict(
-    "CreateLensVersionOutputTypeDef",
-    {
-        "LensArn": str,
-        "LensVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMilestoneInputRequestTypeDef = TypedDict(
     "CreateMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateMilestoneOutputTypeDef = TypedDict(
-    "CreateMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ProfileQuestionUpdateTypeDef = TypedDict(
     "ProfileQuestionUpdateTypeDef",
     {
         "QuestionId": str,
         "SelectedChoiceIds": Sequence[str],
     },
     total=False,
 )
 
-CreateProfileOutputTypeDef = TypedDict(
-    "CreateProfileOutputTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProfileShareInputRequestTypeDef = TypedDict(
     "CreateProfileShareInputRequestTypeDef",
     {
         "ProfileArn": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateProfileShareOutputTypeDef = TypedDict(
-    "CreateProfileShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
         "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
-CreateWorkloadOutputTypeDef = TypedDict(
-    "CreateWorkloadOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
     },
 )
 
-CreateWorkloadShareOutputTypeDef = TypedDict(
-    "CreateWorkloadShareOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLensInputRequestTypeDef = TypedDict(
     "DeleteLensInputRequestTypeDef",
     {
         "LensAlias": str,
         "ClientRequestToken": str,
         "LensStatus": LensStatusTypeType,
     },
@@ -528,21 +479,14 @@
     "DisassociateProfilesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ProfileArns": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
@@ -554,22 +498,14 @@
 )
 
 class ExportLensInputRequestTypeDef(
     _RequiredExportLensInputRequestTypeDef, _OptionalExportLensInputRequestTypeDef
 ):
     pass
 
-ExportLensOutputTypeDef = TypedDict(
-    "ExportLensOutputTypeDef",
-    {
-        "LensJSON": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetAnswerInputRequestTypeDef = TypedDict(
     "_RequiredGetAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "QuestionId": str,
     },
@@ -764,23 +700,14 @@
 )
 
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
-ImportLensOutputTypeDef = TypedDict(
-    "ImportLensOutputTypeDef",
-    {
-        "LensArn": str,
-        "Status": ImportLensStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadProfileTypeDef = TypedDict(
     "WorkloadProfileTypeDef",
     {
         "ProfileArn": str,
         "ProfileVersion": str,
     },
     total=False,
@@ -1137,22 +1064,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWorkloadSharesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkloadSharesInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListWorkloadSharesInputRequestTypeDef = TypedDict(
@@ -1219,25 +1138,14 @@
         "ChoiceId": str,
         "ChoiceTitle": str,
         "ChoiceDescription": str,
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
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
@@ -1363,14 +1271,23 @@
 
 class UpgradeProfileVersionInputRequestTypeDef(
     _RequiredUpgradeProfileVersionInputRequestTypeDef,
     _OptionalUpgradeProfileVersionInputRequestTypeDef,
 ):
     pass
 
+WorkloadDiscoveryConfigOutputTypeDef = TypedDict(
+    "WorkloadDiscoveryConfigOutputTypeDef",
+    {
+        "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
+        "WorkloadResourceDefinition": List[DefinitionTypeType],
+    },
+    total=False,
+)
+
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
@@ -1382,32 +1299,14 @@
         "QuestionId": str,
         "Risk": RiskType,
         "BestPractices": List[BestPracticeTypeDef],
     },
     total=False,
 )
 
-ListCheckDetailsOutputTypeDef = TypedDict(
-    "ListCheckDetailsOutputTypeDef",
-    {
-        "CheckDetails": List[CheckDetailTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCheckSummariesOutputTypeDef = TypedDict(
-    "ListCheckSummariesOutputTypeDef",
-    {
-        "CheckSummaries": List[CheckSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1438,14 +1337,126 @@
 )
 
 class UpdateAnswerInputRequestTypeDef(
     _RequiredUpdateAnswerInputRequestTypeDef, _OptionalUpdateAnswerInputRequestTypeDef
 ):
     pass
 
+CreateLensShareOutputTypeDef = TypedDict(
+    "CreateLensShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLensVersionOutputTypeDef = TypedDict(
+    "CreateLensVersionOutputTypeDef",
+    {
+        "LensArn": str,
+        "LensVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMilestoneOutputTypeDef = TypedDict(
+    "CreateMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileOutputTypeDef = TypedDict(
+    "CreateProfileOutputTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileShareOutputTypeDef = TypedDict(
+    "CreateProfileShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadOutputTypeDef = TypedDict(
+    "CreateWorkloadOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadShareOutputTypeDef = TypedDict(
+    "CreateWorkloadShareOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "ShareId": str,
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
+ExportLensOutputTypeDef = TypedDict(
+    "ExportLensOutputTypeDef",
+    {
+        "LensJSON": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportLensOutputTypeDef = TypedDict(
+    "ImportLensOutputTypeDef",
+    {
+        "LensArn": str,
+        "Status": ImportLensStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckDetailsOutputTypeDef = TypedDict(
+    "ListCheckDetailsOutputTypeDef",
+    {
+        "CheckDetails": List[CheckDetailTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckSummariesOutputTypeDef = TypedDict(
+    "ListCheckSummariesOutputTypeDef",
+    {
+        "CheckSummaries": List[CheckSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateProfileInputRequestTypeDef = TypedDict(
     "_RequiredCreateProfileInputRequestTypeDef",
     {
         "ProfileName": str,
         "ProfileDescription": str,
         "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
         "ClientRequestToken": str,
@@ -1553,25 +1564,25 @@
 ):
     pass
 
 GetLensOutputTypeDef = TypedDict(
     "GetLensOutputTypeDef",
     {
         "Lens": LensTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensReviewReportOutputTypeDef = TypedDict(
     "GetLensReviewReportOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LensReviewSummaryTypeDef = TypedDict(
     "LensReviewSummaryTypeDef",
     {
         "LensAlias": str,
@@ -1600,48 +1611,14 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "Profiles": List[WorkloadProfileTypeDef],
         "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Description": str,
-        "Environment": WorkloadEnvironmentType,
-        "UpdatedAt": datetime,
-        "AccountIds": List[str],
-        "AwsRegions": List[str],
-        "NonAwsRegions": List[str],
-        "ArchitecturalDesign": str,
-        "ReviewOwner": str,
-        "ReviewRestrictionDate": datetime,
-        "IsReviewOwnerUpdateAcknowledged": bool,
-        "IndustryType": str,
-        "Industry": str,
-        "Notes": str,
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "RiskCounts": Dict[RiskType, int],
-        "PillarPriorities": List[str],
-        "Lenses": List[str],
-        "Owner": str,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
-        "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
-        "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
@@ -1658,24 +1635,24 @@
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensesOutputTypeDef = TypedDict(
     "ListLensesOutputTypeDef",
     {
         "LensSummaries": List[LensSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationSummaryTypeDef = TypedDict(
     "NotificationSummaryTypeDef",
     {
         "Type": NotificationTypeType,
@@ -1685,52 +1662,52 @@
 )
 
 ListProfileNotificationsOutputTypeDef = TypedDict(
     "ListProfileNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileSharesOutputTypeDef = TypedDict(
     "ListProfileSharesOutputTypeDef",
     {
         "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesOutputTypeDef = TypedDict(
     "ListProfilesOutputTypeDef",
     {
         "ProfileSummaries": List[ProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadSharesOutputTypeDef = TypedDict(
     "ListWorkloadSharesOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PillarDifferenceTypeDef = TypedDict(
     "PillarDifferenceTypeDef",
     {
         "PillarId": str,
@@ -1768,25 +1745,62 @@
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
         "ShareInvitation": ShareInvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkloadShareOutputTypeDef = TypedDict(
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WorkloadDiscoveryConfigUnionTypeDef = Union[
+    WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
+]
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Description": str,
+        "Environment": WorkloadEnvironmentType,
+        "UpdatedAt": datetime,
+        "AccountIds": List[str],
+        "AwsRegions": List[str],
+        "NonAwsRegions": List[str],
+        "ArchitecturalDesign": str,
+        "ReviewOwner": str,
+        "ReviewRestrictionDate": datetime,
+        "IsReviewOwnerUpdateAcknowledged": bool,
+        "IndustryType": str,
+        "Industry": str,
+        "Notes": str,
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "RiskCounts": Dict[RiskType, int],
+        "PillarPriorities": List[str],
+        "Lenses": List[str],
+        "Owner": str,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+        "DiscoveryConfig": WorkloadDiscoveryConfigOutputTypeDef,
+        "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
+    total=False,
 )
 
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
         "Title": str,
@@ -1813,101 +1827,74 @@
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensReviewsOutputTypeDef = TypedDict(
     "ListLensReviewsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewSummaries": List[LensReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadsOutputTypeDef = TypedDict(
     "ListWorkloadsOutputTypeDef",
     {
         "WorkloadSummaries": List[WorkloadSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MilestoneSummaryTypeDef = TypedDict(
     "MilestoneSummaryTypeDef",
     {
         "MilestoneNumber": int,
         "MilestoneName": str,
         "RecordedAt": datetime,
         "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "Workload": WorkloadTypeDef,
-    },
-    total=False,
-)
-
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLensReviewOutputTypeDef = TypedDict(
     "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VersionDifferencesTypeDef = TypedDict(
     "VersionDifferencesTypeDef",
     {
         "PillarDifferences": List[PillarDifferenceTypeDef],
@@ -1939,14 +1926,41 @@
         "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "Workload": WorkloadTypeDef,
+    },
+    total=False,
+)
+
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
@@ -1993,97 +2007,97 @@
 
 ListMilestonesOutputTypeDef = TypedDict(
     "ListMilestonesOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneSummaries": List[MilestoneSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileOutputTypeDef = TypedDict(
     "GetProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfileOutputTypeDef = TypedDict(
     "UpdateProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileTemplateOutputTypeDef = TypedDict(
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "AnswerSummaries": List[AnswerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnswerOutputTypeDef = TypedDict(
     "GetAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnswerOutputTypeDef = TypedDict(
     "UpdateAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConsolidatedReportMetricTypeDef = TypedDict(
     "ConsolidatedReportMetricTypeDef",
     {
         "MetricType": Literal["WORKLOAD"],
@@ -2100,10 +2114,10 @@
 
 GetConsolidatedReportOutputTypeDef = TypedDict(
     "GetConsolidatedReportOutputTypeDef",
     {
         "Metrics": List[ConsolidatedReportMetricTypeDef],
         "NextToken": str,
         "Base64String": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/PKG-INFO` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wellarchitected
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.WellArchitected 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.WellArchitected 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore wellarchitected type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-wellarchitected"></a>
 
 # types-aiobotocore-wellarchitected
 
 [![PyPI - types-aiobotocore-wellarchitected](https://img.shields.io/pypi/v/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wellarchitected.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-wellarchitected?color=blue)](https://pypistats.org/packages/types-aiobotocore-wellarchitected)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wellarchitected)](https://pepy.tech/project/types-aiobotocore-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.WellArchitected 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [types-aiobotocore-wellarchitected docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/).
 
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
@@ -310,71 +309,62 @@
 )
 
 
 def check_value(value: AdditionalResourceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_wellarchitected.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
     AssociateProfilesInputRequestTypeDef,
     BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
-    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    CreateMilestoneOutputTypeDef,
     ProfileQuestionUpdateTypeDef,
-    CreateProfileOutputTypeDef,
     CreateProfileShareInputRequestTypeDef,
-    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
-    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
-    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteProfileInputRequestTypeDef,
     DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     DisassociateProfilesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
-    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
     GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
     GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    ImportLensOutputTypeDef,
     WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
@@ -390,94 +380,105 @@
     ListProfileSharesInputRequestTypeDef,
     ProfileShareSummaryTypeDef,
     ListProfilesInputRequestTypeDef,
     ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
     QuestionDifferenceTypeDef,
     ProfileChoiceTypeDef,
     ProfileTemplateChoiceTypeDef,
-    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     UpgradeProfileVersionInputRequestTypeDef,
+    WorkloadDiscoveryConfigOutputTypeDef,
     AdditionalResourcesTypeDef,
     QuestionMetricTypeDef,
-    ListCheckDetailsOutputTypeDef,
-    ListCheckSummariesOutputTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
+    CreateLensShareOutputTypeDef,
+    CreateLensVersionOutputTypeDef,
+    CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
+    CreateWorkloadOutputTypeDef,
+    CreateWorkloadShareOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportLensOutputTypeDef,
+    ImportLensOutputTypeDef,
+    ListCheckDetailsOutputTypeDef,
+    ListCheckSummariesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateProfileInputRequestTypeDef,
     UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     LensReviewSummaryTypeDef,
     WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
     ListProfileNotificationsOutputTypeDef,
     ListProfileSharesOutputTypeDef,
     ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadDiscoveryConfigUnionTypeDef,
+    WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
-    GetWorkloadOutputTypeDef,
-    MilestoneTypeDef,
-    UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     VersionDifferencesTypeDef,
     ProfileTypeDef,
     ProfileTemplateTypeDef,
+    GetWorkloadOutputTypeDef,
+    MilestoneTypeDef,
+    UpdateWorkloadOutputTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
     LensMetricTypeDef,
     ListMilestonesOutputTypeDef,
-    GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetProfileOutputTypeDef,
     UpdateProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
+    GetMilestoneOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
 
 
-def get_structure() -> ChoiceContentTypeDef:
+def get_value() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt` & `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*


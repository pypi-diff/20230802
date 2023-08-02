# Comparing `tmp/types-aiobotocore-backup-2.5.2.tar.gz` & `tmp/types-aiobotocore-backup-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-backup-2.5.2.tar` & `types-aiobotocore-backup-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.953739 types-aiobotocore-backup-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-07-08 01:43:16.953739 types-aiobotocore-backup-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20917 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.953739 types-aiobotocore-backup-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.953739 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57895 2023-07-08 01:26:15.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57801 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-08 01:26:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-07-08 01:26:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-07-08 01:26:15.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-07-08 01:26:15.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    67874 2023-07-08 01:26:17.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67799 2023-07-08 01:26:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:14.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.953739 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-07-08 01:43:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:43:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:16.000000 types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21415 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57881 2023-08-02 14:33:42.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57787 2023-08-02 14:33:42.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-08-02 14:33:42.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72090 2023-08-02 14:33:44.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72007 2023-08-02 14:33:43.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:41.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.309648 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:55.000000 types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-2.5.2/LICENSE` & `types-aiobotocore-backup-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2/PKG-INFO` & `types-aiobotocore-backup-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore backup type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore backup type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backup"></a>
 
 # types-aiobotocore-backup
 
 [![PyPI - types-aiobotocore-backup](https://img.shields.io/pypi/v/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backup?color=blue)](https://pypistats.org/packages/types-aiobotocore-backup)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Backup 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [types-aiobotocore-backup docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/).
 
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
@@ -370,201 +369,216 @@
 )
 
 
 def check_value(value: BackupJobStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backup.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backup.type_defs import (
+    AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
     ConditionParameterTypeDef,
     ControlInputParameterTypeDef,
+    ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
-    CreateBackupSelectionOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
-    CreateReportPlanOutputTypeDef,
-    DateRangeTypeDef,
+    DateRangeOutputTypeDef,
+    TimestampTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
-    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
-    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
-    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
-    ListBackupJobsInputRequestTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
-    ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
-    ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
-    ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
-    ListTagsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
-    ResponseMetadataTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
+    ReportSettingOutputTypeDef,
     StartReportJobInputRequestTypeDef,
-    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
-    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
-    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    ListBackupSelectionsOutputTypeDef,
-    ListBackupVaultsOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
-    UpdateRecoveryPointLifecycleOutputTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    CreateBackupSelectionOutputTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
+    CreateReportPlanOutputTypeDef,
+    DeleteBackupPlanOutputTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    DescribeBackupVaultOutputTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
+    DescribeRestoreJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
+    ListBackupSelectionsOutputTypeDef,
+    ListBackupVaultsOutputTypeDef,
+    ListTagsOutputTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
+    StartReportJobOutputTypeDef,
+    StartRestoreJobOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
+    UpdateFrameworkOutputTypeDef,
+    UpdateRecoveryPointLifecycleOutputTypeDef,
+    UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
-    ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
-    RecoveryPointSelectionTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
+    DateRangeTypeDef,
+    ListBackupJobsInputRequestTypeDef,
+    ListCopyJobsInputRequestTypeDef,
+    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListReportJobsInputRequestTypeDef,
+    ListRestoreJobsInputRequestTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
     ReportJobTypeDef,
+    ReportPlanTypeDef,
+    ReportSettingUnionTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
-    CreateFrameworkInputRequestTypeDef,
     DescribeFrameworkOutputTypeDef,
-    UpdateFrameworkInputRequestTypeDef,
-    DescribeReportPlanOutputTypeDef,
-    ListReportPlansOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
+    FrameworkControlUnionTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
+    RecoveryPointSelectionTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
+    DescribeReportPlanOutputTypeDef,
+    ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
-    CreateBackupSelectionInputRequestTypeDef,
     GetBackupSelectionOutputTypeDef,
+    BackupSelectionUnionTypeDef,
+    CreateBackupSelectionInputRequestTypeDef,
+    CreateFrameworkInputRequestTypeDef,
+    UpdateFrameworkInputRequestTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingTypeDef:
+def get_value() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backup-2.5.2/README.md` & `types-aiobotocore-backup-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-backup"></a>
 
 # types-aiobotocore-backup
 
 [![PyPI - types-aiobotocore-backup](https://img.shields.io/pypi/v/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backup?color=blue)](https://pypistats.org/packages/types-aiobotocore-backup)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Backup 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [types-aiobotocore-backup docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/).
 
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
@@ -337,201 +337,216 @@
 )
 
 
 def check_value(value: BackupJobStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backup.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backup.type_defs import (
+    AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
     ConditionParameterTypeDef,
     ControlInputParameterTypeDef,
+    ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
-    CreateBackupSelectionOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
-    CreateReportPlanOutputTypeDef,
-    DateRangeTypeDef,
+    DateRangeOutputTypeDef,
+    TimestampTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
-    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
-    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
-    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
-    ListBackupJobsInputRequestTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
-    ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
-    ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
-    ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
-    ListTagsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
-    ResponseMetadataTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
+    ReportSettingOutputTypeDef,
     StartReportJobInputRequestTypeDef,
-    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
-    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
-    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    ListBackupSelectionsOutputTypeDef,
-    ListBackupVaultsOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
-    UpdateRecoveryPointLifecycleOutputTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    CreateBackupSelectionOutputTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
+    CreateReportPlanOutputTypeDef,
+    DeleteBackupPlanOutputTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    DescribeBackupVaultOutputTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
+    DescribeRestoreJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
+    ListBackupSelectionsOutputTypeDef,
+    ListBackupVaultsOutputTypeDef,
+    ListTagsOutputTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
+    StartReportJobOutputTypeDef,
+    StartRestoreJobOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
+    UpdateFrameworkOutputTypeDef,
+    UpdateRecoveryPointLifecycleOutputTypeDef,
+    UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
-    ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
-    RecoveryPointSelectionTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
+    DateRangeTypeDef,
+    ListBackupJobsInputRequestTypeDef,
+    ListCopyJobsInputRequestTypeDef,
+    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListReportJobsInputRequestTypeDef,
+    ListRestoreJobsInputRequestTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
     ReportJobTypeDef,
+    ReportPlanTypeDef,
+    ReportSettingUnionTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
-    CreateFrameworkInputRequestTypeDef,
     DescribeFrameworkOutputTypeDef,
-    UpdateFrameworkInputRequestTypeDef,
-    DescribeReportPlanOutputTypeDef,
-    ListReportPlansOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
+    FrameworkControlUnionTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
+    RecoveryPointSelectionTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
+    DescribeReportPlanOutputTypeDef,
+    ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
-    CreateBackupSelectionInputRequestTypeDef,
     GetBackupSelectionOutputTypeDef,
+    BackupSelectionUnionTypeDef,
+    CreateBackupSelectionInputRequestTypeDef,
+    CreateFrameworkInputRequestTypeDef,
+    UpdateFrameworkInputRequestTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingTypeDef:
+def get_value() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backup-2.5.2/setup.py` & `types-aiobotocore-backup-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore backup type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore backup type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_backup": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/"
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/__init__.py` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/__init__.pyi` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/__main__.py` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Backup 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Backup 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/client.py` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("backup") as client:
         client: BackupClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BackupJobStateType,
     BackupVaultEventType,
@@ -40,15 +39,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
-    BackupSelectionTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
     DeleteBackupPlanOutputTypeDef,
@@ -61,15 +60,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
-    FrameworkControlTypeDef,
+    FrameworkControlUnionTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldOutputTypeDef,
@@ -89,21 +88,22 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
-    ReportDeliveryChannelTypeDef,
-    ReportSettingTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
+    ReportSettingUnionTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
+    TimestampTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -194,15 +194,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_plan)
         """
 
     async def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: BackupSelectionTypeDef,
+        BackupSelection: BackupSelectionUnionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
@@ -224,15 +224,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_vault)
         """
 
     async def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[FrameworkControlTypeDef],
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
@@ -242,30 +242,30 @@
 
     async def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
+        RecoveryPointSelection: RecoveryPointSelectionUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_legal_hold)
         """
 
     async def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
-        ReportSetting: ReportSettingTypeDef,
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef,
+        ReportSetting: ReportSettingUnionTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
@@ -594,20 +594,20 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListBackupJobsOutputTypeDef:
         """
         Returns a list of existing backup jobs for an authenticated account for the last
         30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_jobs)
@@ -672,21 +672,21 @@
     async def list_copy_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListCopyJobsOutputTypeDef:
         """
         Returns metadata about your copy jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_copy_jobs)
@@ -730,16 +730,16 @@
         *,
         BackupVaultName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...
     ) -> ListRecoveryPointsByBackupVaultOutputTypeDef:
         """
         Returns detailed information about the recovery points stored in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_recovery_points_by_backup_vault)
@@ -767,16 +767,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_recovery_points_by_resource)
         """
 
     async def list_report_jobs(
         self,
         *,
         ByReportPlanName: str = ...,
-        ByCreationBefore: Union[datetime, str] = ...,
-        ByCreationAfter: Union[datetime, str] = ...,
+        ByCreationBefore: TimestampTypeDef = ...,
+        ByCreationAfter: TimestampTypeDef = ...,
         ByStatus: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListReportJobsOutputTypeDef:
         """
         Returns details about your report jobs.
 
@@ -796,19 +796,19 @@
 
     async def list_restore_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...
     ) -> ListRestoreJobsOutputTypeDef:
         """
         Returns a list of jobs that Backup initiated to restore a saved resource,
         including details about the recovery process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_restore_jobs)
@@ -973,15 +973,15 @@
         """
 
     async def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -1023,16 +1023,16 @@
         """
 
     async def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
-        ReportSetting: ReportSettingTypeDef = ...,
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef = ...,
+        ReportSetting: ReportSettingUnionTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/client.pyi` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("backup") as client:
         client: BackupClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BackupJobStateType,
     BackupVaultEventType,
@@ -40,15 +39,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
-    BackupSelectionTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
     DeleteBackupPlanOutputTypeDef,
@@ -61,15 +60,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
-    FrameworkControlTypeDef,
+    FrameworkControlUnionTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldOutputTypeDef,
@@ -89,21 +88,22 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
-    ReportDeliveryChannelTypeDef,
-    ReportSettingTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
+    ReportSettingUnionTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
+    TimestampTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -185,15 +185,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_plan)
         """
     async def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: BackupSelectionTypeDef,
+        BackupSelection: BackupSelectionUnionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
@@ -213,15 +213,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_backup_vault)
         """
     async def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[FrameworkControlTypeDef],
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
@@ -230,29 +230,29 @@
         """
     async def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: RecoveryPointSelectionTypeDef = ...,
+        RecoveryPointSelection: RecoveryPointSelectionUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#create_legal_hold)
         """
     async def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef,
-        ReportSetting: ReportSettingTypeDef,
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef,
+        ReportSetting: ReportSettingUnionTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
@@ -547,20 +547,20 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListBackupJobsOutputTypeDef:
         """
         Returns a list of existing backup jobs for an authenticated account for the last
         30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_jobs)
@@ -619,21 +619,21 @@
     async def list_copy_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListCopyJobsOutputTypeDef:
         """
         Returns metadata about your copy jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_copy_jobs)
@@ -673,16 +673,16 @@
         *,
         BackupVaultName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...
     ) -> ListRecoveryPointsByBackupVaultOutputTypeDef:
         """
         Returns detailed information about the recovery points stored in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_backup_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_recovery_points_by_backup_vault)
@@ -707,16 +707,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_recovery_points_by_resource)
         """
     async def list_report_jobs(
         self,
         *,
         ByReportPlanName: str = ...,
-        ByCreationBefore: Union[datetime, str] = ...,
-        ByCreationAfter: Union[datetime, str] = ...,
+        ByCreationBefore: TimestampTypeDef = ...,
+        ByCreationAfter: TimestampTypeDef = ...,
         ByStatus: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListReportJobsOutputTypeDef:
         """
         Returns details about your report jobs.
 
@@ -734,19 +734,19 @@
         """
     async def list_restore_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...
     ) -> ListRestoreJobsOutputTypeDef:
         """
         Returns a list of jobs that Backup initiated to restore a saved resource,
         including details about the recovery process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#list_restore_jobs)
@@ -898,15 +898,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_backup_plan)
         """
     async def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[FrameworkControlTypeDef] = ...,
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
@@ -944,16 +944,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/client/#update_region_settings)
         """
     async def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: ReportDeliveryChannelTypeDef = ...,
-        ReportSetting: ReportSettingTypeDef = ...,
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef = ...,
+        ReportSetting: ReportSettingUnionTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/literals.py` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/literals.pyi` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/paginator.py` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         list_protected_resources_paginator: ListProtectedResourcesPaginator = client.get_paginator("list_protected_resources")
         list_recovery_points_by_backup_vault_paginator: ListRecoveryPointsByBackupVaultPaginator = client.get_paginator("list_recovery_points_by_backup_vault")
         list_recovery_points_by_legal_hold_paginator: ListRecoveryPointsByLegalHoldPaginator = client.get_paginator("list_recovery_points_by_legal_hold")
         list_recovery_points_by_resource_paginator: ListRecoveryPointsByResourcePaginator = client.get_paginator("list_recovery_points_by_resource")
         list_restore_jobs_paginator: ListRestoreJobsPaginator = client.get_paginator("list_restore_jobs")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import BackupJobStateType, CopyJobStateType, RestoreJobStatusType
 from .type_defs import (
     ListBackupJobsOutputTypeDef,
@@ -62,14 +61,15 @@
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupJobsPaginator",
     "ListBackupPlanTemplatesPaginator",
     "ListBackupPlanVersionsPaginator",
     "ListBackupPlansPaginator",
@@ -103,97 +103,97 @@
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupjobspaginator)
         """
 
 
 class ListBackupPlanTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplantemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupPlanTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplantemplatespaginator)
         """
 
 
 class ListBackupPlanVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanversionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupPlanVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanversionspaginator)
         """
 
 
 class ListBackupPlansPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanspaginator)
     """
 
     def paginate(
-        self, *, IncludeDeleted: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IncludeDeleted: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanspaginator)
         """
 
 
 class ListBackupSelectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupselectionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupSelectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupselectionspaginator)
         """
 
 
 class ListBackupVaultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupvaultspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupvaultspaginator)
         """
 
 
@@ -204,53 +204,53 @@
     """
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listcopyjobspaginator)
         """
 
 
 class ListLegalHoldsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listlegalholdspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLegalHoldsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listlegalholdspaginator)
         """
 
 
 class ListProtectedResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listprotectedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listprotectedresourcespaginator)
         """
 
 
@@ -263,48 +263,48 @@
     def paginate(
         self,
         *,
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 
 class ListRecoveryPointsByLegalHoldPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbylegalholdpaginator)
     """
 
     def paginate(
-        self, *, LegalHoldId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LegalHoldId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbylegalholdpaginator)
         """
 
 
 class ListRecoveryPointsByResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbyresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsByResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbyresourcepaginator)
         """
 
 
@@ -314,18 +314,18 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobspaginator)
     """
 
     def paginate(
         self,
         *,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/paginator.pyi` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         list_protected_resources_paginator: ListProtectedResourcesPaginator = client.get_paginator("list_protected_resources")
         list_recovery_points_by_backup_vault_paginator: ListRecoveryPointsByBackupVaultPaginator = client.get_paginator("list_recovery_points_by_backup_vault")
         list_recovery_points_by_legal_hold_paginator: ListRecoveryPointsByLegalHoldPaginator = client.get_paginator("list_recovery_points_by_legal_hold")
         list_recovery_points_by_resource_paginator: ListRecoveryPointsByResourcePaginator = client.get_paginator("list_recovery_points_by_resource")
         list_restore_jobs_paginator: ListRestoreJobsPaginator = client.get_paginator("list_restore_jobs")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import BackupJobStateType, CopyJobStateType, RestoreJobStatusType
 from .type_defs import (
     ListBackupJobsOutputTypeDef,
@@ -62,14 +61,15 @@
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupJobsPaginator",
     "ListBackupPlanTemplatesPaginator",
     "ListBackupPlanVersionsPaginator",
     "ListBackupPlansPaginator",
@@ -100,92 +100,92 @@
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupjobspaginator)
         """
 
 class ListBackupPlanTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplantemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupPlanTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplantemplatespaginator)
         """
 
 class ListBackupPlanVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanversionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupPlanVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanversionspaginator)
         """
 
 class ListBackupPlansPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanspaginator)
     """
 
     def paginate(
-        self, *, IncludeDeleted: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IncludeDeleted: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupplanspaginator)
         """
 
 class ListBackupSelectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupselectionspaginator)
     """
 
     def paginate(
-        self, *, BackupPlanId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BackupPlanId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupSelectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupselectionspaginator)
         """
 
 class ListBackupVaultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupvaultspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBackupVaultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listbackupvaultspaginator)
         """
 
 class ListCopyJobsPaginator(AioPaginator):
@@ -195,51 +195,51 @@
     """
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listcopyjobspaginator)
         """
 
 class ListLegalHoldsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listlegalholdspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLegalHoldsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listlegalholdspaginator)
         """
 
 class ListProtectedResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listprotectedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectedResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listprotectedresourcespaginator)
         """
 
 class ListRecoveryPointsByBackupVaultPaginator(AioPaginator):
@@ -251,46 +251,46 @@
     def paginate(
         self,
         *,
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
 
 class ListRecoveryPointsByLegalHoldPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbylegalholdpaginator)
     """
 
     def paginate(
-        self, *, LegalHoldId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, LegalHoldId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbylegalholdpaginator)
         """
 
 class ListRecoveryPointsByResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbyresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecoveryPointsByResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrecoverypointsbyresourcepaginator)
         """
 
 class ListRestoreJobsPaginator(AioPaginator):
@@ -299,18 +299,18 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobspaginator)
     """
 
     def paginate(
         self,
         *,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/type_defs.py` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for backup service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingTypeDef
+    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingOutputTypeDef
 
-    data: AdvancedBackupSettingTypeDef = {...}
+    data: AdvancedBackupSettingOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -32,190 +32,214 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
     "ConditionParameterTypeDef",
     "ControlInputParameterTypeDef",
+    "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
-    "CreateBackupSelectionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
-    "CreateBackupVaultOutputTypeDef",
-    "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
-    "CreateReportPlanOutputTypeDef",
-    "DateRangeTypeDef",
+    "DateRangeOutputTypeDef",
+    "TimestampTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
-    "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
     "DeleteRecoveryPointInputRequestTypeDef",
     "DeleteReportPlanInputRequestTypeDef",
     "DescribeBackupJobInputRequestTypeDef",
     "DescribeBackupVaultInputRequestTypeDef",
-    "DescribeBackupVaultOutputTypeDef",
     "DescribeCopyJobInputRequestTypeDef",
     "DescribeFrameworkInputRequestTypeDef",
-    "DescribeGlobalSettingsOutputTypeDef",
     "DescribeProtectedResourceInputRequestTypeDef",
-    "DescribeProtectedResourceOutputTypeDef",
     "DescribeRecoveryPointInputRequestTypeDef",
-    "DescribeRegionSettingsOutputTypeDef",
     "DescribeReportJobInputRequestTypeDef",
     "DescribeReportPlanInputRequestTypeDef",
     "DescribeRestoreJobInputRequestTypeDef",
-    "DescribeRestoreJobOutputTypeDef",
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     "DisassociateRecoveryPointInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportBackupPlanTemplateInputRequestTypeDef",
-    "ExportBackupPlanTemplateOutputTypeDef",
     "FrameworkTypeDef",
     "GetBackupPlanFromJSONInputRequestTypeDef",
     "GetBackupPlanFromTemplateInputRequestTypeDef",
     "GetBackupPlanInputRequestTypeDef",
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
-    "GetBackupVaultAccessPolicyOutputTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
-    "GetBackupVaultNotificationsOutputTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    "GetSupportedResourceTypesOutputTypeDef",
     "LegalHoldTypeDef",
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    "ListBackupJobsInputRequestTypeDef",
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
-    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupPlansInputRequestTypeDef",
-    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
-    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
-    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
-    "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
-    "ListTagsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
+    "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartBackupJobOutputTypeDef",
-    "StartCopyJobOutputTypeDef",
+    "ReportSettingOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
-    "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
-    "StartRestoreJobOutputTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateFrameworkOutputTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
-    "UpdateReportPlanOutputTypeDef",
     "BackupPlansListMemberTypeDef",
-    "CreateBackupPlanOutputTypeDef",
-    "UpdateBackupPlanOutputTypeDef",
     "BackupJobTypeDef",
     "CopyJobTypeDef",
-    "DescribeBackupJobOutputTypeDef",
-    "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
-    "ListBackupSelectionsOutputTypeDef",
-    "ListBackupVaultsOutputTypeDef",
-    "DescribeRecoveryPointOutputTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
+    "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
+    "CreateBackupPlanOutputTypeDef",
+    "CreateBackupSelectionOutputTypeDef",
+    "CreateBackupVaultOutputTypeDef",
+    "CreateFrameworkOutputTypeDef",
+    "CreateReportPlanOutputTypeDef",
+    "DeleteBackupPlanOutputTypeDef",
+    "DescribeBackupJobOutputTypeDef",
+    "DescribeBackupVaultOutputTypeDef",
+    "DescribeGlobalSettingsOutputTypeDef",
+    "DescribeProtectedResourceOutputTypeDef",
+    "DescribeRecoveryPointOutputTypeDef",
+    "DescribeRegionSettingsOutputTypeDef",
+    "DescribeRestoreJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportBackupPlanTemplateOutputTypeDef",
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    "GetBackupVaultNotificationsOutputTypeDef",
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    "GetSupportedResourceTypesOutputTypeDef",
+    "ListBackupPlanTemplatesOutputTypeDef",
+    "ListBackupSelectionsOutputTypeDef",
+    "ListBackupVaultsOutputTypeDef",
+    "ListTagsOutputTypeDef",
+    "StartBackupJobOutputTypeDef",
+    "StartCopyJobOutputTypeDef",
+    "StartReportJobOutputTypeDef",
+    "StartRestoreJobOutputTypeDef",
+    "UpdateBackupPlanOutputTypeDef",
+    "UpdateFrameworkOutputTypeDef",
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
-    "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
-    "RecoveryPointSelectionTypeDef",
+    "RecoveryPointSelectionOutputTypeDef",
+    "DateRangeTypeDef",
+    "ListBackupJobsInputRequestTypeDef",
+    "ListCopyJobsInputRequestTypeDef",
+    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    "ListReportJobsInputRequestTypeDef",
+    "ListRestoreJobsInputRequestTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
+    "ReportDeliveryChannelUnionTypeDef",
     "ReportJobTypeDef",
+    "ReportPlanTypeDef",
+    "ReportSettingUnionTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
+    "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
     "DescribeFrameworkOutputTypeDef",
-    "UpdateFrameworkInputRequestTypeDef",
-    "DescribeReportPlanOutputTypeDef",
-    "ListReportPlansOutputTypeDef",
-    "CreateLegalHoldInputRequestTypeDef",
+    "FrameworkControlUnionTypeDef",
     "CreateLegalHoldOutputTypeDef",
     "GetLegalHoldOutputTypeDef",
+    "RecoveryPointSelectionTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
+    "DescribeReportPlanOutputTypeDef",
+    "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
-    "CreateBackupSelectionInputRequestTypeDef",
     "GetBackupSelectionOutputTypeDef",
+    "BackupSelectionUnionTypeDef",
+    "CreateBackupSelectionInputRequestTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
+    "UpdateFrameworkInputRequestTypeDef",
+    "CreateLegalHoldInputRequestTypeDef",
+    "RecoveryPointSelectionUnionTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
+AdvancedBackupSettingOutputTypeDef = TypedDict(
+    "AdvancedBackupSettingOutputTypeDef",
+    {
+        "ResourceType": str,
+        "BackupOptions": Dict[str, str],
+    },
+    total=False,
+)
+
 AdvancedBackupSettingTypeDef = TypedDict(
     "AdvancedBackupSettingTypeDef",
     {
         "ResourceType": str,
         "BackupOptions": Mapping[str, str],
     },
     total=False,
@@ -334,31 +358,42 @@
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
 )
 
+ControlScopeOutputTypeDef = TypedDict(
+    "ControlScopeOutputTypeDef",
+    {
+        "ComplianceResourceIds": List[str],
+        "ComplianceResourceTypes": List[str],
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ControlScopeTypeDef = TypedDict(
     "ControlScopeTypeDef",
     {
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateBackupSelectionOutputTypeDef = TypedDict(
-    "CreateBackupSelectionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
@@ -377,33 +412,14 @@
 
 class CreateBackupVaultInputRequestTypeDef(
     _RequiredCreateBackupVaultInputRequestTypeDef, _OptionalCreateBackupVaultInputRequestTypeDef
 ):
     pass
 
 
-CreateBackupVaultOutputTypeDef = TypedDict(
-    "CreateBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFrameworkOutputTypeDef = TypedDict(
-    "CreateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReportDeliveryChannelTypeDef = TypedDict(
     "_RequiredReportDeliveryChannelTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalReportDeliveryChannelTypeDef = TypedDict(
@@ -441,50 +457,30 @@
 )
 
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
 
-CreateReportPlanOutputTypeDef = TypedDict(
-    "CreateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DateRangeTypeDef = TypedDict(
-    "DateRangeTypeDef",
+DateRangeOutputTypeDef = TypedDict(
+    "DateRangeOutputTypeDef",
     {
-        "FromDate": Union[datetime, str],
-        "ToDate": Union[datetime, str],
+        "FromDate": datetime,
+        "ToDate": datetime,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-DeleteBackupPlanOutputTypeDef = TypedDict(
-    "DeleteBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "DeletionDate": datetime,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBackupSelectionInputRequestTypeDef = TypedDict(
     "DeleteBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "SelectionId": str,
     },
 )
@@ -549,89 +545,43 @@
 DescribeBackupVaultInputRequestTypeDef = TypedDict(
     "DescribeBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-DescribeBackupVaultOutputTypeDef = TypedDict(
-    "DescribeBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "EncryptionKeyArn": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "NumberOfRecoveryPoints": int,
-        "Locked": bool,
-        "MinRetentionDays": int,
-        "MaxRetentionDays": int,
-        "LockDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCopyJobInputRequestTypeDef = TypedDict(
     "DescribeCopyJobInputRequestTypeDef",
     {
         "CopyJobId": str,
     },
 )
 
 DescribeFrameworkInputRequestTypeDef = TypedDict(
     "DescribeFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 
-DescribeGlobalSettingsOutputTypeDef = TypedDict(
-    "DescribeGlobalSettingsOutputTypeDef",
-    {
-        "GlobalSettings": Dict[str, str],
-        "LastUpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProtectedResourceInputRequestTypeDef = TypedDict(
     "DescribeProtectedResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeProtectedResourceOutputTypeDef = TypedDict(
-    "DescribeProtectedResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceType": str,
-        "LastBackupTime": datetime,
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRecoveryPointInputRequestTypeDef = TypedDict(
     "DescribeRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-DescribeRegionSettingsOutputTypeDef = TypedDict(
-    "DescribeRegionSettingsOutputTypeDef",
-    {
-        "ResourceTypeOptInPreference": Dict[str, bool],
-        "ResourceTypeManagementPreference": Dict[str, bool],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeReportJobInputRequestTypeDef = TypedDict(
     "DescribeReportJobInputRequestTypeDef",
     {
         "ReportJobId": str,
     },
 )
 
@@ -645,34 +595,14 @@
 DescribeRestoreJobInputRequestTypeDef = TypedDict(
     "DescribeRestoreJobInputRequestTypeDef",
     {
         "RestoreJobId": str,
     },
 )
 
-DescribeRestoreJobOutputTypeDef = TypedDict(
-    "DescribeRestoreJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "RestoreJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "Status": RestoreJobStatusType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "ExpectedCompletionTimeMinutes": int,
-        "CreatedResourceArn": str,
-        "ResourceType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateRecoveryPointFromParentInputRequestTypeDef = TypedDict(
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
@@ -681,36 +611,21 @@
     "DisassociateRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportBackupPlanTemplateInputRequestTypeDef = TypedDict(
     "ExportBackupPlanTemplateInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-ExportBackupPlanTemplateOutputTypeDef = TypedDict(
-    "ExportBackupPlanTemplateOutputTypeDef",
-    {
-        "BackupPlanTemplateJson": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FrameworkTypeDef = TypedDict(
     "FrameworkTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "NumberOfControls": int,
@@ -766,42 +681,21 @@
 GetBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBackupVaultNotificationsInputRequestTypeDef = TypedDict(
     "GetBackupVaultNotificationsInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultNotificationsOutputTypeDef = TypedDict(
-    "GetBackupVaultNotificationsOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "SNSTopicArn": str,
-        "BackupVaultEvents": List[BackupVaultEventType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLegalHoldInputRequestTypeDef = TypedDict(
     "GetLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 
@@ -809,122 +703,47 @@
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    {
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "RestoreMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSupportedResourceTypesOutputTypeDef = TypedDict(
-    "GetSupportedResourceTypesOutputTypeDef",
-    {
-        "ResourceTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LegalHoldTypeDef = TypedDict(
     "LegalHoldTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
     },
     total=False,
 )
 
-ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListBackupJobsInputRequestTypeDef = TypedDict(
-    "ListBackupJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
-ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
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
 
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
-    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBackupPlanVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupPlanVersionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupPlanVersionsInputRequestTypeDef = TypedDict(
@@ -940,55 +759,24 @@
 class ListBackupPlanVersionsInputRequestTypeDef(
     _RequiredListBackupPlanVersionsInputRequestTypeDef,
     _OptionalListBackupPlanVersionsInputRequestTypeDef,
 ):
     pass
 
 
-ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    {
-        "IncludeDeleted": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupPlansInputRequestTypeDef = TypedDict(
     "ListBackupPlansInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IncludeDeleted": bool,
     },
     total=False,
 )
 
-_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
-    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBackupSelectionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupSelectionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupSelectionsInputRequestTypeDef = TypedDict(
@@ -1004,102 +792,41 @@
 class ListBackupSelectionsInputRequestTypeDef(
     _RequiredListBackupSelectionsInputRequestTypeDef,
     _OptionalListBackupSelectionsInputRequestTypeDef,
 ):
     pass
 
 
-ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupVaultsInputRequestTypeDef = TypedDict(
     "ListBackupVaultsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListCopyJobsInputRequestTypeDef = TypedDict(
-    "ListCopyJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
 ListFrameworksInputRequestTypeDef = TypedDict(
     "ListFrameworksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLegalHoldsInputRequestTypeDef = TypedDict(
     "ListLegalHoldsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProtectedResourcesInputRequestTypeDef = TypedDict(
     "ListProtectedResourcesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1112,93 +839,14 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "LegalHoldId": str,
-    },
-)
-_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
-    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -1225,36 +873,14 @@
         "ResourceArn": str,
         "ResourceType": str,
         "BackupVaultName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
-    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
@@ -1287,65 +913,23 @@
         "IsParent": bool,
         "ParentRecoveryPointArn": str,
         "ResourceName": str,
     },
     total=False,
 )
 
-ListReportJobsInputRequestTypeDef = TypedDict(
-    "ListReportJobsInputRequestTypeDef",
-    {
-        "ByReportPlanName": str,
-        "ByCreationBefore": Union[datetime, str],
-        "ByCreationAfter": Union[datetime, str],
-        "ByStatus": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListReportPlansInputRequestTypeDef = TypedDict(
     "ListReportPlansInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    {
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRestoreJobsInputRequestTypeDef = TypedDict(
-    "ListRestoreJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 RestoreJobsListMemberTypeDef = TypedDict(
     "RestoreJobsListMemberTypeDef",
     {
         "AccountId": str,
         "RestoreJobId": str,
         "RecoveryPointArn": str,
         "CreationDate": datetime,
@@ -1380,33 +964,14 @@
 
 class ListTagsInputRequestTypeDef(
     _RequiredListTagsInputRequestTypeDef, _OptionalListTagsInputRequestTypeDef
 ):
     pass
 
 
-ListTagsOutputTypeDef = TypedDict(
-    "ListTagsOutputTypeDef",
-    {
-        "NextToken": str,
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
 _RequiredPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -1454,55 +1019,70 @@
     {
         "BackupVaultName": str,
         "SNSTopicArn": str,
         "BackupVaultEvents": Sequence[BackupVaultEventType],
     },
 )
 
-ReportDestinationTypeDef = TypedDict(
-    "ReportDestinationTypeDef",
+_RequiredReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_RequiredReportDeliveryChannelOutputTypeDef",
     {
         "S3BucketName": str,
-        "S3Keys": List[str],
+    },
+)
+_OptionalReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_OptionalReportDeliveryChannelOutputTypeDef",
+    {
+        "S3KeyPrefix": str,
+        "Formats": List[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class ReportDeliveryChannelOutputTypeDef(
+    _RequiredReportDeliveryChannelOutputTypeDef, _OptionalReportDeliveryChannelOutputTypeDef
+):
+    pass
+
+
+ReportDestinationTypeDef = TypedDict(
+    "ReportDestinationTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "S3BucketName": str,
+        "S3Keys": List[str],
     },
+    total=False,
 )
 
-StartBackupJobOutputTypeDef = TypedDict(
-    "StartBackupJobOutputTypeDef",
+_RequiredReportSettingOutputTypeDef = TypedDict(
+    "_RequiredReportSettingOutputTypeDef",
     {
-        "BackupJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReportTemplate": str,
     },
 )
-
-StartCopyJobOutputTypeDef = TypedDict(
-    "StartCopyJobOutputTypeDef",
+_OptionalReportSettingOutputTypeDef = TypedDict(
+    "_OptionalReportSettingOutputTypeDef",
     {
-        "CopyJobId": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FrameworkArns": List[str],
+        "NumberOfFrameworks": int,
+        "Accounts": List[str],
+        "OrganizationUnits": List[str],
+        "Regions": List[str],
     },
+    total=False,
 )
 
+
+class ReportSettingOutputTypeDef(
+    _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
+):
+    pass
+
+
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1516,22 +1096,14 @@
 
 class StartReportJobInputRequestTypeDef(
     _RequiredStartReportJobInputRequestTypeDef, _OptionalStartReportJobInputRequestTypeDef
 ):
     pass
 
 
-StartReportJobOutputTypeDef = TypedDict(
-    "StartReportJobOutputTypeDef",
-    {
-        "ReportJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRestoreJobInputRequestTypeDef = TypedDict(
     "_RequiredStartRestoreJobInputRequestTypeDef",
     {
         "RecoveryPointArn": str,
         "Metadata": Mapping[str, str],
     },
 )
@@ -1549,22 +1121,14 @@
 
 class StartRestoreJobInputRequestTypeDef(
     _RequiredStartRestoreJobInputRequestTypeDef, _OptionalStartRestoreJobInputRequestTypeDef
 ):
     pass
 
 
-StartRestoreJobOutputTypeDef = TypedDict(
-    "StartRestoreJobOutputTypeDef",
-    {
-        "RestoreJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopBackupJobInputRequestTypeDef = TypedDict(
     "StopBackupJobInputRequestTypeDef",
     {
         "BackupJobId": str,
     },
 )
 
@@ -1580,24 +1144,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeyList": Sequence[str],
     },
 )
 
-UpdateFrameworkOutputTypeDef = TypedDict(
-    "UpdateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "GlobalSettings": Mapping[str, str],
     },
     total=False,
 )
@@ -1607,64 +1161,30 @@
     {
         "ResourceTypeOptInPreference": Mapping[str, bool],
         "ResourceTypeManagementPreference": Mapping[str, bool],
     },
     total=False,
 )
 
-UpdateReportPlanOutputTypeDef = TypedDict(
-    "UpdateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupPlansListMemberTypeDef = TypedDict(
     "BackupPlansListMemberTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "VersionId": str,
         "BackupPlanName": str,
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
-CreateBackupPlanOutputTypeDef = TypedDict(
-    "CreateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBackupPlanOutputTypeDef = TypedDict(
-    "UpdateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
         "AccountId": str,
         "BackupJobId": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
@@ -1715,55 +1235,14 @@
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
         "ResourceName": str,
     },
     total=False,
 )
 
-DescribeBackupJobOutputTypeDef = TypedDict(
-    "DescribeBackupJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "BackupJobId": str,
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "State": BackupJobStateType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "ResourceType": str,
-        "BytesTransferred": int,
-        "ExpectedCompletionDate": datetime,
-        "StartBy": datetime,
-        "BackupOptions": Dict[str, str],
-        "BackupType": str,
-        "ParentJobId": str,
-        "IsParent": bool,
-        "NumberOfChildJobs": int,
-        "ChildJobsInState": Dict[BackupJobStateType, int],
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupPlanTemplatesOutputTypeDef = TypedDict(
-    "ListBackupPlanTemplatesOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
         "DestinationBackupVaultArn": str,
     },
 )
 _OptionalCopyActionTypeDef = TypedDict(
@@ -1851,34 +1330,16 @@
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
 
-ListBackupSelectionsOutputTypeDef = TypedDict(
-    "ListBackupSelectionsOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupVaultsOutputTypeDef = TypedDict(
-    "ListBackupVaultsOutputTypeDef",
-    {
-        "BackupVaultList": List[BackupVaultListMemberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeRecoveryPointOutputTypeDef = TypedDict(
-    "DescribeRecoveryPointOutputTypeDef",
+RecoveryPointByBackupVaultTypeDef = TypedDict(
+    "RecoveryPointByBackupVaultTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1889,26 +1350,220 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
-        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-RecoveryPointByBackupVaultTypeDef = TypedDict(
-    "RecoveryPointByBackupVaultTypeDef",
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
+    {
+        "StringEquals": List[ConditionParameterTypeDef],
+        "StringNotEquals": List[ConditionParameterTypeDef],
+        "StringLike": List[ConditionParameterTypeDef],
+        "StringNotLike": List[ConditionParameterTypeDef],
+    },
+    total=False,
+)
+
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
+    {
+        "StringEquals": Sequence[ConditionParameterTypeDef],
+        "StringNotEquals": Sequence[ConditionParameterTypeDef],
+        "StringLike": Sequence[ConditionParameterTypeDef],
+        "StringNotLike": Sequence[ConditionParameterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredFrameworkControlOutputTypeDef = TypedDict(
+    "_RequiredFrameworkControlOutputTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlOutputTypeDef = TypedDict(
+    "_OptionalFrameworkControlOutputTypeDef",
+    {
+        "ControlInputParameters": List[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FrameworkControlOutputTypeDef(
+    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
+):
+    pass
+
+
+_RequiredFrameworkControlTypeDef = TypedDict(
+    "_RequiredFrameworkControlTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlTypeDef = TypedDict(
+    "_OptionalFrameworkControlTypeDef",
+    {
+        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeTypeDef,
+    },
+    total=False,
+)
+
+
+class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
+    pass
+
+
+CreateBackupPlanOutputTypeDef = TypedDict(
+    "CreateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBackupSelectionOutputTypeDef = TypedDict(
+    "CreateBackupSelectionOutputTypeDef",
+    {
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBackupVaultOutputTypeDef = TypedDict(
+    "CreateBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFrameworkOutputTypeDef = TypedDict(
+    "CreateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReportPlanOutputTypeDef = TypedDict(
+    "CreateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupPlanOutputTypeDef = TypedDict(
+    "DeleteBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "DeletionDate": datetime,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupJobOutputTypeDef = TypedDict(
+    "DescribeBackupJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "BackupJobId": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "ResourceArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "State": BackupJobStateType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "ResourceType": str,
+        "BytesTransferred": int,
+        "ExpectedCompletionDate": datetime,
+        "StartBy": datetime,
+        "BackupOptions": Dict[str, str],
+        "BackupType": str,
+        "ParentJobId": str,
+        "IsParent": bool,
+        "NumberOfChildJobs": int,
+        "ChildJobsInState": Dict[BackupJobStateType, int],
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupVaultOutputTypeDef = TypedDict(
+    "DescribeBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "EncryptionKeyArn": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "NumberOfRecoveryPoints": int,
+        "Locked": bool,
+        "MinRetentionDays": int,
+        "MaxRetentionDays": int,
+        "LockDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGlobalSettingsOutputTypeDef = TypedDict(
+    "DescribeGlobalSettingsOutputTypeDef",
+    {
+        "GlobalSettings": Dict[str, str],
+        "LastUpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProtectedResourceOutputTypeDef = TypedDict(
+    "DescribeProtectedResourceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceType": str,
+        "LastBackupTime": datetime,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRecoveryPointOutputTypeDef = TypedDict(
+    "DescribeRecoveryPointOutputTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1919,64 +1574,222 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
+        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+DescribeRegionSettingsOutputTypeDef = TypedDict(
+    "DescribeRegionSettingsOutputTypeDef",
+    {
+        "ResourceTypeOptInPreference": Dict[str, bool],
+        "ResourceTypeManagementPreference": Dict[str, bool],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRestoreJobOutputTypeDef = TypedDict(
+    "DescribeRestoreJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "RestoreJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "Status": RestoreJobStatusType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "ExpectedCompletionTimeMinutes": int,
+        "CreatedResourceArn": str,
+        "ResourceType": str,
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
+ExportBackupPlanTemplateOutputTypeDef = TypedDict(
+    "ExportBackupPlanTemplateOutputTypeDef",
+    {
+        "BackupPlanTemplateJson": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultNotificationsOutputTypeDef = TypedDict(
+    "GetBackupVaultNotificationsOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SNSTopicArn": str,
+        "BackupVaultEvents": List[BackupVaultEventType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "Lifecycle": LifecycleTypeDef,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RestoreMetadata": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionsTypeDef = TypedDict(
-    "ConditionsTypeDef",
+GetSupportedResourceTypesOutputTypeDef = TypedDict(
+    "GetSupportedResourceTypesOutputTypeDef",
     {
-        "StringEquals": Sequence[ConditionParameterTypeDef],
-        "StringNotEquals": Sequence[ConditionParameterTypeDef],
-        "StringLike": Sequence[ConditionParameterTypeDef],
-        "StringNotLike": Sequence[ConditionParameterTypeDef],
+        "ResourceTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredFrameworkControlTypeDef = TypedDict(
-    "_RequiredFrameworkControlTypeDef",
+ListBackupPlanTemplatesOutputTypeDef = TypedDict(
+    "ListBackupPlanTemplatesOutputTypeDef",
     {
-        "ControlName": str,
+        "NextToken": str,
+        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFrameworkControlTypeDef = TypedDict(
-    "_OptionalFrameworkControlTypeDef",
+
+ListBackupSelectionsOutputTypeDef = TypedDict(
+    "ListBackupSelectionsOutputTypeDef",
     {
-        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeTypeDef,
+        "NextToken": str,
+        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListBackupVaultsOutputTypeDef = TypedDict(
+    "ListBackupVaultsOutputTypeDef",
+    {
+        "BackupVaultList": List[BackupVaultListMemberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
-    pass
+ListTagsOutputTypeDef = TypedDict(
+    "ListTagsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartBackupJobOutputTypeDef = TypedDict(
+    "StartBackupJobOutputTypeDef",
+    {
+        "BackupJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartCopyJobOutputTypeDef = TypedDict(
+    "StartCopyJobOutputTypeDef",
+    {
+        "CopyJobId": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReportJobOutputTypeDef = TypedDict(
+    "StartReportJobOutputTypeDef",
+    {
+        "ReportJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRestoreJobOutputTypeDef = TypedDict(
+    "StartRestoreJobOutputTypeDef",
+    {
+        "RestoreJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBackupPlanOutputTypeDef = TypedDict(
+    "UpdateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFrameworkOutputTypeDef = TypedDict(
+    "UpdateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "Lifecycle": LifecycleTypeDef,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateReportPlanOutputTypeDef = TypedDict(
+    "UpdateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
         "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
         "ReportSetting": ReportSettingTypeDef,
@@ -1995,30 +1808,14 @@
 
 class CreateReportPlanInputRequestTypeDef(
     _RequiredCreateReportPlanInputRequestTypeDef, _OptionalCreateReportPlanInputRequestTypeDef
 ):
     pass
 
 
-ReportPlanTypeDef = TypedDict(
-    "ReportPlanTypeDef",
-    {
-        "ReportPlanArn": str,
-        "ReportPlanName": str,
-        "ReportPlanDescription": str,
-        "ReportSetting": ReportSettingTypeDef,
-        "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
-        "DeploymentStatus": str,
-        "CreationTime": datetime,
-        "LastAttemptedExecutionTime": datetime,
-        "LastSuccessfulExecutionTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalUpdateReportPlanInputRequestTypeDef = TypedDict(
@@ -2035,78 +1832,391 @@
 
 class UpdateReportPlanInputRequestTypeDef(
     _RequiredUpdateReportPlanInputRequestTypeDef, _OptionalUpdateReportPlanInputRequestTypeDef
 ):
     pass
 
 
-RecoveryPointSelectionTypeDef = TypedDict(
-    "RecoveryPointSelectionTypeDef",
+RecoveryPointSelectionOutputTypeDef = TypedDict(
+    "RecoveryPointSelectionOutputTypeDef",
     {
-        "VaultNames": Sequence[str],
-        "ResourceIdentifiers": Sequence[str],
-        "DateRange": DateRangeTypeDef,
+        "VaultNames": List[str],
+        "ResourceIdentifiers": List[str],
+        "DateRange": DateRangeOutputTypeDef,
+    },
+    total=False,
+)
+
+DateRangeTypeDef = TypedDict(
+    "DateRangeTypeDef",
+    {
+        "FromDate": TimestampTypeDef,
+        "ToDate": TimestampTypeDef,
+    },
+)
+
+ListBackupJobsInputRequestTypeDef = TypedDict(
+    "ListBackupJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+ListCopyJobsInputRequestTypeDef = TypedDict(
+    "ListCopyJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByParentRecoveryPointArn": str,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
+):
+    pass
+
+
+ListReportJobsInputRequestTypeDef = TypedDict(
+    "ListReportJobsInputRequestTypeDef",
+    {
+        "ByReportPlanName": str,
+        "ByCreationBefore": TimestampTypeDef,
+        "ByCreationAfter": TimestampTypeDef,
+        "ByStatus": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListRestoreJobsInputRequestTypeDef = TypedDict(
+    "ListRestoreJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByAccountId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
         "Frameworks": List[FrameworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLegalHoldsOutputTypeDef = TypedDict(
     "ListLegalHoldsOutputTypeDef",
     {
         "NextToken": str,
         "LegalHolds": List[LegalHoldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
+    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    {
+        "IncludeDeleted": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
+    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+):
+    pass
+
+
+ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByParentRecoveryPointArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "LegalHoldId": str,
+    },
+)
+_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
+    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
+    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+):
+    pass
+
+
+ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
+    {
+        "ByAccountId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
     {
         "Results": List[ProtectedResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByLegalHoldOutputTypeDef = TypedDict(
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     {
         "RecoveryPoints": List[RecoveryPointMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByResourceOutputTypeDef = TypedDict(
     "ListRecoveryPointsByResourceOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRestoreJobsOutputTypeDef = TypedDict(
     "ListRestoreJobsOutputTypeDef",
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReportDeliveryChannelUnionTypeDef = Union[
+    ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+]
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
         "ReportPlanArn": str,
         "ReportTemplate": str,
         "CreationTime": datetime,
@@ -2114,55 +2224,72 @@
         "Status": str,
         "StatusMessage": str,
         "ReportDestination": ReportDestinationTypeDef,
     },
     total=False,
 )
 
+ReportPlanTypeDef = TypedDict(
+    "ReportPlanTypeDef",
+    {
+        "ReportPlanArn": str,
+        "ReportPlanName": str,
+        "ReportPlanDescription": str,
+        "ReportSetting": ReportSettingOutputTypeDef,
+        "ReportDeliveryChannel": ReportDeliveryChannelOutputTypeDef,
+        "DeploymentStatus": str,
+        "CreationTime": datetime,
+        "LastAttemptedExecutionTime": datetime,
+        "LastSuccessfulExecutionTime": datetime,
+    },
+    total=False,
+)
+
+ReportSettingUnionTypeDef = Union[ReportSettingTypeDef, ReportSettingOutputTypeDef]
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupPlansOutputTypeDef = TypedDict(
     "ListBackupPlansOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlansList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupJobsOutputTypeDef = TypedDict(
     "ListBackupJobsOutputTypeDef",
     {
         "BackupJobs": List[BackupJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCopyJobOutputTypeDef = TypedDict(
     "DescribeCopyJobOutputTypeDef",
     {
         "CopyJob": CopyJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCopyJobsOutputTypeDef = TypedDict(
     "ListCopyJobsOutputTypeDef",
     {
         "CopyJobs": List[CopyJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupRuleInputTypeDef = TypedDict(
     "_RequiredBackupRuleInputTypeDef",
     {
         "RuleName": str,
@@ -2216,155 +2343,93 @@
 
 
 ListRecoveryPointsByBackupVaultOutputTypeDef = TypedDict(
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBackupSelectionTypeDef = TypedDict(
-    "_RequiredBackupSelectionTypeDef",
+_RequiredBackupSelectionOutputTypeDef = TypedDict(
+    "_RequiredBackupSelectionOutputTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
-_OptionalBackupSelectionTypeDef = TypedDict(
-    "_OptionalBackupSelectionTypeDef",
+_OptionalBackupSelectionOutputTypeDef = TypedDict(
+    "_OptionalBackupSelectionOutputTypeDef",
     {
-        "Resources": Sequence[str],
-        "ListOfTags": Sequence[ConditionTypeDef],
-        "NotResources": Sequence[str],
-        "Conditions": ConditionsTypeDef,
+        "Resources": List[str],
+        "ListOfTags": List[ConditionTypeDef],
+        "NotResources": List[str],
+        "Conditions": ConditionsOutputTypeDef,
     },
     total=False,
 )
 
 
-class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
+class BackupSelectionOutputTypeDef(
+    _RequiredBackupSelectionOutputTypeDef, _OptionalBackupSelectionOutputTypeDef
+):
     pass
 
 
-_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredCreateFrameworkInputRequestTypeDef",
+_RequiredBackupSelectionTypeDef = TypedDict(
+    "_RequiredBackupSelectionTypeDef",
     {
-        "FrameworkName": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "SelectionName": str,
+        "IamRoleArn": str,
     },
 )
-_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalCreateFrameworkInputRequestTypeDef",
+_OptionalBackupSelectionTypeDef = TypedDict(
+    "_OptionalBackupSelectionTypeDef",
     {
-        "FrameworkDescription": str,
-        "IdempotencyToken": str,
-        "FrameworkTags": Mapping[str, str],
+        "Resources": Sequence[str],
+        "ListOfTags": Sequence[ConditionTypeDef],
+        "NotResources": Sequence[str],
+        "Conditions": ConditionsTypeDef,
     },
     total=False,
 )
 
 
-class CreateFrameworkInputRequestTypeDef(
-    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
-):
+class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
     pass
 
 
 DescribeFrameworkOutputTypeDef = TypedDict(
     "DescribeFrameworkOutputTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
-        "FrameworkControls": List[FrameworkControlTypeDef],
+        "FrameworkControls": List[FrameworkControlOutputTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-    },
-)
-_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateFrameworkInputRequestTypeDef(
-    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
-):
-    pass
-
-
-DescribeReportPlanOutputTypeDef = TypedDict(
-    "DescribeReportPlanOutputTypeDef",
-    {
-        "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportPlansOutputTypeDef = TypedDict(
-    "ListReportPlansOutputTypeDef",
-    {
-        "ReportPlans": List[ReportPlanTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_RequiredCreateLegalHoldInputRequestTypeDef",
-    {
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_OptionalCreateLegalHoldInputRequestTypeDef",
-    {
-        "IdempotencyToken": str,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateLegalHoldInputRequestTypeDef(
-    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
-):
-    pass
-
-
+FrameworkControlUnionTypeDef = Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
 CreateLegalHoldOutputTypeDef = TypedDict(
     "CreateLegalHoldOutputTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLegalHoldOutputTypeDef = TypedDict(
     "GetLegalHoldOutputTypeDef",
     {
         "Title": str,
@@ -2372,33 +2437,60 @@
         "Description": str,
         "CancelDescription": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecoveryPointSelectionTypeDef = TypedDict(
+    "RecoveryPointSelectionTypeDef",
+    {
+        "VaultNames": Sequence[str],
+        "ResourceIdentifiers": Sequence[str],
+        "DateRange": DateRangeTypeDef,
+    },
+    total=False,
+)
+
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReportJobsOutputTypeDef = TypedDict(
     "ListReportJobsOutputTypeDef",
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReportPlanOutputTypeDef = TypedDict(
+    "DescribeReportPlanOutputTypeDef",
+    {
+        "ReportPlan": ReportPlanTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportPlansOutputTypeDef = TypedDict(
+    "ListReportPlansOutputTypeDef",
+    {
+        "ReportPlans": List[ReportPlanTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
@@ -2424,24 +2516,37 @@
         "BackupPlanName": str,
         "Rules": List[BackupRuleTypeDef],
     },
 )
 _OptionalBackupPlanTypeDef = TypedDict(
     "_OptionalBackupPlanTypeDef",
     {
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
 
 class BackupPlanTypeDef(_RequiredBackupPlanTypeDef, _OptionalBackupPlanTypeDef):
     pass
 
 
+GetBackupSelectionOutputTypeDef = TypedDict(
+    "GetBackupSelectionOutputTypeDef",
+    {
+        "BackupSelection": BackupSelectionOutputTypeDef,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BackupSelectionUnionTypeDef = Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef]
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2457,26 +2562,88 @@
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
 
-GetBackupSelectionOutputTypeDef = TypedDict(
-    "GetBackupSelectionOutputTypeDef",
+_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredCreateFrameworkInputRequestTypeDef",
     {
-        "BackupSelection": BackupSelectionTypeDef,
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FrameworkName": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+    },
+)
+_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalCreateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "IdempotencyToken": str,
+        "FrameworkTags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateFrameworkInputRequestTypeDef(
+    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkName": str,
     },
 )
+_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateFrameworkInputRequestTypeDef(
+    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_RequiredCreateLegalHoldInputRequestTypeDef",
+    {
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_OptionalCreateLegalHoldInputRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateLegalHoldInputRequestTypeDef(
+    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
+):
+    pass
+
 
+RecoveryPointSelectionUnionTypeDef = Union[
+    RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
+]
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
@@ -2503,34 +2670,34 @@
     },
 )
 
 GetBackupPlanFromJSONOutputTypeDef = TypedDict(
     "GetBackupPlanFromJSONOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanFromTemplateOutputTypeDef = TypedDict(
     "GetBackupPlanFromTemplateOutputTypeDef",
     {
         "BackupPlanDocument": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanOutputTypeDef = TypedDict(
     "GetBackupPlanOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup/type_defs.pyi` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for backup service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingTypeDef
+    from types_aiobotocore_backup.type_defs import AdvancedBackupSettingOutputTypeDef
 
-    data: AdvancedBackupSettingTypeDef = {...}
+    data: AdvancedBackupSettingOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -31,190 +31,214 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
     "ConditionParameterTypeDef",
     "ControlInputParameterTypeDef",
+    "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
-    "CreateBackupSelectionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
-    "CreateBackupVaultOutputTypeDef",
-    "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
-    "CreateReportPlanOutputTypeDef",
-    "DateRangeTypeDef",
+    "DateRangeOutputTypeDef",
+    "TimestampTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
-    "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
     "DeleteRecoveryPointInputRequestTypeDef",
     "DeleteReportPlanInputRequestTypeDef",
     "DescribeBackupJobInputRequestTypeDef",
     "DescribeBackupVaultInputRequestTypeDef",
-    "DescribeBackupVaultOutputTypeDef",
     "DescribeCopyJobInputRequestTypeDef",
     "DescribeFrameworkInputRequestTypeDef",
-    "DescribeGlobalSettingsOutputTypeDef",
     "DescribeProtectedResourceInputRequestTypeDef",
-    "DescribeProtectedResourceOutputTypeDef",
     "DescribeRecoveryPointInputRequestTypeDef",
-    "DescribeRegionSettingsOutputTypeDef",
     "DescribeReportJobInputRequestTypeDef",
     "DescribeReportPlanInputRequestTypeDef",
     "DescribeRestoreJobInputRequestTypeDef",
-    "DescribeRestoreJobOutputTypeDef",
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     "DisassociateRecoveryPointInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportBackupPlanTemplateInputRequestTypeDef",
-    "ExportBackupPlanTemplateOutputTypeDef",
     "FrameworkTypeDef",
     "GetBackupPlanFromJSONInputRequestTypeDef",
     "GetBackupPlanFromTemplateInputRequestTypeDef",
     "GetBackupPlanInputRequestTypeDef",
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
-    "GetBackupVaultAccessPolicyOutputTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
-    "GetBackupVaultNotificationsOutputTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    "GetSupportedResourceTypesOutputTypeDef",
     "LegalHoldTypeDef",
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    "ListBackupJobsInputRequestTypeDef",
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
-    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupPlansInputRequestTypeDef",
-    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
-    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
-    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
-    "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
-    "ListTagsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
+    "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartBackupJobOutputTypeDef",
-    "StartCopyJobOutputTypeDef",
+    "ReportSettingOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
-    "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
-    "StartRestoreJobOutputTypeDef",
     "StopBackupJobInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "UpdateFrameworkOutputTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateRegionSettingsInputRequestTypeDef",
-    "UpdateReportPlanOutputTypeDef",
     "BackupPlansListMemberTypeDef",
-    "CreateBackupPlanOutputTypeDef",
-    "UpdateBackupPlanOutputTypeDef",
     "BackupJobTypeDef",
     "CopyJobTypeDef",
-    "DescribeBackupJobOutputTypeDef",
-    "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
-    "ListBackupSelectionsOutputTypeDef",
-    "ListBackupVaultsOutputTypeDef",
-    "DescribeRecoveryPointOutputTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
+    "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
+    "CreateBackupPlanOutputTypeDef",
+    "CreateBackupSelectionOutputTypeDef",
+    "CreateBackupVaultOutputTypeDef",
+    "CreateFrameworkOutputTypeDef",
+    "CreateReportPlanOutputTypeDef",
+    "DeleteBackupPlanOutputTypeDef",
+    "DescribeBackupJobOutputTypeDef",
+    "DescribeBackupVaultOutputTypeDef",
+    "DescribeGlobalSettingsOutputTypeDef",
+    "DescribeProtectedResourceOutputTypeDef",
+    "DescribeRecoveryPointOutputTypeDef",
+    "DescribeRegionSettingsOutputTypeDef",
+    "DescribeRestoreJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportBackupPlanTemplateOutputTypeDef",
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    "GetBackupVaultNotificationsOutputTypeDef",
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
+    "GetSupportedResourceTypesOutputTypeDef",
+    "ListBackupPlanTemplatesOutputTypeDef",
+    "ListBackupSelectionsOutputTypeDef",
+    "ListBackupVaultsOutputTypeDef",
+    "ListTagsOutputTypeDef",
+    "StartBackupJobOutputTypeDef",
+    "StartCopyJobOutputTypeDef",
+    "StartReportJobOutputTypeDef",
+    "StartRestoreJobOutputTypeDef",
+    "UpdateBackupPlanOutputTypeDef",
+    "UpdateFrameworkOutputTypeDef",
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
-    "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
-    "RecoveryPointSelectionTypeDef",
+    "RecoveryPointSelectionOutputTypeDef",
+    "DateRangeTypeDef",
+    "ListBackupJobsInputRequestTypeDef",
+    "ListCopyJobsInputRequestTypeDef",
+    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    "ListReportJobsInputRequestTypeDef",
+    "ListRestoreJobsInputRequestTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    "ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
+    "ReportDeliveryChannelUnionTypeDef",
     "ReportJobTypeDef",
+    "ReportPlanTypeDef",
+    "ReportSettingUnionTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
+    "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
     "DescribeFrameworkOutputTypeDef",
-    "UpdateFrameworkInputRequestTypeDef",
-    "DescribeReportPlanOutputTypeDef",
-    "ListReportPlansOutputTypeDef",
-    "CreateLegalHoldInputRequestTypeDef",
+    "FrameworkControlUnionTypeDef",
     "CreateLegalHoldOutputTypeDef",
     "GetLegalHoldOutputTypeDef",
+    "RecoveryPointSelectionTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
+    "DescribeReportPlanOutputTypeDef",
+    "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
-    "CreateBackupSelectionInputRequestTypeDef",
     "GetBackupSelectionOutputTypeDef",
+    "BackupSelectionUnionTypeDef",
+    "CreateBackupSelectionInputRequestTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
+    "UpdateFrameworkInputRequestTypeDef",
+    "CreateLegalHoldInputRequestTypeDef",
+    "RecoveryPointSelectionUnionTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
+AdvancedBackupSettingOutputTypeDef = TypedDict(
+    "AdvancedBackupSettingOutputTypeDef",
+    {
+        "ResourceType": str,
+        "BackupOptions": Dict[str, str],
+    },
+    total=False,
+)
+
 AdvancedBackupSettingTypeDef = TypedDict(
     "AdvancedBackupSettingTypeDef",
     {
         "ResourceType": str,
         "BackupOptions": Mapping[str, str],
     },
     total=False,
@@ -331,31 +355,42 @@
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
 )
 
+ControlScopeOutputTypeDef = TypedDict(
+    "ControlScopeOutputTypeDef",
+    {
+        "ComplianceResourceIds": List[str],
+        "ComplianceResourceTypes": List[str],
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ControlScopeTypeDef = TypedDict(
     "ControlScopeTypeDef",
     {
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateBackupSelectionOutputTypeDef = TypedDict(
-    "CreateBackupSelectionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateBackupVaultInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
@@ -372,33 +407,14 @@
 )
 
 class CreateBackupVaultInputRequestTypeDef(
     _RequiredCreateBackupVaultInputRequestTypeDef, _OptionalCreateBackupVaultInputRequestTypeDef
 ):
     pass
 
-CreateBackupVaultOutputTypeDef = TypedDict(
-    "CreateBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFrameworkOutputTypeDef = TypedDict(
-    "CreateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReportDeliveryChannelTypeDef = TypedDict(
     "_RequiredReportDeliveryChannelTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalReportDeliveryChannelTypeDef = TypedDict(
@@ -432,50 +448,30 @@
     },
     total=False,
 )
 
 class ReportSettingTypeDef(_RequiredReportSettingTypeDef, _OptionalReportSettingTypeDef):
     pass
 
-CreateReportPlanOutputTypeDef = TypedDict(
-    "CreateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DateRangeTypeDef = TypedDict(
-    "DateRangeTypeDef",
+DateRangeOutputTypeDef = TypedDict(
+    "DateRangeOutputTypeDef",
     {
-        "FromDate": Union[datetime, str],
-        "ToDate": Union[datetime, str],
+        "FromDate": datetime,
+        "ToDate": datetime,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-DeleteBackupPlanOutputTypeDef = TypedDict(
-    "DeleteBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "DeletionDate": datetime,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBackupSelectionInputRequestTypeDef = TypedDict(
     "DeleteBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "SelectionId": str,
     },
 )
@@ -540,89 +536,43 @@
 DescribeBackupVaultInputRequestTypeDef = TypedDict(
     "DescribeBackupVaultInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-DescribeBackupVaultOutputTypeDef = TypedDict(
-    "DescribeBackupVaultOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "EncryptionKeyArn": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "NumberOfRecoveryPoints": int,
-        "Locked": bool,
-        "MinRetentionDays": int,
-        "MaxRetentionDays": int,
-        "LockDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCopyJobInputRequestTypeDef = TypedDict(
     "DescribeCopyJobInputRequestTypeDef",
     {
         "CopyJobId": str,
     },
 )
 
 DescribeFrameworkInputRequestTypeDef = TypedDict(
     "DescribeFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 
-DescribeGlobalSettingsOutputTypeDef = TypedDict(
-    "DescribeGlobalSettingsOutputTypeDef",
-    {
-        "GlobalSettings": Dict[str, str],
-        "LastUpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProtectedResourceInputRequestTypeDef = TypedDict(
     "DescribeProtectedResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-DescribeProtectedResourceOutputTypeDef = TypedDict(
-    "DescribeProtectedResourceOutputTypeDef",
-    {
-        "ResourceArn": str,
-        "ResourceType": str,
-        "LastBackupTime": datetime,
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRecoveryPointInputRequestTypeDef = TypedDict(
     "DescribeRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-DescribeRegionSettingsOutputTypeDef = TypedDict(
-    "DescribeRegionSettingsOutputTypeDef",
-    {
-        "ResourceTypeOptInPreference": Dict[str, bool],
-        "ResourceTypeManagementPreference": Dict[str, bool],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeReportJobInputRequestTypeDef = TypedDict(
     "DescribeReportJobInputRequestTypeDef",
     {
         "ReportJobId": str,
     },
 )
 
@@ -636,34 +586,14 @@
 DescribeRestoreJobInputRequestTypeDef = TypedDict(
     "DescribeRestoreJobInputRequestTypeDef",
     {
         "RestoreJobId": str,
     },
 )
 
-DescribeRestoreJobOutputTypeDef = TypedDict(
-    "DescribeRestoreJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "RestoreJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "Status": RestoreJobStatusType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "ExpectedCompletionTimeMinutes": int,
-        "CreatedResourceArn": str,
-        "ResourceType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateRecoveryPointFromParentInputRequestTypeDef = TypedDict(
     "DisassociateRecoveryPointFromParentInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
@@ -672,36 +602,21 @@
     "DisassociateRecoveryPointInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportBackupPlanTemplateInputRequestTypeDef = TypedDict(
     "ExportBackupPlanTemplateInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
-ExportBackupPlanTemplateOutputTypeDef = TypedDict(
-    "ExportBackupPlanTemplateOutputTypeDef",
-    {
-        "BackupPlanTemplateJson": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FrameworkTypeDef = TypedDict(
     "FrameworkTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
         "NumberOfControls": int,
@@ -755,42 +670,21 @@
 GetBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
-    "GetBackupVaultAccessPolicyOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBackupVaultNotificationsInputRequestTypeDef = TypedDict(
     "GetBackupVaultNotificationsInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 
-GetBackupVaultNotificationsOutputTypeDef = TypedDict(
-    "GetBackupVaultNotificationsOutputTypeDef",
-    {
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "SNSTopicArn": str,
-        "BackupVaultEvents": List[BackupVaultEventType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLegalHoldInputRequestTypeDef = TypedDict(
     "GetLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 
@@ -798,120 +692,47 @@
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     {
         "BackupVaultName": str,
         "RecoveryPointArn": str,
     },
 )
 
-GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
-    "GetRecoveryPointRestoreMetadataOutputTypeDef",
-    {
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "RestoreMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSupportedResourceTypesOutputTypeDef = TypedDict(
-    "GetSupportedResourceTypesOutputTypeDef",
-    {
-        "ResourceTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LegalHoldTypeDef = TypedDict(
     "LegalHoldTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
     },
     total=False,
 )
 
-ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
-    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListBackupJobsInputRequestTypeDef = TypedDict(
-    "ListBackupJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
-ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
-    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
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
 
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
-    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBackupPlanVersionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupPlanVersionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupPlanVersionsInputRequestTypeDef = TypedDict(
@@ -925,53 +746,24 @@
 
 class ListBackupPlanVersionsInputRequestTypeDef(
     _RequiredListBackupPlanVersionsInputRequestTypeDef,
     _OptionalListBackupPlanVersionsInputRequestTypeDef,
 ):
     pass
 
-ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
-    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
-    {
-        "IncludeDeleted": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupPlansInputRequestTypeDef = TypedDict(
     "ListBackupPlansInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IncludeDeleted": bool,
     },
     total=False,
 )
 
-_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "BackupPlanId": str,
-    },
-)
-_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
-    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
-    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBackupSelectionsInputRequestTypeDef = TypedDict(
     "_RequiredListBackupSelectionsInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 _OptionalListBackupSelectionsInputRequestTypeDef = TypedDict(
@@ -985,102 +777,41 @@
 
 class ListBackupSelectionsInputRequestTypeDef(
     _RequiredListBackupSelectionsInputRequestTypeDef,
     _OptionalListBackupSelectionsInputRequestTypeDef,
 ):
     pass
 
-ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
-    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBackupVaultsInputRequestTypeDef = TypedDict(
     "ListBackupVaultsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
-    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListCopyJobsInputRequestTypeDef = TypedDict(
-    "ListCopyJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
 ListFrameworksInputRequestTypeDef = TypedDict(
     "ListFrameworksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
-    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLegalHoldsInputRequestTypeDef = TypedDict(
     "ListLegalHoldsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
-    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProtectedResourcesInputRequestTypeDef = TypedDict(
     "ListProtectedResourcesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1093,87 +824,14 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
-    {
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-):
-    pass
-
-_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
-):
-    pass
-
-_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "LegalHoldId": str,
-    },
-)
-_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
-    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
-):
-    pass
-
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -1198,34 +856,14 @@
         "ResourceArn": str,
         "ResourceType": str,
         "BackupVaultName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
-    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListRecoveryPointsByResourceInputRequestTypeDef = TypedDict(
@@ -1256,65 +894,23 @@
         "IsParent": bool,
         "ParentRecoveryPointArn": str,
         "ResourceName": str,
     },
     total=False,
 )
 
-ListReportJobsInputRequestTypeDef = TypedDict(
-    "ListReportJobsInputRequestTypeDef",
-    {
-        "ByReportPlanName": str,
-        "ByCreationBefore": Union[datetime, str],
-        "ByCreationAfter": Union[datetime, str],
-        "ByStatus": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListReportPlansInputRequestTypeDef = TypedDict(
     "ListReportPlansInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
-    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
-    {
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRestoreJobsInputRequestTypeDef = TypedDict(
-    "ListRestoreJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 RestoreJobsListMemberTypeDef = TypedDict(
     "RestoreJobsListMemberTypeDef",
     {
         "AccountId": str,
         "RestoreJobId": str,
         "RecoveryPointArn": str,
         "CreationDate": datetime,
@@ -1347,33 +943,14 @@
 )
 
 class ListTagsInputRequestTypeDef(
     _RequiredListTagsInputRequestTypeDef, _OptionalListTagsInputRequestTypeDef
 ):
     pass
 
-ListTagsOutputTypeDef = TypedDict(
-    "ListTagsOutputTypeDef",
-    {
-        "NextToken": str,
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
 _RequiredPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutBackupVaultAccessPolicyInputRequestTypeDef",
     {
         "BackupVaultName": str,
     },
 )
 _OptionalPutBackupVaultAccessPolicyInputRequestTypeDef = TypedDict(
@@ -1417,55 +994,66 @@
     {
         "BackupVaultName": str,
         "SNSTopicArn": str,
         "BackupVaultEvents": Sequence[BackupVaultEventType],
     },
 )
 
-ReportDestinationTypeDef = TypedDict(
-    "ReportDestinationTypeDef",
+_RequiredReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_RequiredReportDeliveryChannelOutputTypeDef",
     {
         "S3BucketName": str,
-        "S3Keys": List[str],
+    },
+)
+_OptionalReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_OptionalReportDeliveryChannelOutputTypeDef",
+    {
+        "S3KeyPrefix": str,
+        "Formats": List[str],
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class ReportDeliveryChannelOutputTypeDef(
+    _RequiredReportDeliveryChannelOutputTypeDef, _OptionalReportDeliveryChannelOutputTypeDef
+):
+    pass
+
+ReportDestinationTypeDef = TypedDict(
+    "ReportDestinationTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "S3BucketName": str,
+        "S3Keys": List[str],
     },
+    total=False,
 )
 
-StartBackupJobOutputTypeDef = TypedDict(
-    "StartBackupJobOutputTypeDef",
+_RequiredReportSettingOutputTypeDef = TypedDict(
+    "_RequiredReportSettingOutputTypeDef",
     {
-        "BackupJobId": str,
-        "RecoveryPointArn": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReportTemplate": str,
     },
 )
-
-StartCopyJobOutputTypeDef = TypedDict(
-    "StartCopyJobOutputTypeDef",
+_OptionalReportSettingOutputTypeDef = TypedDict(
+    "_OptionalReportSettingOutputTypeDef",
     {
-        "CopyJobId": str,
-        "CreationDate": datetime,
-        "IsParent": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FrameworkArns": List[str],
+        "NumberOfFrameworks": int,
+        "Accounts": List[str],
+        "OrganizationUnits": List[str],
+        "Regions": List[str],
     },
+    total=False,
 )
 
+class ReportSettingOutputTypeDef(
+    _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
+):
+    pass
+
 _RequiredStartReportJobInputRequestTypeDef = TypedDict(
     "_RequiredStartReportJobInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalStartReportJobInputRequestTypeDef = TypedDict(
@@ -1477,22 +1065,14 @@
 )
 
 class StartReportJobInputRequestTypeDef(
     _RequiredStartReportJobInputRequestTypeDef, _OptionalStartReportJobInputRequestTypeDef
 ):
     pass
 
-StartReportJobOutputTypeDef = TypedDict(
-    "StartReportJobOutputTypeDef",
-    {
-        "ReportJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRestoreJobInputRequestTypeDef = TypedDict(
     "_RequiredStartRestoreJobInputRequestTypeDef",
     {
         "RecoveryPointArn": str,
         "Metadata": Mapping[str, str],
     },
 )
@@ -1508,22 +1088,14 @@
 )
 
 class StartRestoreJobInputRequestTypeDef(
     _RequiredStartRestoreJobInputRequestTypeDef, _OptionalStartRestoreJobInputRequestTypeDef
 ):
     pass
 
-StartRestoreJobOutputTypeDef = TypedDict(
-    "StartRestoreJobOutputTypeDef",
-    {
-        "RestoreJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopBackupJobInputRequestTypeDef = TypedDict(
     "StopBackupJobInputRequestTypeDef",
     {
         "BackupJobId": str,
     },
 )
 
@@ -1539,24 +1111,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeyList": Sequence[str],
     },
 )
 
-UpdateFrameworkOutputTypeDef = TypedDict(
-    "UpdateFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "GlobalSettings": Mapping[str, str],
     },
     total=False,
 )
@@ -1566,64 +1128,30 @@
     {
         "ResourceTypeOptInPreference": Mapping[str, bool],
         "ResourceTypeManagementPreference": Mapping[str, bool],
     },
     total=False,
 )
 
-UpdateReportPlanOutputTypeDef = TypedDict(
-    "UpdateReportPlanOutputTypeDef",
-    {
-        "ReportPlanName": str,
-        "ReportPlanArn": str,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupPlansListMemberTypeDef = TypedDict(
     "BackupPlansListMemberTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "VersionId": str,
         "BackupPlanName": str,
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
-CreateBackupPlanOutputTypeDef = TypedDict(
-    "CreateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBackupPlanOutputTypeDef = TypedDict(
-    "UpdateBackupPlanOutputTypeDef",
-    {
-        "BackupPlanId": str,
-        "BackupPlanArn": str,
-        "CreationDate": datetime,
-        "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
         "AccountId": str,
         "BackupJobId": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
@@ -1674,55 +1202,14 @@
         "NumberOfChildJobs": int,
         "ChildJobsInState": Dict[CopyJobStateType, int],
         "ResourceName": str,
     },
     total=False,
 )
 
-DescribeBackupJobOutputTypeDef = TypedDict(
-    "DescribeBackupJobOutputTypeDef",
-    {
-        "AccountId": str,
-        "BackupJobId": str,
-        "BackupVaultName": str,
-        "BackupVaultArn": str,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "CreationDate": datetime,
-        "CompletionDate": datetime,
-        "State": BackupJobStateType,
-        "StatusMessage": str,
-        "PercentDone": str,
-        "BackupSizeInBytes": int,
-        "IamRoleArn": str,
-        "CreatedBy": RecoveryPointCreatorTypeDef,
-        "ResourceType": str,
-        "BytesTransferred": int,
-        "ExpectedCompletionDate": datetime,
-        "StartBy": datetime,
-        "BackupOptions": Dict[str, str],
-        "BackupType": str,
-        "ParentJobId": str,
-        "IsParent": bool,
-        "NumberOfChildJobs": int,
-        "ChildJobsInState": Dict[BackupJobStateType, int],
-        "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupPlanTemplatesOutputTypeDef = TypedDict(
-    "ListBackupPlanTemplatesOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyActionTypeDef = TypedDict(
     "_RequiredCopyActionTypeDef",
     {
         "DestinationBackupVaultArn": str,
     },
 )
 _OptionalCopyActionTypeDef = TypedDict(
@@ -1802,34 +1289,16 @@
 
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
-ListBackupSelectionsOutputTypeDef = TypedDict(
-    "ListBackupSelectionsOutputTypeDef",
-    {
-        "NextToken": str,
-        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBackupVaultsOutputTypeDef = TypedDict(
-    "ListBackupVaultsOutputTypeDef",
-    {
-        "BackupVaultList": List[BackupVaultListMemberTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeRecoveryPointOutputTypeDef = TypedDict(
-    "DescribeRecoveryPointOutputTypeDef",
+RecoveryPointByBackupVaultTypeDef = TypedDict(
+    "RecoveryPointByBackupVaultTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1840,26 +1309,216 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
-        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-RecoveryPointByBackupVaultTypeDef = TypedDict(
-    "RecoveryPointByBackupVaultTypeDef",
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
+    {
+        "StringEquals": List[ConditionParameterTypeDef],
+        "StringNotEquals": List[ConditionParameterTypeDef],
+        "StringLike": List[ConditionParameterTypeDef],
+        "StringNotLike": List[ConditionParameterTypeDef],
+    },
+    total=False,
+)
+
+ConditionsTypeDef = TypedDict(
+    "ConditionsTypeDef",
+    {
+        "StringEquals": Sequence[ConditionParameterTypeDef],
+        "StringNotEquals": Sequence[ConditionParameterTypeDef],
+        "StringLike": Sequence[ConditionParameterTypeDef],
+        "StringNotLike": Sequence[ConditionParameterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredFrameworkControlOutputTypeDef = TypedDict(
+    "_RequiredFrameworkControlOutputTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlOutputTypeDef = TypedDict(
+    "_OptionalFrameworkControlOutputTypeDef",
+    {
+        "ControlInputParameters": List[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeOutputTypeDef,
+    },
+    total=False,
+)
+
+class FrameworkControlOutputTypeDef(
+    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
+):
+    pass
+
+_RequiredFrameworkControlTypeDef = TypedDict(
+    "_RequiredFrameworkControlTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlTypeDef = TypedDict(
+    "_OptionalFrameworkControlTypeDef",
+    {
+        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
+        "ControlScope": ControlScopeTypeDef,
+    },
+    total=False,
+)
+
+class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
+    pass
+
+CreateBackupPlanOutputTypeDef = TypedDict(
+    "CreateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBackupSelectionOutputTypeDef = TypedDict(
+    "CreateBackupSelectionOutputTypeDef",
+    {
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBackupVaultOutputTypeDef = TypedDict(
+    "CreateBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "CreationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFrameworkOutputTypeDef = TypedDict(
+    "CreateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateReportPlanOutputTypeDef = TypedDict(
+    "CreateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupPlanOutputTypeDef = TypedDict(
+    "DeleteBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "DeletionDate": datetime,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupJobOutputTypeDef = TypedDict(
+    "DescribeBackupJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "BackupJobId": str,
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "ResourceArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "State": BackupJobStateType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "CreatedBy": RecoveryPointCreatorTypeDef,
+        "ResourceType": str,
+        "BytesTransferred": int,
+        "ExpectedCompletionDate": datetime,
+        "StartBy": datetime,
+        "BackupOptions": Dict[str, str],
+        "BackupType": str,
+        "ParentJobId": str,
+        "IsParent": bool,
+        "NumberOfChildJobs": int,
+        "ChildJobsInState": Dict[BackupJobStateType, int],
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupVaultOutputTypeDef = TypedDict(
+    "DescribeBackupVaultOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "EncryptionKeyArn": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "NumberOfRecoveryPoints": int,
+        "Locked": bool,
+        "MinRetentionDays": int,
+        "MaxRetentionDays": int,
+        "LockDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGlobalSettingsOutputTypeDef = TypedDict(
+    "DescribeGlobalSettingsOutputTypeDef",
+    {
+        "GlobalSettings": Dict[str, str],
+        "LastUpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProtectedResourceOutputTypeDef = TypedDict(
+    "DescribeProtectedResourceOutputTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceType": str,
+        "LastBackupTime": datetime,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRecoveryPointOutputTypeDef = TypedDict(
+    "DescribeRecoveryPointOutputTypeDef",
     {
         "RecoveryPointArn": str,
         "BackupVaultName": str,
         "BackupVaultArn": str,
         "SourceBackupVaultArn": str,
         "ResourceArn": str,
         "ResourceType": str,
@@ -1870,62 +1529,222 @@
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "Lifecycle": LifecycleTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
+        "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
-    "UpdateRecoveryPointLifecycleOutputTypeDef",
+DescribeRegionSettingsOutputTypeDef = TypedDict(
+    "DescribeRegionSettingsOutputTypeDef",
+    {
+        "ResourceTypeOptInPreference": Dict[str, bool],
+        "ResourceTypeManagementPreference": Dict[str, bool],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRestoreJobOutputTypeDef = TypedDict(
+    "DescribeRestoreJobOutputTypeDef",
+    {
+        "AccountId": str,
+        "RestoreJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "CompletionDate": datetime,
+        "Status": RestoreJobStatusType,
+        "StatusMessage": str,
+        "PercentDone": str,
+        "BackupSizeInBytes": int,
+        "IamRoleArn": str,
+        "ExpectedCompletionTimeMinutes": int,
+        "CreatedResourceArn": str,
+        "ResourceType": str,
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
+ExportBackupPlanTemplateOutputTypeDef = TypedDict(
+    "ExportBackupPlanTemplateOutputTypeDef",
+    {
+        "BackupPlanTemplateJson": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultAccessPolicyOutputTypeDef = TypedDict(
+    "GetBackupVaultAccessPolicyOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBackupVaultNotificationsOutputTypeDef = TypedDict(
+    "GetBackupVaultNotificationsOutputTypeDef",
+    {
+        "BackupVaultName": str,
+        "BackupVaultArn": str,
+        "SNSTopicArn": str,
+        "BackupVaultEvents": List[BackupVaultEventType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRecoveryPointRestoreMetadataOutputTypeDef = TypedDict(
+    "GetRecoveryPointRestoreMetadataOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "Lifecycle": LifecycleTypeDef,
-        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RestoreMetadata": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConditionsTypeDef = TypedDict(
-    "ConditionsTypeDef",
+GetSupportedResourceTypesOutputTypeDef = TypedDict(
+    "GetSupportedResourceTypesOutputTypeDef",
     {
-        "StringEquals": Sequence[ConditionParameterTypeDef],
-        "StringNotEquals": Sequence[ConditionParameterTypeDef],
-        "StringLike": Sequence[ConditionParameterTypeDef],
-        "StringNotLike": Sequence[ConditionParameterTypeDef],
+        "ResourceTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredFrameworkControlTypeDef = TypedDict(
-    "_RequiredFrameworkControlTypeDef",
+ListBackupPlanTemplatesOutputTypeDef = TypedDict(
+    "ListBackupPlanTemplatesOutputTypeDef",
     {
-        "ControlName": str,
+        "NextToken": str,
+        "BackupPlanTemplatesList": List[BackupPlanTemplatesListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFrameworkControlTypeDef = TypedDict(
-    "_OptionalFrameworkControlTypeDef",
+
+ListBackupSelectionsOutputTypeDef = TypedDict(
+    "ListBackupSelectionsOutputTypeDef",
     {
-        "ControlInputParameters": Sequence[ControlInputParameterTypeDef],
-        "ControlScope": ControlScopeTypeDef,
+        "NextToken": str,
+        "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class FrameworkControlTypeDef(_RequiredFrameworkControlTypeDef, _OptionalFrameworkControlTypeDef):
-    pass
+ListBackupVaultsOutputTypeDef = TypedDict(
+    "ListBackupVaultsOutputTypeDef",
+    {
+        "BackupVaultList": List[BackupVaultListMemberTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsOutputTypeDef = TypedDict(
+    "ListTagsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartBackupJobOutputTypeDef = TypedDict(
+    "StartBackupJobOutputTypeDef",
+    {
+        "BackupJobId": str,
+        "RecoveryPointArn": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCopyJobOutputTypeDef = TypedDict(
+    "StartCopyJobOutputTypeDef",
+    {
+        "CopyJobId": str,
+        "CreationDate": datetime,
+        "IsParent": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReportJobOutputTypeDef = TypedDict(
+    "StartReportJobOutputTypeDef",
+    {
+        "ReportJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRestoreJobOutputTypeDef = TypedDict(
+    "StartRestoreJobOutputTypeDef",
+    {
+        "RestoreJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBackupPlanOutputTypeDef = TypedDict(
+    "UpdateBackupPlanOutputTypeDef",
+    {
+        "BackupPlanId": str,
+        "BackupPlanArn": str,
+        "CreationDate": datetime,
+        "VersionId": str,
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFrameworkOutputTypeDef = TypedDict(
+    "UpdateFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
+    "UpdateRecoveryPointLifecycleOutputTypeDef",
+    {
+        "BackupVaultArn": str,
+        "RecoveryPointArn": str,
+        "Lifecycle": LifecycleTypeDef,
+        "CalculatedLifecycle": CalculatedLifecycleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateReportPlanOutputTypeDef = TypedDict(
+    "UpdateReportPlanOutputTypeDef",
+    {
+        "ReportPlanName": str,
+        "ReportPlanArn": str,
+        "CreationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
         "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
         "ReportSetting": ReportSettingTypeDef,
@@ -1942,30 +1761,14 @@
 )
 
 class CreateReportPlanInputRequestTypeDef(
     _RequiredCreateReportPlanInputRequestTypeDef, _OptionalCreateReportPlanInputRequestTypeDef
 ):
     pass
 
-ReportPlanTypeDef = TypedDict(
-    "ReportPlanTypeDef",
-    {
-        "ReportPlanArn": str,
-        "ReportPlanName": str,
-        "ReportPlanDescription": str,
-        "ReportSetting": ReportSettingTypeDef,
-        "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
-        "DeploymentStatus": str,
-        "CreationTime": datetime,
-        "LastAttemptedExecutionTime": datetime,
-        "LastSuccessfulExecutionTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalUpdateReportPlanInputRequestTypeDef = TypedDict(
@@ -1980,78 +1783,379 @@
 )
 
 class UpdateReportPlanInputRequestTypeDef(
     _RequiredUpdateReportPlanInputRequestTypeDef, _OptionalUpdateReportPlanInputRequestTypeDef
 ):
     pass
 
-RecoveryPointSelectionTypeDef = TypedDict(
-    "RecoveryPointSelectionTypeDef",
+RecoveryPointSelectionOutputTypeDef = TypedDict(
+    "RecoveryPointSelectionOutputTypeDef",
     {
-        "VaultNames": Sequence[str],
-        "ResourceIdentifiers": Sequence[str],
-        "DateRange": DateRangeTypeDef,
+        "VaultNames": List[str],
+        "ResourceIdentifiers": List[str],
+        "DateRange": DateRangeOutputTypeDef,
+    },
+    total=False,
+)
+
+DateRangeTypeDef = TypedDict(
+    "DateRangeTypeDef",
+    {
+        "FromDate": TimestampTypeDef,
+        "ToDate": TimestampTypeDef,
+    },
+)
+
+ListBackupJobsInputRequestTypeDef = TypedDict(
+    "ListBackupJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+ListCopyJobsInputRequestTypeDef = TypedDict(
+    "ListCopyJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByParentRecoveryPointArn": str,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
+):
+    pass
+
+ListReportJobsInputRequestTypeDef = TypedDict(
+    "ListReportJobsInputRequestTypeDef",
+    {
+        "ByReportPlanName": str,
+        "ByCreationBefore": TimestampTypeDef,
+        "ByCreationAfter": TimestampTypeDef,
+        "ByStatus": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListRestoreJobsInputRequestTypeDef = TypedDict(
+    "ListRestoreJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByAccountId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
         "Frameworks": List[FrameworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLegalHoldsOutputTypeDef = TypedDict(
     "ListLegalHoldsOutputTypeDef",
     {
         "NextToken": str,
         "LegalHolds": List[LegalHoldTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
+    "ListBackupJobsInputListBackupJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
+    "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef(
+    _RequiredListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    _OptionalListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+):
+    pass
+
+ListBackupPlansInputListBackupPlansPaginateTypeDef = TypedDict(
+    "ListBackupPlansInputListBackupPlansPaginateTypeDef",
+    {
+        "IncludeDeleted": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "BackupPlanId": str,
+    },
+)
+_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = TypedDict(
+    "_OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef(
+    _RequiredListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    _OptionalListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+):
+    pass
+
+ListBackupVaultsInputListBackupVaultsPaginateTypeDef = TypedDict(
+    "ListBackupVaultsInputListBackupVaultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
+    "ListCopyJobsInputListCopyJobsPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByParentJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
+    "ListLegalHoldsInputListLegalHoldsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = TypedDict(
+    "ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
+    {
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByParentRecoveryPointArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+):
+    pass
+
+_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "LegalHoldId": str,
+    },
+)
+_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef(
+    _RequiredListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    _OptionalListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+):
+    pass
+
+_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef(
+    _RequiredListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    _OptionalListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+):
+    pass
+
+ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
+    "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
+    {
+        "ByAccountId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
     {
         "Results": List[ProtectedResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByLegalHoldOutputTypeDef = TypedDict(
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     {
         "RecoveryPoints": List[RecoveryPointMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsByResourceOutputTypeDef = TypedDict(
     "ListRecoveryPointsByResourceOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRestoreJobsOutputTypeDef = TypedDict(
     "ListRestoreJobsOutputTypeDef",
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReportDeliveryChannelUnionTypeDef = Union[
+    ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+]
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
         "ReportPlanArn": str,
         "ReportTemplate": str,
         "CreationTime": datetime,
@@ -2059,55 +2163,72 @@
         "Status": str,
         "StatusMessage": str,
         "ReportDestination": ReportDestinationTypeDef,
     },
     total=False,
 )
 
+ReportPlanTypeDef = TypedDict(
+    "ReportPlanTypeDef",
+    {
+        "ReportPlanArn": str,
+        "ReportPlanName": str,
+        "ReportPlanDescription": str,
+        "ReportSetting": ReportSettingOutputTypeDef,
+        "ReportDeliveryChannel": ReportDeliveryChannelOutputTypeDef,
+        "DeploymentStatus": str,
+        "CreationTime": datetime,
+        "LastAttemptedExecutionTime": datetime,
+        "LastSuccessfulExecutionTime": datetime,
+    },
+    total=False,
+)
+
+ReportSettingUnionTypeDef = Union[ReportSettingTypeDef, ReportSettingOutputTypeDef]
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupPlansOutputTypeDef = TypedDict(
     "ListBackupPlansOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlansList": List[BackupPlansListMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBackupJobsOutputTypeDef = TypedDict(
     "ListBackupJobsOutputTypeDef",
     {
         "BackupJobs": List[BackupJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCopyJobOutputTypeDef = TypedDict(
     "DescribeCopyJobOutputTypeDef",
     {
         "CopyJob": CopyJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCopyJobsOutputTypeDef = TypedDict(
     "ListCopyJobsOutputTypeDef",
     {
         "CopyJobs": List[CopyJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupRuleInputTypeDef = TypedDict(
     "_RequiredBackupRuleInputTypeDef",
     {
         "RuleName": str,
@@ -2157,147 +2278,89 @@
     pass
 
 ListRecoveryPointsByBackupVaultOutputTypeDef = TypedDict(
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBackupSelectionTypeDef = TypedDict(
-    "_RequiredBackupSelectionTypeDef",
+_RequiredBackupSelectionOutputTypeDef = TypedDict(
+    "_RequiredBackupSelectionOutputTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
-_OptionalBackupSelectionTypeDef = TypedDict(
-    "_OptionalBackupSelectionTypeDef",
+_OptionalBackupSelectionOutputTypeDef = TypedDict(
+    "_OptionalBackupSelectionOutputTypeDef",
     {
-        "Resources": Sequence[str],
-        "ListOfTags": Sequence[ConditionTypeDef],
-        "NotResources": Sequence[str],
-        "Conditions": ConditionsTypeDef,
+        "Resources": List[str],
+        "ListOfTags": List[ConditionTypeDef],
+        "NotResources": List[str],
+        "Conditions": ConditionsOutputTypeDef,
     },
     total=False,
 )
 
-class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
+class BackupSelectionOutputTypeDef(
+    _RequiredBackupSelectionOutputTypeDef, _OptionalBackupSelectionOutputTypeDef
+):
     pass
 
-_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredCreateFrameworkInputRequestTypeDef",
+_RequiredBackupSelectionTypeDef = TypedDict(
+    "_RequiredBackupSelectionTypeDef",
     {
-        "FrameworkName": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
+        "SelectionName": str,
+        "IamRoleArn": str,
     },
 )
-_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalCreateFrameworkInputRequestTypeDef",
+_OptionalBackupSelectionTypeDef = TypedDict(
+    "_OptionalBackupSelectionTypeDef",
     {
-        "FrameworkDescription": str,
-        "IdempotencyToken": str,
-        "FrameworkTags": Mapping[str, str],
+        "Resources": Sequence[str],
+        "ListOfTags": Sequence[ConditionTypeDef],
+        "NotResources": Sequence[str],
+        "Conditions": ConditionsTypeDef,
     },
     total=False,
 )
 
-class CreateFrameworkInputRequestTypeDef(
-    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
-):
+class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
     pass
 
 DescribeFrameworkOutputTypeDef = TypedDict(
     "DescribeFrameworkOutputTypeDef",
     {
         "FrameworkName": str,
         "FrameworkArn": str,
         "FrameworkDescription": str,
-        "FrameworkControls": List[FrameworkControlTypeDef],
+        "FrameworkControls": List[FrameworkControlOutputTypeDef],
         "CreationTime": datetime,
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-    },
-)
-_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "FrameworkControls": Sequence[FrameworkControlTypeDef],
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-class UpdateFrameworkInputRequestTypeDef(
-    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
-):
-    pass
-
-DescribeReportPlanOutputTypeDef = TypedDict(
-    "DescribeReportPlanOutputTypeDef",
-    {
-        "ReportPlan": ReportPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportPlansOutputTypeDef = TypedDict(
-    "ListReportPlansOutputTypeDef",
-    {
-        "ReportPlans": List[ReportPlanTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_RequiredCreateLegalHoldInputRequestTypeDef",
-    {
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_OptionalCreateLegalHoldInputRequestTypeDef",
-    {
-        "IdempotencyToken": str,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "Tags": Mapping[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateLegalHoldInputRequestTypeDef(
-    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
-):
-    pass
-
+FrameworkControlUnionTypeDef = Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
 CreateLegalHoldOutputTypeDef = TypedDict(
     "CreateLegalHoldOutputTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLegalHoldOutputTypeDef = TypedDict(
     "GetLegalHoldOutputTypeDef",
     {
         "Title": str,
@@ -2305,33 +2368,60 @@
         "Description": str,
         "CancelDescription": str,
         "LegalHoldId": str,
         "LegalHoldArn": str,
         "CreationDate": datetime,
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecoveryPointSelectionTypeDef = TypedDict(
+    "RecoveryPointSelectionTypeDef",
+    {
+        "VaultNames": Sequence[str],
+        "ResourceIdentifiers": Sequence[str],
+        "DateRange": DateRangeTypeDef,
     },
+    total=False,
 )
 
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReportJobsOutputTypeDef = TypedDict(
     "ListReportJobsOutputTypeDef",
     {
         "ReportJobs": List[ReportJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReportPlanOutputTypeDef = TypedDict(
+    "DescribeReportPlanOutputTypeDef",
+    {
+        "ReportPlan": ReportPlanTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReportPlansOutputTypeDef = TypedDict(
+    "ListReportPlansOutputTypeDef",
+    {
+        "ReportPlans": List[ReportPlanTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
     {
         "BackupPlanName": str,
@@ -2355,22 +2445,35 @@
         "BackupPlanName": str,
         "Rules": List[BackupRuleTypeDef],
     },
 )
 _OptionalBackupPlanTypeDef = TypedDict(
     "_OptionalBackupPlanTypeDef",
     {
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
 class BackupPlanTypeDef(_RequiredBackupPlanTypeDef, _OptionalBackupPlanTypeDef):
     pass
 
+GetBackupSelectionOutputTypeDef = TypedDict(
+    "GetBackupSelectionOutputTypeDef",
+    {
+        "BackupSelection": BackupSelectionOutputTypeDef,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BackupSelectionUnionTypeDef = Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef]
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2384,26 +2487,82 @@
 
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
-GetBackupSelectionOutputTypeDef = TypedDict(
-    "GetBackupSelectionOutputTypeDef",
+_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredCreateFrameworkInputRequestTypeDef",
     {
-        "BackupSelection": BackupSelectionTypeDef,
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FrameworkName": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+    },
+)
+_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalCreateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "IdempotencyToken": str,
+        "FrameworkTags": Mapping[str, str],
     },
+    total=False,
+)
+
+class CreateFrameworkInputRequestTypeDef(
+    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
+):
+    pass
+
+_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkName": str,
+    },
+)
+_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+class UpdateFrameworkInputRequestTypeDef(
+    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
+):
+    pass
+
+_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_RequiredCreateLegalHoldInputRequestTypeDef",
+    {
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_OptionalCreateLegalHoldInputRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
 )
 
+class CreateLegalHoldInputRequestTypeDef(
+    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
+):
+    pass
+
+RecoveryPointSelectionUnionTypeDef = Union[
+    RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
+]
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
@@ -2428,34 +2587,34 @@
     },
 )
 
 GetBackupPlanFromJSONOutputTypeDef = TypedDict(
     "GetBackupPlanFromJSONOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanFromTemplateOutputTypeDef = TypedDict(
     "GetBackupPlanFromTemplateOutputTypeDef",
     {
         "BackupPlanDocument": BackupPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBackupPlanOutputTypeDef = TypedDict(
     "GetBackupPlanOutputTypeDef",
     {
         "BackupPlan": BackupPlanTypeDef,
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/PKG-INFO` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Backup 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore backup type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore backup type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backup"></a>
 
 # types-aiobotocore-backup
 
 [![PyPI - types-aiobotocore-backup](https://img.shields.io/pypi/v/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backup?color=blue)](https://pypistats.org/packages/types-aiobotocore-backup)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup)](https://pepy.tech/project/types-aiobotocore-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Backup 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [types-aiobotocore-backup docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup/).
 
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
@@ -370,201 +369,216 @@
 )
 
 
 def check_value(value: BackupJobStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backup.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backup.type_defs import (
+    AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
     ConditionParameterTypeDef,
     ControlInputParameterTypeDef,
+    ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
-    CreateBackupSelectionOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
-    CreateBackupVaultOutputTypeDef,
-    CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
-    CreateReportPlanOutputTypeDef,
-    DateRangeTypeDef,
+    DateRangeOutputTypeDef,
+    TimestampTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
-    DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
     DeleteRecoveryPointInputRequestTypeDef,
     DeleteReportPlanInputRequestTypeDef,
     DescribeBackupJobInputRequestTypeDef,
     DescribeBackupVaultInputRequestTypeDef,
-    DescribeBackupVaultOutputTypeDef,
     DescribeCopyJobInputRequestTypeDef,
     DescribeFrameworkInputRequestTypeDef,
-    DescribeGlobalSettingsOutputTypeDef,
     DescribeProtectedResourceInputRequestTypeDef,
-    DescribeProtectedResourceOutputTypeDef,
     DescribeRecoveryPointInputRequestTypeDef,
-    DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobInputRequestTypeDef,
     DescribeReportPlanInputRequestTypeDef,
     DescribeRestoreJobInputRequestTypeDef,
-    DescribeRestoreJobOutputTypeDef,
     DisassociateRecoveryPointFromParentInputRequestTypeDef,
     DisassociateRecoveryPointInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateInputRequestTypeDef,
-    ExportBackupPlanTemplateOutputTypeDef,
     FrameworkTypeDef,
     GetBackupPlanFromJSONInputRequestTypeDef,
     GetBackupPlanFromTemplateInputRequestTypeDef,
     GetBackupPlanInputRequestTypeDef,
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
-    GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
-    GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
-    GetRecoveryPointRestoreMetadataOutputTypeDef,
-    GetSupportedResourceTypesOutputTypeDef,
     LegalHoldTypeDef,
-    ListBackupJobsInputListBackupJobsPaginateTypeDef,
-    ListBackupJobsInputRequestTypeDef,
-    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
-    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
-    ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupPlansInputRequestTypeDef,
-    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
-    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputListCopyJobsPaginateTypeDef,
-    ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
-    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
     ListLegalHoldsInputRequestTypeDef,
-    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
-    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
-    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
-    ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
-    ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
-    ListTagsOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
-    ResponseMetadataTypeDef,
-    StartBackupJobOutputTypeDef,
-    StartCopyJobOutputTypeDef,
+    ReportSettingOutputTypeDef,
     StartReportJobInputRequestTypeDef,
-    StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
-    StartRestoreJobOutputTypeDef,
     StopBackupJobInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    UpdateFrameworkOutputTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateRegionSettingsInputRequestTypeDef,
-    UpdateReportPlanOutputTypeDef,
     BackupPlansListMemberTypeDef,
-    CreateBackupPlanOutputTypeDef,
-    UpdateBackupPlanOutputTypeDef,
     BackupJobTypeDef,
     CopyJobTypeDef,
-    DescribeBackupJobOutputTypeDef,
-    ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
-    ListBackupSelectionsOutputTypeDef,
-    ListBackupVaultsOutputTypeDef,
-    DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
-    UpdateRecoveryPointLifecycleOutputTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
+    CreateBackupPlanOutputTypeDef,
+    CreateBackupSelectionOutputTypeDef,
+    CreateBackupVaultOutputTypeDef,
+    CreateFrameworkOutputTypeDef,
+    CreateReportPlanOutputTypeDef,
+    DeleteBackupPlanOutputTypeDef,
+    DescribeBackupJobOutputTypeDef,
+    DescribeBackupVaultOutputTypeDef,
+    DescribeGlobalSettingsOutputTypeDef,
+    DescribeProtectedResourceOutputTypeDef,
+    DescribeRecoveryPointOutputTypeDef,
+    DescribeRegionSettingsOutputTypeDef,
+    DescribeRestoreJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportBackupPlanTemplateOutputTypeDef,
+    GetBackupVaultAccessPolicyOutputTypeDef,
+    GetBackupVaultNotificationsOutputTypeDef,
+    GetRecoveryPointRestoreMetadataOutputTypeDef,
+    GetSupportedResourceTypesOutputTypeDef,
+    ListBackupPlanTemplatesOutputTypeDef,
+    ListBackupSelectionsOutputTypeDef,
+    ListBackupVaultsOutputTypeDef,
+    ListTagsOutputTypeDef,
+    StartBackupJobOutputTypeDef,
+    StartCopyJobOutputTypeDef,
+    StartReportJobOutputTypeDef,
+    StartRestoreJobOutputTypeDef,
+    UpdateBackupPlanOutputTypeDef,
+    UpdateFrameworkOutputTypeDef,
+    UpdateRecoveryPointLifecycleOutputTypeDef,
+    UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
-    ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
-    RecoveryPointSelectionTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
+    DateRangeTypeDef,
+    ListBackupJobsInputRequestTypeDef,
+    ListCopyJobsInputRequestTypeDef,
+    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListReportJobsInputRequestTypeDef,
+    ListRestoreJobsInputRequestTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
+    ListBackupJobsInputListBackupJobsPaginateTypeDef,
+    ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
+    ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
+    ListBackupPlansInputListBackupPlansPaginateTypeDef,
+    ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
+    ListBackupVaultsInputListBackupVaultsPaginateTypeDef,
+    ListCopyJobsInputListCopyJobsPaginateTypeDef,
+    ListLegalHoldsInputListLegalHoldsPaginateTypeDef,
+    ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef,
+    ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef,
+    ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
+    ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
+    ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
     ReportJobTypeDef,
+    ReportPlanTypeDef,
+    ReportSettingUnionTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
-    CreateFrameworkInputRequestTypeDef,
     DescribeFrameworkOutputTypeDef,
-    UpdateFrameworkInputRequestTypeDef,
-    DescribeReportPlanOutputTypeDef,
-    ListReportPlansOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
+    FrameworkControlUnionTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
+    RecoveryPointSelectionTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
+    DescribeReportPlanOutputTypeDef,
+    ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
-    CreateBackupSelectionInputRequestTypeDef,
     GetBackupSelectionOutputTypeDef,
+    BackupSelectionUnionTypeDef,
+    CreateBackupSelectionInputRequestTypeDef,
+    CreateFrameworkInputRequestTypeDef,
+    UpdateFrameworkInputRequestTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingTypeDef:
+def get_value() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backup-2.5.2/types_aiobotocore_backup.egg-info/SOURCES.txt` & `types-aiobotocore-backup-2.5.2.post1/types_aiobotocore_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*


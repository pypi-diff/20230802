# Comparing `tmp/types-aiobotocore-ssm-2.5.2.tar.gz` & `tmp/types-aiobotocore-ssm-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-2.5.2.tar", last modified: Sat Jul  8 01:44:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
```

## Comparing `types-aiobotocore-ssm-2.5.2.tar` & `types-aiobotocore-ssm-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.618945 types-aiobotocore-ssm-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-08 01:44:22.614945 types-aiobotocore-ssm-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45445 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:22.618945 types-aiobotocore-ssm-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:22.000000 types-aiobotocore-ssm-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.610945 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136641 2023-07-08 01:41:24.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   136446 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28097 2023-07-08 01:41:27.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-07-08 01:41:24.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    61515 2023-07-08 01:41:24.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    61466 2023-07-08 01:41:24.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   204499 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   204271 2023-07-08 01:41:29.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:23.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-08 01:41:24.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-08 01:41:24.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.614945 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:22.000000 types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.073449 types-aiobotocore-ssm-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48263 2023-08-02 14:53:04.069448 types-aiobotocore-ssm-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46761 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.073449 types-aiobotocore-ssm-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.065448 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136861 2023-08-02 14:50:04.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136666 2023-08-02 14:50:01.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28097 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    61436 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61387 2023-08-02 14:50:04.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   215372 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215130 2023-08-02 14:50:07.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:00.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-02 14:50:05.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.069448 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48263 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-2.5.2/LICENSE` & `types-aiobotocore-ssm-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/PKG-INFO` & `types-aiobotocore-ssm-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-ssm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ssm type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-ssm"></a>
 
 # types-aiobotocore-ssm
 
 [![PyPI - types-aiobotocore-ssm](https://img.shields.io/pypi/v/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [types-aiobotocore-ssm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +42,15 @@
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
@@ -639,306 +606,311 @@
 )
 
 
 def check_value(value: AssociationComplianceSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ssm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
-    AssociationStatusTypeDef,
-    TargetTypeDef,
+    AssociationStatusOutputTypeDef,
+    TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    TimestampTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
+    BlobTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
-    NotificationConfigTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    NotificationConfigOutputTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
-    CreateActivationResultTypeDef,
+    TargetTypeDef,
     DocumentRequiresTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
-    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
-    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
-    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
-    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
-    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
-    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
-    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
     LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
-    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
-    MaintenanceWindowLambdaParametersTypeDef,
+    MaintenanceWindowLambdaParametersOutputTypeDef,
+    NotificationConfigTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
-    PaginatorConfigTypeDef,
     ParameterInlinePolicyTypeDef,
+    PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
-    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
-    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
-    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
-    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
+    CreateActivationResultTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
+    CreateOpsItemResponseTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
+    DeleteParametersResultTypeDef,
+    DeletePatchBaselineResultTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesResultTypeDef,
+    GetCalendarStateResponseTypeDef,
+    GetConnectionStatusResponseTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
+    GetMaintenanceWindowResultTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListInventoryEntriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
+    ResumeSessionResponseTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
+    StartSessionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
+    UnlabelParameterVersionResultTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     AssociationTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
+    AssociationStatusTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     UpdateDocumentRequestRequestTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
+    MaintenanceWindowLambdaParametersTypeDef,
     GetCommandInvocationResultTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
-    MaintenanceWindowRunCommandParametersTypeDef,
+    MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
-    PutComplianceItemsRequestRequestTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
+    TargetUnionTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
     GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeActivationsRequestRequestTypeDef,
+    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
-    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
-    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
     DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef,
     DescribePatchBaselinesRequestRequestTypeDef,
     DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef,
     DescribePatchGroupsRequestRequestTypeDef,
     DescribeAvailablePatchesResultTypeDef,
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef,
@@ -990,14 +962,15 @@
     GetInventoryRequestRequestTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
+    PatchSourceUnionTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
@@ -1007,39 +980,56 @@
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
+    MaintenanceWindowRunCommandParametersTypeDef,
+    NotificationConfigUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     OpsEntityTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
+    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
-    SendCommandRequestRequestTypeDef,
+    TargetLocationOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
+    AssociationStatusUnionTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
+    PutComplianceItemsRequestRequestTypeDef,
     ListCommandInvocationsResultTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
+    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
+    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    SendCommandRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     ListDocumentsResultTypeDef,
     DescribeOpsItemsResponseTypeDef,
     GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -1049,74 +1039,85 @@
     InventoryAggregatorTypeDef,
     DescribeInstanceInformationResultTypeDef,
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
+    PatchRuleOutputTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchRuleTypeDef,
-    ResourceDataSyncSourceTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
+    ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
+    RunbookOutputTypeDef,
+    StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
-    CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
-    StartAutomationExecutionRequestRequestTypeDef,
-    StepExecutionTypeDef,
-    UpdateAssociationRequestRequestTypeDef,
+    TargetLocationUnionTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
-    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
-    ResourceDataSyncItemTypeDef,
     CreateAssociationResultTypeDef,
     DescribeAssociationResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
+    RunbookUnionTypeDef,
+    CreateAssociationRequestRequestTypeDef,
+    StartAutomationExecutionRequestRequestTypeDef,
+    UpdateAssociationRequestRequestTypeDef,
+    GetPatchBaselineResultTypeDef,
+    UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
-    GetPatchBaselineResultTypeDef,
+    PatchRuleGroupUnionTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
-    UpdatePatchBaselineResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSharingInfoTypeDef:
+def get_value() -> AccountSharingInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ssm-2.5.2/README.md` & `types-aiobotocore-ssm-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ssm
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ssm type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-ssm"></a>
 
 # types-aiobotocore-ssm
 
 [![PyPI - types-aiobotocore-ssm](https://img.shields.io/pypi/v/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [types-aiobotocore-ssm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -606,306 +638,311 @@
 )
 
 
 def check_value(value: AssociationComplianceSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ssm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
-    AssociationStatusTypeDef,
-    TargetTypeDef,
+    AssociationStatusOutputTypeDef,
+    TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    TimestampTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
+    BlobTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
-    NotificationConfigTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    NotificationConfigOutputTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
-    CreateActivationResultTypeDef,
+    TargetTypeDef,
     DocumentRequiresTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
-    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
-    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
-    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
-    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
-    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
-    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
-    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
     LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
-    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
-    MaintenanceWindowLambdaParametersTypeDef,
+    MaintenanceWindowLambdaParametersOutputTypeDef,
+    NotificationConfigTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
-    PaginatorConfigTypeDef,
     ParameterInlinePolicyTypeDef,
+    PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
-    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
-    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
-    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
-    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
+    CreateActivationResultTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
+    CreateOpsItemResponseTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
+    DeleteParametersResultTypeDef,
+    DeletePatchBaselineResultTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesResultTypeDef,
+    GetCalendarStateResponseTypeDef,
+    GetConnectionStatusResponseTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
+    GetMaintenanceWindowResultTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListInventoryEntriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
+    ResumeSessionResponseTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
+    StartSessionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
+    UnlabelParameterVersionResultTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     AssociationTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
+    AssociationStatusTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     UpdateDocumentRequestRequestTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
+    MaintenanceWindowLambdaParametersTypeDef,
     GetCommandInvocationResultTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
-    MaintenanceWindowRunCommandParametersTypeDef,
+    MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
-    PutComplianceItemsRequestRequestTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
+    TargetUnionTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
     GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeActivationsRequestRequestTypeDef,
+    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
-    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
-    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
     DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef,
     DescribePatchBaselinesRequestRequestTypeDef,
     DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef,
     DescribePatchGroupsRequestRequestTypeDef,
     DescribeAvailablePatchesResultTypeDef,
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef,
@@ -957,14 +994,15 @@
     GetInventoryRequestRequestTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
+    PatchSourceUnionTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
@@ -974,39 +1012,56 @@
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
+    MaintenanceWindowRunCommandParametersTypeDef,
+    NotificationConfigUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     OpsEntityTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
+    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
-    SendCommandRequestRequestTypeDef,
+    TargetLocationOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
+    AssociationStatusUnionTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
+    PutComplianceItemsRequestRequestTypeDef,
     ListCommandInvocationsResultTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
+    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
+    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    SendCommandRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     ListDocumentsResultTypeDef,
     DescribeOpsItemsResponseTypeDef,
     GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -1016,74 +1071,85 @@
     InventoryAggregatorTypeDef,
     DescribeInstanceInformationResultTypeDef,
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
+    PatchRuleOutputTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchRuleTypeDef,
-    ResourceDataSyncSourceTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
+    ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
+    RunbookOutputTypeDef,
+    StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
-    CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
-    StartAutomationExecutionRequestRequestTypeDef,
-    StepExecutionTypeDef,
-    UpdateAssociationRequestRequestTypeDef,
+    TargetLocationUnionTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
-    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
-    ResourceDataSyncItemTypeDef,
     CreateAssociationResultTypeDef,
     DescribeAssociationResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
+    RunbookUnionTypeDef,
+    CreateAssociationRequestRequestTypeDef,
+    StartAutomationExecutionRequestRequestTypeDef,
+    UpdateAssociationRequestRequestTypeDef,
+    GetPatchBaselineResultTypeDef,
+    UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
-    GetPatchBaselineResultTypeDef,
+    PatchRuleGroupUnionTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
-    UpdatePatchBaselineResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSharingInfoTypeDef:
+def get_value() -> AccountSharingInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ssm-2.5.2/setup.py` & `types-aiobotocore-ssm-2.5.2.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore ssm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ssm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ssm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/__init__.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/__init__.pyi` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/__main__.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSM 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SSM 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/client.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("ssm") as client:
         client: SSMClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationSyncComplianceType,
@@ -92,31 +91,31 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusTypeDef,
+    AssociationStatusUnionTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
-    CreateAssociationBatchRequestEntryTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
     CreatePatchBaselineResultTypeDef,
@@ -211,58 +210,59 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     MetadataValueTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigUnionTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
-    PatchFilterGroupTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchOrchestratorFilterTypeDef,
-    PatchRuleGroupTypeDef,
-    PatchSourceTypeDef,
+    PatchRuleGroupUnionTypeDef,
+    PatchSourceUnionTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
     RegisterTaskWithMaintenanceWindowResultTypeDef,
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
-    RunbookTypeDef,
+    RunbookUnionTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
-    TargetLocationTypeDef,
-    TargetTypeDef,
+    TargetLocationUnionTypeDef,
+    TargetUnionTypeDef,
     TerminateSessionResponseTypeDef,
+    TimestampTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
     UpdateMaintenanceWindowResultTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
@@ -273,26 +273,23 @@
 from .waiter import CommandExecutedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SSMClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     AssociatedInstances: Type[BotocoreClientError]
     AssociationAlreadyExists: Type[BotocoreClientError]
     AssociationDoesNotExist: Type[BotocoreClientError]
     AssociationExecutionDoesNotExist: Type[BotocoreClientError]
     AssociationLimitExceeded: Type[BotocoreClientError]
@@ -416,15 +413,14 @@
     UnsupportedFeatureRequiredException: Type[BotocoreClientError]
     UnsupportedInventoryItemContextException: Type[BotocoreClientError]
     UnsupportedInventorySchemaVersionException: Type[BotocoreClientError]
     UnsupportedOperatingSystem: Type[BotocoreClientError]
     UnsupportedParameterType: Type[BotocoreClientError]
     UnsupportedPlatformType: Type[BotocoreClientError]
 
-
 class SSMClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
     """
 
     meta: ClientMeta
@@ -433,139 +429,129 @@
     def exceptions(self) -> Exceptions:
         """
         SSMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#exceptions)
         """
-
     async def add_tags_to_resource(
         self,
         *,
         ResourceType: ResourceTypeForTaggingType,
         ResourceId: str,
         Tags: Sequence[TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds or overwrites one or more tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.add_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#add_tags_to_resource)
         """
-
     async def associate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationType: str, ResourceType: str, ResourceUri: str
     ) -> AssociateOpsItemRelatedItemResponseTypeDef:
         """
         Associates a related item to a Systems Manager OpsCenter OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.associate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#associate_ops_item_related_item)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#can_paginate)
         """
-
     async def cancel_command(
         self, *, CommandId: str, InstanceIds: Sequence[str] = ...
     ) -> Dict[str, Any]:
         """
         Attempts to cancel the command specified by the Command ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_command)
         """
-
     async def cancel_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> CancelMaintenanceWindowExecutionResultTypeDef:
         """
         Stops a maintenance window execution that is already in progress and cancels any
         tasks in the window that haven't already starting running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_maintenance_window_execution)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#close)
         """
-
     async def create_activation(
         self,
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
-        ExpirationDate: Union[datetime, str] = ...,
+        ExpirationDate: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...
     ) -> CreateActivationResultTypeDef:
         """
         Generates an activation code and activation ID you can use to register your on-
         premises servers, edge devices, or virtual machine (VM) with Amazon Web Services
         Systems Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_activation)
         """
-
     async def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association)
         """
-
     async def create_association_batch(
-        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryTypeDef]
+        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association_batch)
         """
-
     async def create_document(
         self,
         *,
         Content: str,
         Name: str,
         Requires: Sequence[DocumentRequiresTypeDef] = ...,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
@@ -578,15 +564,14 @@
     ) -> CreateDocumentResultTypeDef:
         """
         Creates a Amazon Web Services Systems Manager (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_document)
         """
-
     async def create_maintenance_window(
         self,
         *,
         Name: str,
         Schedule: str,
         Duration: int,
         Cutoff: int,
@@ -601,42 +586,40 @@
     ) -> CreateMaintenanceWindowResultTypeDef:
         """
         Creates a new maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_maintenance_window)
         """
-
     async def create_ops_item(
         self,
         *,
         Description: str,
         Source: str,
         Title: str,
         OpsItemType: str = ...,
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         AccountId: str = ...
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_item)
         """
-
     async def create_ops_metadata(
         self,
         *,
         ResourceId: str,
         Metadata: Mapping[str, MetadataValueTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateOpsMetadataResultTypeDef:
@@ -644,39 +627,37 @@
         If you create a new application in Application Manager, Amazon Web Services
         Systems Manager calls this API operation to specify information about the new
         application, including the application type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_metadata)
         """
-
     async def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_patch_baseline)
         """
-
     async def create_resource_data_sync(
         self,
         *,
         SyncName: str,
         S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,
         SyncType: str = ...,
         SyncSource: ResourceDataSyncSourceTypeDef = ...
@@ -684,45 +665,41 @@
         """
         A resource data sync helps you view data from multiple sources in a single
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_resource_data_sync)
         """
-
     async def delete_activation(self, *, ActivationId: str) -> Dict[str, Any]:
         """
         Deletes an activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_activation)
         """
-
     async def delete_association(
         self, *, Name: str = ..., InstanceId: str = ..., AssociationId: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociates the specified Amazon Web Services Systems Manager document (SSM
         document) from the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_association)
         """
-
     async def delete_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ..., Force: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the Amazon Web Services Systems Manager document (SSM document) and all
         managed node associations to the document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_document)
         """
-
     async def delete_inventory(
         self,
         *,
         TypeName: str,
         SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
@@ -730,115 +707,103 @@
         """
         Delete a custom inventory type or the data associated with a custom Inventory
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_inventory)
         """
-
     async def delete_maintenance_window(
         self, *, WindowId: str
     ) -> DeleteMaintenanceWindowResultTypeDef:
         """
         Deletes a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_maintenance_window)
         """
-
     async def delete_ops_metadata(self, *, OpsMetadataArn: str) -> Dict[str, Any]:
         """
         Delete OpsMetadata related to an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_ops_metadata)
         """
-
     async def delete_parameter(self, *, Name: str) -> Dict[str, Any]:
         """
         Delete a parameter from the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameter)
         """
-
     async def delete_parameters(self, *, Names: Sequence[str]) -> DeleteParametersResultTypeDef:
         """
         Delete a list of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameters)
         """
-
     async def delete_patch_baseline(self, *, BaselineId: str) -> DeletePatchBaselineResultTypeDef:
         """
         Deletes a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_patch_baseline)
         """
-
     async def delete_resource_data_sync(
         self, *, SyncName: str, SyncType: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a resource data sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_data_sync)
         """
-
     async def delete_resource_policy(
         self, *, ResourceArn: str, PolicyId: str, PolicyHash: str
     ) -> Dict[str, Any]:
         """
         Deletes a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_policy)
         """
-
     async def deregister_managed_instance(self, *, InstanceId: str) -> Dict[str, Any]:
         """
         Removes the server or virtual machine from the list of registered servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_managed_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_managed_instance)
         """
-
     async def deregister_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> DeregisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Removes a patch group from a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_patch_baseline_for_patch_group)
         """
-
     async def deregister_target_from_maintenance_window(
         self, *, WindowId: str, WindowTargetId: str, Safe: bool = ...
     ) -> DeregisterTargetFromMaintenanceWindowResultTypeDef:
         """
         Removes a target from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_target_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_target_from_maintenance_window)
         """
-
     async def deregister_task_from_maintenance_window(
         self, *, WindowId: str, WindowTaskId: str
     ) -> DeregisterTaskFromMaintenanceWindowResultTypeDef:
         """
         Removes a task from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_task_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_task_from_maintenance_window)
         """
-
     async def describe_activations(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeActivationsResultTypeDef:
@@ -847,30 +812,28 @@
         was created, its expiration date, the Identity and Access Management (IAM) role
         assigned to the managed nodes in the activation, and the number of nodes
         registered by using this activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_activations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_activations)
         """
-
     async def describe_association(
         self,
         *,
         Name: str = ...,
         InstanceId: str = ...,
         AssociationId: str = ...,
         AssociationVersion: str = ...
     ) -> DescribeAssociationResultTypeDef:
         """
         Describes the association for the specified target or managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association)
         """
-
     async def describe_association_execution_targets(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -878,44 +841,41 @@
     ) -> DescribeAssociationExecutionTargetsResultTypeDef:
         """
         Views information about a specific execution of a specific association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_execution_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_execution_targets)
         """
-
     async def describe_association_executions(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAssociationExecutionsResultTypeDef:
         """
         Views all executions for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_executions)
         """
-
     async def describe_automation_executions(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAutomationExecutionsResultTypeDef:
         """
         Provides details about all active and terminated Automation executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_executions)
         """
-
     async def describe_automation_step_executions(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
@@ -924,40 +884,37 @@
         """
         Information about all active and terminated step executions in an Automation
         workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_step_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_step_executions)
         """
-
     async def describe_available_patches(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAvailablePatchesResultTypeDef:
         """
         Lists all patches eligible to be included in a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_available_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_available_patches)
         """
-
     async def describe_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ...
     ) -> DescribeDocumentResultTypeDef:
         """
         Describes the specified Amazon Web Services Systems Manager document (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document)
         """
-
     async def describe_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         MaxResults: int = ...,
         NextToken: str = ...
@@ -965,46 +922,42 @@
         """
         Describes the permissions for a Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document_permission)
         """
-
     async def describe_effective_instance_associations(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectiveInstanceAssociationsResultTypeDef:
         """
         All associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_instance_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_instance_associations)
         """
-
     async def describe_effective_patches_for_patch_baseline(
         self, *, BaselineId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectivePatchesForPatchBaselineResultTypeDef:
         """
         Retrieves the current effective patches (the patch and the approval state) for
         the specified patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_patches_for_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_patches_for_patch_baseline)
         """
-
     async def describe_instance_associations_status(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeInstanceAssociationsStatusResultTypeDef:
         """
         The status of the associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_associations_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_associations_status)
         """
-
     async def describe_instance_information(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1013,25 +966,23 @@
         Describes one or more of your managed nodes, including information about the
         operating system platform, the version of SSM Agent installed on the managed
         node, node status, and so on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_information)
         """
-
     async def describe_instance_patch_states(
         self, *, InstanceIds: Sequence[str], NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInstancePatchStatesResultTypeDef:
         """
         Retrieves the high-level patch state of one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states)
         """
-
     async def describe_instance_patch_states_for_patch_group(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -1039,15 +990,14 @@
         """
         Retrieves the high-level patch state for the managed nodes in the specified
         patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states_for_patch_group)
         """
-
     async def describe_instance_patches(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -1055,25 +1005,23 @@
         """
         Retrieves information about the patches on the specified managed node and their
         state relative to the patch baseline being used for the node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patches)
         """
-
     async def describe_inventory_deletions(
         self, *, DeletionId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInventoryDeletionsResultTypeDef:
         """
         Describes a specific delete inventory operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_inventory_deletions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_inventory_deletions)
         """
-
     async def describe_maintenance_window_execution_task_invocations(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -1082,190 +1030,177 @@
         """
         Retrieves the individual task executions (one per target) for a particular task
         run as part of a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_task_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_task_invocations)
         """
-
     async def describe_maintenance_window_execution_tasks(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
         """
         For a given maintenance window execution, lists the tasks that were run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_tasks)
         """
-
     async def describe_maintenance_window_executions(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionsResultTypeDef:
         """
         Lists the executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_executions)
         """
-
     async def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_schedule)
         """
-
     async def describe_maintenance_window_targets(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTargetsResultTypeDef:
         """
         Lists the targets registered with the maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_targets)
         """
-
     async def describe_maintenance_window_tasks(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTasksResultTypeDef:
         """
         Lists the tasks in a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_tasks)
         """
-
     async def describe_maintenance_windows(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsResultTypeDef:
         """
         Retrieves the maintenance windows in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows)
         """
-
     async def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows_for_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows_for_target)
         """
-
     async def describe_ops_items(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeOpsItemsResponseTypeDef:
         """
         Query a set of OpsItems.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_ops_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_ops_items)
         """
-
     async def describe_parameters(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeParametersResultTypeDef:
         """
         Get information about a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_parameters)
         """
-
     async def describe_patch_baselines(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribePatchBaselinesResultTypeDef:
         """
         Lists the patch baselines in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_baselines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_baselines)
         """
-
     async def describe_patch_group_state(
         self, *, PatchGroup: str
     ) -> DescribePatchGroupStateResultTypeDef:
         """
         Returns high-level aggregated patch compliance state information for a patch
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_group_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_group_state)
         """
-
     async def describe_patch_groups(
         self,
         *,
         MaxResults: int = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...
     ) -> DescribePatchGroupsResultTypeDef:
         """
         Lists all patch groups that have been registered with patch baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_groups)
         """
-
     async def describe_patch_properties(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
         MaxResults: int = ...,
@@ -1274,15 +1209,14 @@
         """
         Lists the properties of available patches organized by product, product family,
         classification, severity, and other properties of available patches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_properties)
         """
-
     async def describe_sessions(
         self,
         *,
         State: SessionStateType,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[SessionFilterTypeDef] = ...
@@ -1290,100 +1224,91 @@
         """
         Retrieves a list of all active sessions (both connected and disconnected) or
         terminated sessions from the past 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_sessions)
         """
-
     async def disassociate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationId: str
     ) -> Dict[str, Any]:
         """
         Deletes the association between an OpsItem and a related item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.disassociate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#disassociate_ops_item_related_item)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#generate_presigned_url)
         """
-
     async def get_automation_execution(
         self, *, AutomationExecutionId: str
     ) -> GetAutomationExecutionResultTypeDef:
         """
         Get detailed information about a particular Automation execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_automation_execution)
         """
-
     async def get_calendar_state(
         self, *, CalendarNames: Sequence[str], AtTime: str = ...
     ) -> GetCalendarStateResponseTypeDef:
         """
         Gets the state of a Amazon Web Services Systems Manager change calendar at the
         current time or a specified time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_calendar_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_calendar_state)
         """
-
     async def get_command_invocation(
         self, *, CommandId: str, InstanceId: str, PluginName: str = ...
     ) -> GetCommandInvocationResultTypeDef:
         """
         Returns detailed information about command execution for an invocation or
         plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_command_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_command_invocation)
         """
-
     async def get_connection_status(self, *, Target: str) -> GetConnectionStatusResponseTypeDef:
         """
         Retrieves the Session Manager connection status for a managed node to determine
         whether it is running and ready to receive Session Manager connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_connection_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_connection_status)
         """
-
     async def get_default_patch_baseline(
         self, *, OperatingSystem: OperatingSystemType = ...
     ) -> GetDefaultPatchBaselineResultTypeDef:
         """
         Retrieves the default patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_default_patch_baseline)
         """
-
     async def get_deployable_patch_snapshot_for_instance(
         self, *, InstanceId: str, SnapshotId: str, BaselineOverride: BaselineOverrideTypeDef = ...
     ) -> GetDeployablePatchSnapshotForInstanceResultTypeDef:
         """
         Retrieves the current snapshot for the patch baseline the managed node uses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_deployable_patch_snapshot_for_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_deployable_patch_snapshot_for_instance)
         """
-
     async def get_document(
         self,
         *,
         Name: str,
         VersionName: str = ...,
         DocumentVersion: str = ...,
         DocumentFormat: DocumentFormatType = ...
@@ -1391,15 +1316,14 @@
         """
         Gets the contents of the specified Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_document)
         """
-
     async def get_inventory(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
         NextToken: str = ...,
@@ -1407,15 +1331,14 @@
     ) -> GetInventoryResultTypeDef:
         """
         Query inventory information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory)
         """
-
     async def get_inventory_schema(
         self,
         *,
         TypeName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Aggregator: bool = ...,
@@ -1424,84 +1347,76 @@
         """
         Return a list of inventory type names for the account, or return a list of
         attribute names for a specific Inventory item type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory_schema)
         """
-
     async def get_maintenance_window(self, *, WindowId: str) -> GetMaintenanceWindowResultTypeDef:
         """
         Retrieves a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window)
         """
-
     async def get_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> GetMaintenanceWindowExecutionResultTypeDef:
         """
         Retrieves details about a specific a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution)
         """
-
     async def get_maintenance_window_execution_task(
         self, *, WindowExecutionId: str, TaskId: str
     ) -> GetMaintenanceWindowExecutionTaskResultTypeDef:
         """
         Retrieves the details about a specific task run as part of a maintenance window
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task)
         """
-
     async def get_maintenance_window_execution_task_invocation(
         self, *, WindowExecutionId: str, TaskId: str, InvocationId: str
     ) -> GetMaintenanceWindowExecutionTaskInvocationResultTypeDef:
         """
         Retrieves information about a specific task running on a specific target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task_invocation)
         """
-
     async def get_maintenance_window_task(
         self, *, WindowId: str, WindowTaskId: str
     ) -> GetMaintenanceWindowTaskResultTypeDef:
         """
         Retrieves the details of a maintenance window task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_task)
         """
-
     async def get_ops_item(
         self, *, OpsItemId: str, OpsItemArn: str = ...
     ) -> GetOpsItemResponseTypeDef:
         """
         Get information about an OpsItem by using the ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_item)
         """
-
     async def get_ops_metadata(
         self, *, OpsMetadataArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetOpsMetadataResultTypeDef:
         """
         View operational metadata related to an application in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_metadata)
         """
-
     async def get_ops_summary(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
@@ -1511,46 +1426,42 @@
         """
         View a summary of operations metadata (OpsData) based on specified filters and
         aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_summary)
         """
-
     async def get_parameter(
         self, *, Name: str, WithDecryption: bool = ...
     ) -> GetParameterResultTypeDef:
         """
         Get information about a single parameter by specifying the parameter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter)
         """
-
     async def get_parameter_history(
         self, *, Name: str, WithDecryption: bool = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> GetParameterHistoryResultTypeDef:
         """
         Retrieves the history of all changes to a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter_history)
         """
-
     async def get_parameters(
         self, *, Names: Sequence[str], WithDecryption: bool = ...
     ) -> GetParametersResultTypeDef:
         """
         Get information about one or more parameters by specifying multiple parameter
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters)
         """
-
     async def get_parameters_by_path(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
@@ -1559,87 +1470,79 @@
     ) -> GetParametersByPathResultTypeDef:
         """
         Retrieve information about one or more parameters in a specific hierarchy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters_by_path)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters_by_path)
         """
-
     async def get_patch_baseline(self, *, BaselineId: str) -> GetPatchBaselineResultTypeDef:
         """
         Retrieves information about a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline)
         """
-
     async def get_patch_baseline_for_patch_group(
         self, *, PatchGroup: str, OperatingSystem: OperatingSystemType = ...
     ) -> GetPatchBaselineForPatchGroupResultTypeDef:
         """
         Retrieves the patch baseline that should be used for the specified patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline_for_patch_group)
         """
-
     async def get_resource_policies(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetResourcePoliciesResponseTypeDef:
         """
         Returns an array of the `Policy` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_resource_policies)
         """
-
     async def get_service_setting(self, *, SettingId: str) -> GetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_service_setting)
         """
-
     async def label_parameter_version(
         self, *, Name: str, Labels: Sequence[str], ParameterVersion: int = ...
     ) -> LabelParameterVersionResultTypeDef:
         """
         A parameter label is a user-defined alias to help you manage different versions
         of a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.label_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#label_parameter_version)
         """
-
     async def list_association_versions(
         self, *, AssociationId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAssociationVersionsResultTypeDef:
         """
         Retrieves all versions of an association for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_association_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_association_versions)
         """
-
     async def list_associations(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListAssociationsResultTypeDef:
         """
         Returns all State Manager associations in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_associations)
         """
-
     async def list_command_invocations(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1648,15 +1551,14 @@
     ) -> ListCommandInvocationsResultTypeDef:
         """
         An invocation is copy of a command sent to a specific managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_command_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_command_invocations)
         """
-
     async def list_commands(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1664,15 +1566,14 @@
     ) -> ListCommandsResultTypeDef:
         """
         Lists the commands requested by users of the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_commands)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_commands)
         """
-
     async def list_compliance_items(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
@@ -1681,30 +1582,28 @@
         """
         For a specified resource ID, this API operation returns a list of compliance
         statuses for different resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_items)
         """
-
     async def list_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListComplianceSummariesResultTypeDef:
         """
         Returns a summary count of compliant and non-compliant resources for a
         compliance type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_summaries)
         """
-
     async def list_document_metadata_history(
         self,
         *,
         Name: str,
         Metadata: Literal["DocumentReviews"],
         DocumentVersion: str = ...,
         NextToken: str = ...,
@@ -1713,25 +1612,23 @@
         """
         Information about approval reviews for a version of a change template in Change
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_metadata_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_metadata_history)
         """
-
     async def list_document_versions(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListDocumentVersionsResultTypeDef:
         """
         List all versions for a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_versions)
         """
-
     async def list_documents(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1739,15 +1636,14 @@
         """
         Returns all Systems Manager (SSM) documents in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_documents)
         """
-
     async def list_inventory_entries(
         self,
         *,
         InstanceId: str,
         TypeName: str,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         NextToken: str = ...,
@@ -1755,30 +1651,28 @@
     ) -> ListInventoryEntriesResultTypeDef:
         """
         A list of inventory items returned by the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_inventory_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_inventory_entries)
         """
-
     async def list_ops_item_events(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsItemEventsResponseTypeDef:
         """
         Returns a list of all OpsItem events in the current Amazon Web Services Region
         and Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_events)
         """
-
     async def list_ops_item_related_items(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1786,64 +1680,59 @@
         """
         Lists all related-item resources associated with a Systems Manager OpsCenter
         OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_related_items)
         """
-
     async def list_ops_metadata(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when displaying all
         Application Manager OpsMetadata objects or blobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_metadata)
         """
-
     async def list_resource_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListResourceComplianceSummariesResultTypeDef:
         """
         Returns a resource-level summary count.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_compliance_summaries)
         """
-
     async def list_resource_data_sync(
         self, *, SyncType: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListResourceDataSyncResultTypeDef:
         """
         Lists your resource data sync configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_data_sync)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str
     ) -> ListTagsForResourceResultTypeDef:
         """
         Returns a list of the tags assigned to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_tags_for_resource)
         """
-
     async def modify_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         AccountIdsToAdd: Sequence[str] = ...,
         AccountIdsToRemove: Sequence[str] = ...,
@@ -1852,44 +1741,41 @@
         """
         Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
         privately.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.modify_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#modify_document_permission)
         """
-
     async def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: ComplianceExecutionSummaryTypeDef,
+        ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_compliance_items)
         """
-
     async def put_inventory(
         self, *, InstanceId: str, Items: Sequence[InventoryItemTypeDef]
     ) -> PutInventoryResultTypeDef:
         """
         Bulk update custom inventory items on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_inventory)
         """
-
     async def put_parameter(
         self,
         *,
         Name: str,
         Value: str,
         Description: str = ...,
         Type: ParameterTypeType = ...,
@@ -1903,214 +1789,202 @@
     ) -> PutParameterResultTypeDef:
         """
         Add a parameter to the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_parameter)
         """
-
     async def put_resource_policy(
         self, *, ResourceArn: str, Policy: str, PolicyId: str = ..., PolicyHash: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates or updates a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_resource_policy)
         """
-
     async def register_default_patch_baseline(
         self, *, BaselineId: str
     ) -> RegisterDefaultPatchBaselineResultTypeDef:
         """
         Defines the default patch baseline for the relevant operating system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_default_patch_baseline)
         """
-
     async def register_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> RegisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Registers a patch baseline for a patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_patch_baseline_for_patch_group)
         """
-
     async def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[TargetUnionTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_target_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_target_with_maintenance_window)
         """
-
     async def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
+        ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_task_with_maintenance_window)
         """
-
     async def remove_tags_from_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str, TagKeys: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Removes tag keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.remove_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#remove_tags_from_resource)
         """
-
     async def reset_service_setting(self, *, SettingId: str) -> ResetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.reset_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#reset_service_setting)
         """
-
     async def resume_session(self, *, SessionId: str) -> ResumeSessionResponseTypeDef:
         """
         Reconnects a session to a managed node after it has been disconnected.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.resume_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#resume_session)
         """
-
     async def send_automation_signal(
         self,
         *,
         AutomationExecutionId: str,
         SignalType: SignalTypeType,
         Payload: Mapping[str, Sequence[str]] = ...
     ) -> Dict[str, Any]:
         """
         Sends a signal to an Automation execution to change the current behavior or
         status of the execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_automation_signal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_automation_signal)
         """
-
     async def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: NotificationConfigTypeDef = ...,
+        NotificationConfig: NotificationConfigUnionTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_command)
         """
-
     async def start_associations_once(self, *, AssociationIds: Sequence[str]) -> Dict[str, Any]:
         """
         Runs an association immediately and only one time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_associations_once)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_associations_once)
         """
-
     async def start_automation_execution(
         self,
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_automation_execution)
         """
-
     async def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[RunbookTypeDef],
-        ScheduledTime: Union[datetime, str] = ...,
+        Runbooks: Sequence[RunbookUnionTypeDef],
+        ScheduledTime: TimestampTypeDef = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ScheduledEndTime: Union[datetime, str] = ...,
+        ScheduledEndTime: TimestampTypeDef = ...,
         ChangeDetails: str = ...
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_change_request_execution)
         """
-
     async def start_session(
         self,
         *,
         Target: str,
         DocumentName: str = ...,
         Reason: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...
@@ -2118,86 +1992,80 @@
         """
         Initiates a connection to a target (for example, a managed node) for a Session
         Manager session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_session)
         """
-
     async def stop_automation_execution(
         self, *, AutomationExecutionId: str, Type: StopTypeType = ...
     ) -> Dict[str, Any]:
         """
         Stop an Automation that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.stop_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#stop_automation_execution)
         """
-
     async def terminate_session(self, *, SessionId: str) -> TerminateSessionResponseTypeDef:
         """
         Permanently ends a session and closes the data connection between the Session
         Manager client and SSM Agent on the managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.terminate_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#terminate_session)
         """
-
     async def unlabel_parameter_version(
         self, *, Name: str, ParameterVersion: int, Labels: Sequence[str]
     ) -> UnlabelParameterVersionResultTypeDef:
         """
         Remove a label or labels from a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.unlabel_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#unlabel_parameter_version)
         """
-
     async def update_association(
         self,
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association)
         """
-
     async def update_association_status(
-        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusTypeDef
+        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusUnionTypeDef
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association_status)
         """
-
     async def update_document(
         self,
         *,
         Content: str,
         Name: str,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
@@ -2208,36 +2076,33 @@
     ) -> UpdateDocumentResultTypeDef:
         """
         Updates one or more values for an SSM document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document)
         """
-
     async def update_document_default_version(
         self, *, Name: str, DocumentVersion: str
     ) -> UpdateDocumentDefaultVersionResultTypeDef:
         """
         Set the default version of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_default_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_default_version)
         """
-
     async def update_document_metadata(
         self, *, Name: str, DocumentReviews: DocumentReviewsTypeDef, DocumentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates information related to approval reviews for a specific version of a
         change template in Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_metadata)
         """
-
     async def update_maintenance_window(
         self,
         *,
         WindowId: str,
         Name: str = ...,
         Description: str = ...,
         StartDate: str = ...,
@@ -2253,579 +2118,523 @@
     ) -> UpdateMaintenanceWindowResultTypeDef:
         """
         Updates an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window)
         """
-
     async def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_target)
         """
-
     async def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
+        ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_task)
         """
-
     async def update_managed_instance_role(
         self, *, InstanceId: str, IamRole: str
     ) -> Dict[str, Any]:
         """
         Changes the Identity and Access Management (IAM) role that is assigned to the
         on-premises server, edge device, or virtual machines (VM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_managed_instance_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_managed_instance_role)
         """
-
     async def update_ops_item(
         self,
         *,
         OpsItemId: str,
         Description: str = ...,
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         OperationalDataToDelete: Sequence[str] = ...,
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Status: OpsItemStatusType = ...,
         Title: str = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         OpsItemArn: str = ...
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_item)
         """
-
     async def update_ops_metadata(
         self,
         *,
         OpsMetadataArn: str,
         MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,
         KeysToDelete: Sequence[str] = ...
     ) -> UpdateOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when you edit
         OpsMetadata in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_metadata)
         """
-
     async def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_patch_baseline)
         """
-
     async def update_resource_data_sync(
         self, *, SyncName: str, SyncType: str, SyncSource: ResourceDataSyncSourceTypeDef
     ) -> Dict[str, Any]:
         """
         Update a resource data sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_resource_data_sync)
         """
-
     async def update_service_setting(self, *, SettingId: str, SettingValue: str) -> Dict[str, Any]:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_service_setting)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_activations"]
     ) -> DescribeActivationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_execution_targets"]
     ) -> DescribeAssociationExecutionTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_executions"]
     ) -> DescribeAssociationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_executions"]
     ) -> DescribeAutomationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_step_executions"]
     ) -> DescribeAutomationStepExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_available_patches"]
     ) -> DescribeAvailablePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_instance_associations"]
     ) -> DescribeEffectiveInstanceAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_patches_for_patch_baseline"]
     ) -> DescribeEffectivePatchesForPatchBaselinePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_associations_status"]
     ) -> DescribeInstanceAssociationsStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_information"]
     ) -> DescribeInstanceInformationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states"]
     ) -> DescribeInstancePatchStatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states_for_patch_group"]
     ) -> DescribeInstancePatchStatesForPatchGroupPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patches"]
     ) -> DescribeInstancePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_inventory_deletions"]
     ) -> DescribeInventoryDeletionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_task_invocations"]
     ) -> DescribeMaintenanceWindowExecutionTaskInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_tasks"]
     ) -> DescribeMaintenanceWindowExecutionTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_executions"]
     ) -> DescribeMaintenanceWindowExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_schedule"]
     ) -> DescribeMaintenanceWindowSchedulePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_targets"]
     ) -> DescribeMaintenanceWindowTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_tasks"]
     ) -> DescribeMaintenanceWindowTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows"]
     ) -> DescribeMaintenanceWindowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows_for_target"]
     ) -> DescribeMaintenanceWindowsForTargetPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_ops_items"]
     ) -> DescribeOpsItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_parameters"]
     ) -> DescribeParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_baselines"]
     ) -> DescribePatchBaselinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_groups"]
     ) -> DescribePatchGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_properties"]
     ) -> DescribePatchPropertiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_sessions"]
     ) -> DescribeSessionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_inventory"]) -> GetInventoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_inventory_schema"]
     ) -> GetInventorySchemaPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_ops_summary"]) -> GetOpsSummaryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameter_history"]
     ) -> GetParameterHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameters_by_path"]
     ) -> GetParametersByPathPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_association_versions"]
     ) -> ListAssociationVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_associations"]
     ) -> ListAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_command_invocations"]
     ) -> ListCommandInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_commands"]) -> ListCommandsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_items"]
     ) -> ListComplianceItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_summaries"]
     ) -> ListComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_versions"]
     ) -> ListDocumentVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_documents"]) -> ListDocumentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_events"]
     ) -> ListOpsItemEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_related_items"]
     ) -> ListOpsItemRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_metadata"]
     ) -> ListOpsMetadataPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_compliance_summaries"]
     ) -> ListResourceComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_data_sync"]
     ) -> ListResourceDataSyncPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
-
     def get_waiter(self, waiter_name: Literal["command_executed"]) -> CommandExecutedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "SSMClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/client.pyi` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("ssm") as client:
         client: SSMClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationSyncComplianceType,
@@ -92,31 +91,31 @@
     ListOpsItemEventsPaginator,
     ListOpsItemRelatedItemsPaginator,
     ListOpsMetadataPaginator,
     ListResourceComplianceSummariesPaginator,
     ListResourceDataSyncPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
     AssociateOpsItemRelatedItemResponseTypeDef,
     AssociationExecutionFilterTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
-    AssociationStatusTypeDef,
+    AssociationStatusUnionTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     BaselineOverrideTypeDef,
     CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     CreateActivationResultTypeDef,
-    CreateAssociationBatchRequestEntryTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
     CreateAssociationBatchResultTypeDef,
     CreateAssociationResultTypeDef,
     CreateDocumentResultTypeDef,
     CreateMaintenanceWindowResultTypeDef,
     CreateOpsItemResponseTypeDef,
     CreateOpsMetadataResultTypeDef,
     CreatePatchBaselineResultTypeDef,
@@ -211,58 +210,59 @@
     ListOpsItemRelatedItemsResponseTypeDef,
     ListOpsMetadataResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     ListTagsForResourceResultTypeDef,
     LoggingInfoTypeDef,
     MaintenanceWindowFilterTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     MetadataValueTypeDef,
-    NotificationConfigTypeDef,
+    NotificationConfigUnionTypeDef,
     OpsAggregatorTypeDef,
     OpsFilterTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemFilterTypeDef,
     OpsItemNotificationTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsResultAttributeTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
-    PatchFilterGroupTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchOrchestratorFilterTypeDef,
-    PatchRuleGroupTypeDef,
-    PatchSourceTypeDef,
+    PatchRuleGroupUnionTypeDef,
+    PatchSourceUnionTypeDef,
     PutInventoryResultTypeDef,
     PutParameterResultTypeDef,
     PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupResultTypeDef,
     RegisterTargetWithMaintenanceWindowResultTypeDef,
     RegisterTaskWithMaintenanceWindowResultTypeDef,
     RegistrationMetadataItemTypeDef,
     RelatedOpsItemTypeDef,
     ResetServiceSettingResultTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     ResourceDataSyncSourceTypeDef,
     ResultAttributeTypeDef,
     ResumeSessionResponseTypeDef,
-    RunbookTypeDef,
+    RunbookUnionTypeDef,
     SendCommandResultTypeDef,
     SessionFilterTypeDef,
     StartAutomationExecutionResultTypeDef,
     StartChangeRequestExecutionResultTypeDef,
     StartSessionResponseTypeDef,
     StepExecutionFilterTypeDef,
     TagTypeDef,
-    TargetLocationTypeDef,
-    TargetTypeDef,
+    TargetLocationUnionTypeDef,
+    TargetUnionTypeDef,
     TerminateSessionResponseTypeDef,
+    TimestampTypeDef,
     UnlabelParameterVersionResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
     UpdateDocumentResultTypeDef,
     UpdateMaintenanceWindowResultTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
@@ -273,23 +273,26 @@
 from .waiter import CommandExecutedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SSMClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     AssociatedInstances: Type[BotocoreClientError]
     AssociationAlreadyExists: Type[BotocoreClientError]
     AssociationDoesNotExist: Type[BotocoreClientError]
     AssociationExecutionDoesNotExist: Type[BotocoreClientError]
     AssociationLimitExceeded: Type[BotocoreClientError]
@@ -413,14 +416,15 @@
     UnsupportedFeatureRequiredException: Type[BotocoreClientError]
     UnsupportedInventoryItemContextException: Type[BotocoreClientError]
     UnsupportedInventorySchemaVersionException: Type[BotocoreClientError]
     UnsupportedOperatingSystem: Type[BotocoreClientError]
     UnsupportedParameterType: Type[BotocoreClientError]
     UnsupportedPlatformType: Type[BotocoreClientError]
 
+
 class SSMClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
     """
 
     meta: ClientMeta
@@ -429,129 +433,139 @@
     def exceptions(self) -> Exceptions:
         """
         SSMClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#exceptions)
         """
+
     async def add_tags_to_resource(
         self,
         *,
         ResourceType: ResourceTypeForTaggingType,
         ResourceId: str,
         Tags: Sequence[TagTypeDef]
     ) -> Dict[str, Any]:
         """
         Adds or overwrites one or more tags for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.add_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#add_tags_to_resource)
         """
+
     async def associate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationType: str, ResourceType: str, ResourceUri: str
     ) -> AssociateOpsItemRelatedItemResponseTypeDef:
         """
         Associates a related item to a Systems Manager OpsCenter OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.associate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#associate_ops_item_related_item)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#can_paginate)
         """
+
     async def cancel_command(
         self, *, CommandId: str, InstanceIds: Sequence[str] = ...
     ) -> Dict[str, Any]:
         """
         Attempts to cancel the command specified by the Command ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_command)
         """
+
     async def cancel_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> CancelMaintenanceWindowExecutionResultTypeDef:
         """
         Stops a maintenance window execution that is already in progress and cancels any
         tasks in the window that haven't already starting running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.cancel_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#cancel_maintenance_window_execution)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#close)
         """
+
     async def create_activation(
         self,
         *,
         IamRole: str,
         Description: str = ...,
         DefaultInstanceName: str = ...,
         RegistrationLimit: int = ...,
-        ExpirationDate: Union[datetime, str] = ...,
+        ExpirationDate: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RegistrationMetadata: Sequence[RegistrationMetadataItemTypeDef] = ...
     ) -> CreateActivationResultTypeDef:
         """
         Generates an activation code and activation ID you can use to register your on-
         premises servers, edge devices, or virtual machine (VM) with Amazon Web Services
         Systems Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_activation)
         """
+
     async def create_association(
         self,
         *,
         Name: str,
         DocumentVersion: str = ...,
         InstanceId: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         AssociationName: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateAssociationResultTypeDef:
         """
         A State Manager association defines the state that you want to maintain on your
         managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association)
         """
+
     async def create_association_batch(
-        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryTypeDef]
+        self, *, Entries: Sequence[CreateAssociationBatchRequestEntryUnionTypeDef]
     ) -> CreateAssociationBatchResultTypeDef:
         """
         Associates the specified Amazon Web Services Systems Manager document (SSM
         document) with the specified managed nodes or targets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_association_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_association_batch)
         """
+
     async def create_document(
         self,
         *,
         Content: str,
         Name: str,
         Requires: Sequence[DocumentRequiresTypeDef] = ...,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
@@ -564,14 +578,15 @@
     ) -> CreateDocumentResultTypeDef:
         """
         Creates a Amazon Web Services Systems Manager (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_document)
         """
+
     async def create_maintenance_window(
         self,
         *,
         Name: str,
         Schedule: str,
         Duration: int,
         Cutoff: int,
@@ -586,40 +601,42 @@
     ) -> CreateMaintenanceWindowResultTypeDef:
         """
         Creates a new maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_maintenance_window)
         """
+
     async def create_ops_item(
         self,
         *,
         Description: str,
         Source: str,
         Title: str,
         OpsItemType: str = ...,
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         AccountId: str = ...
     ) -> CreateOpsItemResponseTypeDef:
         """
         Creates a new OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_item)
         """
+
     async def create_ops_metadata(
         self,
         *,
         ResourceId: str,
         Metadata: Mapping[str, MetadataValueTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateOpsMetadataResultTypeDef:
@@ -627,37 +644,39 @@
         If you create a new application in Application Manager, Amazon Web Services
         Systems Manager calls this API operation to specify information about the new
         application, including the application type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_ops_metadata)
         """
+
     async def create_patch_baseline(
         self,
         *,
         Name: str,
         OperatingSystem: OperatingSystemType = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePatchBaselineResultTypeDef:
         """
         Creates a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_patch_baseline)
         """
+
     async def create_resource_data_sync(
         self,
         *,
         SyncName: str,
         S3Destination: ResourceDataSyncS3DestinationTypeDef = ...,
         SyncType: str = ...,
         SyncSource: ResourceDataSyncSourceTypeDef = ...
@@ -665,41 +684,45 @@
         """
         A resource data sync helps you view data from multiple sources in a single
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.create_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#create_resource_data_sync)
         """
+
     async def delete_activation(self, *, ActivationId: str) -> Dict[str, Any]:
         """
         Deletes an activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_activation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_activation)
         """
+
     async def delete_association(
         self, *, Name: str = ..., InstanceId: str = ..., AssociationId: str = ...
     ) -> Dict[str, Any]:
         """
         Disassociates the specified Amazon Web Services Systems Manager document (SSM
         document) from the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_association)
         """
+
     async def delete_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ..., Force: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the Amazon Web Services Systems Manager document (SSM document) and all
         managed node associations to the document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_document)
         """
+
     async def delete_inventory(
         self,
         *,
         TypeName: str,
         SchemaDeleteOption: InventorySchemaDeleteOptionType = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
@@ -707,103 +730,115 @@
         """
         Delete a custom inventory type or the data associated with a custom Inventory
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_inventory)
         """
+
     async def delete_maintenance_window(
         self, *, WindowId: str
     ) -> DeleteMaintenanceWindowResultTypeDef:
         """
         Deletes a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_maintenance_window)
         """
+
     async def delete_ops_metadata(self, *, OpsMetadataArn: str) -> Dict[str, Any]:
         """
         Delete OpsMetadata related to an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_ops_metadata)
         """
+
     async def delete_parameter(self, *, Name: str) -> Dict[str, Any]:
         """
         Delete a parameter from the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameter)
         """
+
     async def delete_parameters(self, *, Names: Sequence[str]) -> DeleteParametersResultTypeDef:
         """
         Delete a list of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_parameters)
         """
+
     async def delete_patch_baseline(self, *, BaselineId: str) -> DeletePatchBaselineResultTypeDef:
         """
         Deletes a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_patch_baseline)
         """
+
     async def delete_resource_data_sync(
         self, *, SyncName: str, SyncType: str = ...
     ) -> Dict[str, Any]:
         """
         Deletes a resource data sync configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_data_sync)
         """
+
     async def delete_resource_policy(
         self, *, ResourceArn: str, PolicyId: str, PolicyHash: str
     ) -> Dict[str, Any]:
         """
         Deletes a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.delete_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#delete_resource_policy)
         """
+
     async def deregister_managed_instance(self, *, InstanceId: str) -> Dict[str, Any]:
         """
         Removes the server or virtual machine from the list of registered servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_managed_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_managed_instance)
         """
+
     async def deregister_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> DeregisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Removes a patch group from a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_patch_baseline_for_patch_group)
         """
+
     async def deregister_target_from_maintenance_window(
         self, *, WindowId: str, WindowTargetId: str, Safe: bool = ...
     ) -> DeregisterTargetFromMaintenanceWindowResultTypeDef:
         """
         Removes a target from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_target_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_target_from_maintenance_window)
         """
+
     async def deregister_task_from_maintenance_window(
         self, *, WindowId: str, WindowTaskId: str
     ) -> DeregisterTaskFromMaintenanceWindowResultTypeDef:
         """
         Removes a task from a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.deregister_task_from_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#deregister_task_from_maintenance_window)
         """
+
     async def describe_activations(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeActivationsResultTypeDef:
@@ -812,28 +847,30 @@
         was created, its expiration date, the Identity and Access Management (IAM) role
         assigned to the managed nodes in the activation, and the number of nodes
         registered by using this activation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_activations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_activations)
         """
+
     async def describe_association(
         self,
         *,
         Name: str = ...,
         InstanceId: str = ...,
         AssociationId: str = ...,
         AssociationVersion: str = ...
     ) -> DescribeAssociationResultTypeDef:
         """
         Describes the association for the specified target or managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association)
         """
+
     async def describe_association_execution_targets(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -841,41 +878,44 @@
     ) -> DescribeAssociationExecutionTargetsResultTypeDef:
         """
         Views information about a specific execution of a specific association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_execution_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_execution_targets)
         """
+
     async def describe_association_executions(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAssociationExecutionsResultTypeDef:
         """
         Views all executions for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_association_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_association_executions)
         """
+
     async def describe_automation_executions(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAutomationExecutionsResultTypeDef:
         """
         Provides details about all active and terminated Automation executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_executions)
         """
+
     async def describe_automation_step_executions(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
@@ -884,37 +924,40 @@
         """
         Information about all active and terminated step executions in an Automation
         workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_automation_step_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_automation_step_executions)
         """
+
     async def describe_available_patches(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeAvailablePatchesResultTypeDef:
         """
         Lists all patches eligible to be included in a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_available_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_available_patches)
         """
+
     async def describe_document(
         self, *, Name: str, DocumentVersion: str = ..., VersionName: str = ...
     ) -> DescribeDocumentResultTypeDef:
         """
         Describes the specified Amazon Web Services Systems Manager document (SSM
         document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document)
         """
+
     async def describe_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         MaxResults: int = ...,
         NextToken: str = ...
@@ -922,42 +965,46 @@
         """
         Describes the permissions for a Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_document_permission)
         """
+
     async def describe_effective_instance_associations(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectiveInstanceAssociationsResultTypeDef:
         """
         All associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_instance_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_instance_associations)
         """
+
     async def describe_effective_patches_for_patch_baseline(
         self, *, BaselineId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeEffectivePatchesForPatchBaselineResultTypeDef:
         """
         Retrieves the current effective patches (the patch and the approval state) for
         the specified patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_effective_patches_for_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_effective_patches_for_patch_baseline)
         """
+
     async def describe_instance_associations_status(
         self, *, InstanceId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeInstanceAssociationsStatusResultTypeDef:
         """
         The status of the associations for the managed node(s).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_associations_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_associations_status)
         """
+
     async def describe_instance_information(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -966,23 +1013,25 @@
         Describes one or more of your managed nodes, including information about the
         operating system platform, the version of SSM Agent installed on the managed
         node, node status, and so on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_information)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_information)
         """
+
     async def describe_instance_patch_states(
         self, *, InstanceIds: Sequence[str], NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInstancePatchStatesResultTypeDef:
         """
         Retrieves the high-level patch state of one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states)
         """
+
     async def describe_instance_patch_states_for_patch_group(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -990,14 +1039,15 @@
         """
         Retrieves the high-level patch state for the managed nodes in the specified
         patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patch_states_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patch_states_for_patch_group)
         """
+
     async def describe_instance_patches(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
@@ -1005,23 +1055,25 @@
         """
         Retrieves information about the patches on the specified managed node and their
         state relative to the patch baseline being used for the node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_instance_patches)
         """
+
     async def describe_inventory_deletions(
         self, *, DeletionId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInventoryDeletionsResultTypeDef:
         """
         Describes a specific delete inventory operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_inventory_deletions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_inventory_deletions)
         """
+
     async def describe_maintenance_window_execution_task_invocations(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
@@ -1030,177 +1082,190 @@
         """
         Retrieves the individual task executions (one per target) for a particular task
         run as part of a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_task_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_task_invocations)
         """
+
     async def describe_maintenance_window_execution_tasks(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionTasksResultTypeDef:
         """
         For a given maintenance window execution, lists the tasks that were run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_execution_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_execution_tasks)
         """
+
     async def describe_maintenance_window_executions(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowExecutionsResultTypeDef:
         """
         Lists the executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_executions)
         """
+
     async def describe_maintenance_window_schedule(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowScheduleResultTypeDef:
         """
         Retrieves information about upcoming executions of a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_schedule)
         """
+
     async def describe_maintenance_window_targets(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTargetsResultTypeDef:
         """
         Lists the targets registered with the maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_targets)
         """
+
     async def describe_maintenance_window_tasks(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowTasksResultTypeDef:
         """
         Lists the tasks in a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_window_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_window_tasks)
         """
+
     async def describe_maintenance_windows(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsResultTypeDef:
         """
         Retrieves the maintenance windows in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows)
         """
+
     async def describe_maintenance_windows_for_target(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeMaintenanceWindowsForTargetResultTypeDef:
         """
         Retrieves information about the maintenance window targets or tasks that a
         managed node is associated with.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_maintenance_windows_for_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_maintenance_windows_for_target)
         """
+
     async def describe_ops_items(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeOpsItemsResponseTypeDef:
         """
         Query a set of OpsItems.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_ops_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_ops_items)
         """
+
     async def describe_parameters(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeParametersResultTypeDef:
         """
         Get information about a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_parameters)
         """
+
     async def describe_patch_baselines(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribePatchBaselinesResultTypeDef:
         """
         Lists the patch baselines in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_baselines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_baselines)
         """
+
     async def describe_patch_group_state(
         self, *, PatchGroup: str
     ) -> DescribePatchGroupStateResultTypeDef:
         """
         Returns high-level aggregated patch compliance state information for a patch
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_group_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_group_state)
         """
+
     async def describe_patch_groups(
         self,
         *,
         MaxResults: int = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
         NextToken: str = ...
     ) -> DescribePatchGroupsResultTypeDef:
         """
         Lists all patch groups that have been registered with patch baselines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_groups)
         """
+
     async def describe_patch_properties(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
         MaxResults: int = ...,
@@ -1209,14 +1274,15 @@
         """
         Lists the properties of available patches organized by product, product family,
         classification, severity, and other properties of available patches.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_patch_properties)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_patch_properties)
         """
+
     async def describe_sessions(
         self,
         *,
         State: SessionStateType,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[SessionFilterTypeDef] = ...
@@ -1224,91 +1290,100 @@
         """
         Retrieves a list of all active sessions (both connected and disconnected) or
         terminated sessions from the past 30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#describe_sessions)
         """
+
     async def disassociate_ops_item_related_item(
         self, *, OpsItemId: str, AssociationId: str
     ) -> Dict[str, Any]:
         """
         Deletes the association between an OpsItem and a related item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.disassociate_ops_item_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#disassociate_ops_item_related_item)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#generate_presigned_url)
         """
+
     async def get_automation_execution(
         self, *, AutomationExecutionId: str
     ) -> GetAutomationExecutionResultTypeDef:
         """
         Get detailed information about a particular Automation execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_automation_execution)
         """
+
     async def get_calendar_state(
         self, *, CalendarNames: Sequence[str], AtTime: str = ...
     ) -> GetCalendarStateResponseTypeDef:
         """
         Gets the state of a Amazon Web Services Systems Manager change calendar at the
         current time or a specified time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_calendar_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_calendar_state)
         """
+
     async def get_command_invocation(
         self, *, CommandId: str, InstanceId: str, PluginName: str = ...
     ) -> GetCommandInvocationResultTypeDef:
         """
         Returns detailed information about command execution for an invocation or
         plugin.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_command_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_command_invocation)
         """
+
     async def get_connection_status(self, *, Target: str) -> GetConnectionStatusResponseTypeDef:
         """
         Retrieves the Session Manager connection status for a managed node to determine
         whether it is running and ready to receive Session Manager connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_connection_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_connection_status)
         """
+
     async def get_default_patch_baseline(
         self, *, OperatingSystem: OperatingSystemType = ...
     ) -> GetDefaultPatchBaselineResultTypeDef:
         """
         Retrieves the default patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_default_patch_baseline)
         """
+
     async def get_deployable_patch_snapshot_for_instance(
         self, *, InstanceId: str, SnapshotId: str, BaselineOverride: BaselineOverrideTypeDef = ...
     ) -> GetDeployablePatchSnapshotForInstanceResultTypeDef:
         """
         Retrieves the current snapshot for the patch baseline the managed node uses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_deployable_patch_snapshot_for_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_deployable_patch_snapshot_for_instance)
         """
+
     async def get_document(
         self,
         *,
         Name: str,
         VersionName: str = ...,
         DocumentVersion: str = ...,
         DocumentFormat: DocumentFormatType = ...
@@ -1316,14 +1391,15 @@
         """
         Gets the contents of the specified Amazon Web Services Systems Manager document
         (SSM document).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_document)
         """
+
     async def get_inventory(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
         NextToken: str = ...,
@@ -1331,14 +1407,15 @@
     ) -> GetInventoryResultTypeDef:
         """
         Query inventory information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory)
         """
+
     async def get_inventory_schema(
         self,
         *,
         TypeName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Aggregator: bool = ...,
@@ -1347,76 +1424,84 @@
         """
         Return a list of inventory type names for the account, or return a list of
         attribute names for a specific Inventory item type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_inventory_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_inventory_schema)
         """
+
     async def get_maintenance_window(self, *, WindowId: str) -> GetMaintenanceWindowResultTypeDef:
         """
         Retrieves a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window)
         """
+
     async def get_maintenance_window_execution(
         self, *, WindowExecutionId: str
     ) -> GetMaintenanceWindowExecutionResultTypeDef:
         """
         Retrieves details about a specific a maintenance window execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution)
         """
+
     async def get_maintenance_window_execution_task(
         self, *, WindowExecutionId: str, TaskId: str
     ) -> GetMaintenanceWindowExecutionTaskResultTypeDef:
         """
         Retrieves the details about a specific task run as part of a maintenance window
         execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task)
         """
+
     async def get_maintenance_window_execution_task_invocation(
         self, *, WindowExecutionId: str, TaskId: str, InvocationId: str
     ) -> GetMaintenanceWindowExecutionTaskInvocationResultTypeDef:
         """
         Retrieves information about a specific task running on a specific target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_execution_task_invocation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_execution_task_invocation)
         """
+
     async def get_maintenance_window_task(
         self, *, WindowId: str, WindowTaskId: str
     ) -> GetMaintenanceWindowTaskResultTypeDef:
         """
         Retrieves the details of a maintenance window task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_maintenance_window_task)
         """
+
     async def get_ops_item(
         self, *, OpsItemId: str, OpsItemArn: str = ...
     ) -> GetOpsItemResponseTypeDef:
         """
         Get information about an OpsItem by using the ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_item)
         """
+
     async def get_ops_metadata(
         self, *, OpsMetadataArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> GetOpsMetadataResultTypeDef:
         """
         View operational metadata related to an application in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_metadata)
         """
+
     async def get_ops_summary(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
@@ -1426,42 +1511,46 @@
         """
         View a summary of operations metadata (OpsData) based on specified filters and
         aggregators.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_ops_summary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_ops_summary)
         """
+
     async def get_parameter(
         self, *, Name: str, WithDecryption: bool = ...
     ) -> GetParameterResultTypeDef:
         """
         Get information about a single parameter by specifying the parameter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter)
         """
+
     async def get_parameter_history(
         self, *, Name: str, WithDecryption: bool = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> GetParameterHistoryResultTypeDef:
         """
         Retrieves the history of all changes to a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameter_history)
         """
+
     async def get_parameters(
         self, *, Names: Sequence[str], WithDecryption: bool = ...
     ) -> GetParametersResultTypeDef:
         """
         Get information about one or more parameters by specifying multiple parameter
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters)
         """
+
     async def get_parameters_by_path(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
@@ -1470,79 +1559,87 @@
     ) -> GetParametersByPathResultTypeDef:
         """
         Retrieve information about one or more parameters in a specific hierarchy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameters_by_path)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_parameters_by_path)
         """
+
     async def get_patch_baseline(self, *, BaselineId: str) -> GetPatchBaselineResultTypeDef:
         """
         Retrieves information about a patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline)
         """
+
     async def get_patch_baseline_for_patch_group(
         self, *, PatchGroup: str, OperatingSystem: OperatingSystemType = ...
     ) -> GetPatchBaselineForPatchGroupResultTypeDef:
         """
         Retrieves the patch baseline that should be used for the specified patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_patch_baseline_for_patch_group)
         """
+
     async def get_resource_policies(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> GetResourcePoliciesResponseTypeDef:
         """
         Returns an array of the `Policy` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_resource_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_resource_policies)
         """
+
     async def get_service_setting(self, *, SettingId: str) -> GetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_service_setting)
         """
+
     async def label_parameter_version(
         self, *, Name: str, Labels: Sequence[str], ParameterVersion: int = ...
     ) -> LabelParameterVersionResultTypeDef:
         """
         A parameter label is a user-defined alias to help you manage different versions
         of a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.label_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#label_parameter_version)
         """
+
     async def list_association_versions(
         self, *, AssociationId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAssociationVersionsResultTypeDef:
         """
         Retrieves all versions of an association for a specific association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_association_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_association_versions)
         """
+
     async def list_associations(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListAssociationsResultTypeDef:
         """
         Returns all State Manager associations in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_associations)
         """
+
     async def list_command_invocations(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1551,14 +1648,15 @@
     ) -> ListCommandInvocationsResultTypeDef:
         """
         An invocation is copy of a command sent to a specific managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_command_invocations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_command_invocations)
         """
+
     async def list_commands(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
@@ -1566,14 +1664,15 @@
     ) -> ListCommandsResultTypeDef:
         """
         Lists the commands requested by users of the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_commands)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_commands)
         """
+
     async def list_compliance_items(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
         NextToken: str = ...,
@@ -1582,28 +1681,30 @@
         """
         For a specified resource ID, this API operation returns a list of compliance
         statuses for different resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_items)
         """
+
     async def list_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListComplianceSummariesResultTypeDef:
         """
         Returns a summary count of compliant and non-compliant resources for a
         compliance type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_compliance_summaries)
         """
+
     async def list_document_metadata_history(
         self,
         *,
         Name: str,
         Metadata: Literal["DocumentReviews"],
         DocumentVersion: str = ...,
         NextToken: str = ...,
@@ -1612,23 +1713,25 @@
         """
         Information about approval reviews for a version of a change template in Change
         Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_metadata_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_metadata_history)
         """
+
     async def list_document_versions(
         self, *, Name: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListDocumentVersionsResultTypeDef:
         """
         List all versions for a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_document_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_document_versions)
         """
+
     async def list_documents(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1636,14 +1739,15 @@
         """
         Returns all Systems Manager (SSM) documents in the current Amazon Web Services
         account and Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_documents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_documents)
         """
+
     async def list_inventory_entries(
         self,
         *,
         InstanceId: str,
         TypeName: str,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         NextToken: str = ...,
@@ -1651,28 +1755,30 @@
     ) -> ListInventoryEntriesResultTypeDef:
         """
         A list of inventory items returned by the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_inventory_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_inventory_entries)
         """
+
     async def list_ops_item_events(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsItemEventsResponseTypeDef:
         """
         Returns a list of all OpsItem events in the current Amazon Web Services Region
         and Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_events)
         """
+
     async def list_ops_item_related_items(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -1680,59 +1786,64 @@
         """
         Lists all related-item resources associated with a Systems Manager OpsCenter
         OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_item_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_item_related_items)
         """
+
     async def list_ops_metadata(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when displaying all
         Application Manager OpsMetadata objects or blobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_ops_metadata)
         """
+
     async def list_resource_compliance_summaries(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListResourceComplianceSummariesResultTypeDef:
         """
         Returns a resource-level summary count.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_compliance_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_compliance_summaries)
         """
+
     async def list_resource_data_sync(
         self, *, SyncType: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListResourceDataSyncResultTypeDef:
         """
         Lists your resource data sync configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_resource_data_sync)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str
     ) -> ListTagsForResourceResultTypeDef:
         """
         Returns a list of the tags assigned to the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#list_tags_for_resource)
         """
+
     async def modify_document_permission(
         self,
         *,
         Name: str,
         PermissionType: Literal["Share"],
         AccountIdsToAdd: Sequence[str] = ...,
         AccountIdsToRemove: Sequence[str] = ...,
@@ -1741,41 +1852,44 @@
         """
         Shares a Amazon Web Services Systems Manager document (SSM document)publicly or
         privately.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.modify_document_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#modify_document_permission)
         """
+
     async def put_compliance_items(
         self,
         *,
         ResourceId: str,
         ResourceType: str,
         ComplianceType: str,
-        ExecutionSummary: ComplianceExecutionSummaryTypeDef,
+        ExecutionSummary: ComplianceExecutionSummaryUnionTypeDef,
         Items: Sequence[ComplianceItemEntryTypeDef],
         ItemContentHash: str = ...,
         UploadType: ComplianceUploadTypeType = ...
     ) -> Dict[str, Any]:
         """
         Registers a compliance type and other compliance details on a designated
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_compliance_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_compliance_items)
         """
+
     async def put_inventory(
         self, *, InstanceId: str, Items: Sequence[InventoryItemTypeDef]
     ) -> PutInventoryResultTypeDef:
         """
         Bulk update custom inventory items on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_inventory)
         """
+
     async def put_parameter(
         self,
         *,
         Name: str,
         Value: str,
         Description: str = ...,
         Type: ParameterTypeType = ...,
@@ -1789,200 +1903,216 @@
     ) -> PutParameterResultTypeDef:
         """
         Add a parameter to the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_parameter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_parameter)
         """
+
     async def put_resource_policy(
         self, *, ResourceArn: str, Policy: str, PolicyId: str = ..., PolicyHash: str = ...
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Creates or updates a Systems Manager resource policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#put_resource_policy)
         """
+
     async def register_default_patch_baseline(
         self, *, BaselineId: str
     ) -> RegisterDefaultPatchBaselineResultTypeDef:
         """
         Defines the default patch baseline for the relevant operating system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_default_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_default_patch_baseline)
         """
+
     async def register_patch_baseline_for_patch_group(
         self, *, BaselineId: str, PatchGroup: str
     ) -> RegisterPatchBaselineForPatchGroupResultTypeDef:
         """
         Registers a patch baseline for a patch group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_patch_baseline_for_patch_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_patch_baseline_for_patch_group)
         """
+
     async def register_target_with_maintenance_window(
         self,
         *,
         WindowId: str,
         ResourceType: MaintenanceWindowResourceTypeType,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[TargetUnionTypeDef],
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> RegisterTargetWithMaintenanceWindowResultTypeDef:
         """
         Registers a target with a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_target_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_target_with_maintenance_window)
         """
+
     async def register_task_with_maintenance_window(
         self,
         *,
         WindowId: str,
         TaskArn: str,
         TaskType: MaintenanceWindowTaskTypeType,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
+        ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         ClientToken: str = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> RegisterTaskWithMaintenanceWindowResultTypeDef:
         """
         Adds a new task to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.register_task_with_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#register_task_with_maintenance_window)
         """
+
     async def remove_tags_from_resource(
         self, *, ResourceType: ResourceTypeForTaggingType, ResourceId: str, TagKeys: Sequence[str]
     ) -> Dict[str, Any]:
         """
         Removes tag keys from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.remove_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#remove_tags_from_resource)
         """
+
     async def reset_service_setting(self, *, SettingId: str) -> ResetServiceSettingResultTypeDef:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.reset_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#reset_service_setting)
         """
+
     async def resume_session(self, *, SessionId: str) -> ResumeSessionResponseTypeDef:
         """
         Reconnects a session to a managed node after it has been disconnected.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.resume_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#resume_session)
         """
+
     async def send_automation_signal(
         self,
         *,
         AutomationExecutionId: str,
         SignalType: SignalTypeType,
         Payload: Mapping[str, Sequence[str]] = ...
     ) -> Dict[str, Any]:
         """
         Sends a signal to an Automation execution to change the current behavior or
         status of the execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_automation_signal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_automation_signal)
         """
+
     async def send_command(
         self,
         *,
         DocumentName: str,
         InstanceIds: Sequence[str] = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         DocumentVersion: str = ...,
         DocumentHash: str = ...,
         DocumentHashType: DocumentHashTypeType = ...,
         TimeoutSeconds: int = ...,
         Comment: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         OutputS3Region: str = ...,
         OutputS3BucketName: str = ...,
         OutputS3KeyPrefix: str = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         ServiceRoleArn: str = ...,
-        NotificationConfig: NotificationConfigTypeDef = ...,
+        NotificationConfig: NotificationConfigUnionTypeDef = ...,
         CloudWatchOutputConfig: CloudWatchOutputConfigTypeDef = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> SendCommandResultTypeDef:
         """
         Runs commands on one or more managed nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.send_command)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#send_command)
         """
+
     async def start_associations_once(self, *, AssociationIds: Sequence[str]) -> Dict[str, Any]:
         """
         Runs an association immediately and only one time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_associations_once)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_associations_once)
         """
+
     async def start_automation_execution(
         self,
         *,
         DocumentName: str,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ClientToken: str = ...,
         Mode: ExecutionModeType = ...,
         TargetParameterName: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> StartAutomationExecutionResultTypeDef:
         """
         Initiates execution of an Automation runbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_automation_execution)
         """
+
     async def start_change_request_execution(
         self,
         *,
         DocumentName: str,
-        Runbooks: Sequence[RunbookTypeDef],
-        ScheduledTime: Union[datetime, str] = ...,
+        Runbooks: Sequence[RunbookUnionTypeDef],
+        ScheduledTime: TimestampTypeDef = ...,
         DocumentVersion: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...,
         ChangeRequestName: str = ...,
         ClientToken: str = ...,
         AutoApprove: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ScheduledEndTime: Union[datetime, str] = ...,
+        ScheduledEndTime: TimestampTypeDef = ...,
         ChangeDetails: str = ...
     ) -> StartChangeRequestExecutionResultTypeDef:
         """
         Creates a change request for Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_change_request_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_change_request_execution)
         """
+
     async def start_session(
         self,
         *,
         Target: str,
         DocumentName: str = ...,
         Reason: str = ...,
         Parameters: Mapping[str, Sequence[str]] = ...
@@ -1990,80 +2120,86 @@
         """
         Initiates a connection to a target (for example, a managed node) for a Session
         Manager session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.start_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#start_session)
         """
+
     async def stop_automation_execution(
         self, *, AutomationExecutionId: str, Type: StopTypeType = ...
     ) -> Dict[str, Any]:
         """
         Stop an Automation that is currently running.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.stop_automation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#stop_automation_execution)
         """
+
     async def terminate_session(self, *, SessionId: str) -> TerminateSessionResponseTypeDef:
         """
         Permanently ends a session and closes the data connection between the Session
         Manager client and SSM Agent on the managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.terminate_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#terminate_session)
         """
+
     async def unlabel_parameter_version(
         self, *, Name: str, ParameterVersion: int, Labels: Sequence[str]
     ) -> UnlabelParameterVersionResultTypeDef:
         """
         Remove a label or labels from a parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.unlabel_parameter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#unlabel_parameter_version)
         """
+
     async def update_association(
         self,
         *,
         AssociationId: str,
         Parameters: Mapping[str, Sequence[str]] = ...,
         DocumentVersion: str = ...,
         ScheduleExpression: str = ...,
         OutputLocation: InstanceAssociationOutputLocationTypeDef = ...,
         Name: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         AssociationName: str = ...,
         AssociationVersion: str = ...,
         AutomationTargetParameterName: str = ...,
         MaxErrors: str = ...,
         MaxConcurrency: str = ...,
         ComplianceSeverity: AssociationComplianceSeverityType = ...,
         SyncCompliance: AssociationSyncComplianceType = ...,
         ApplyOnlyAtCronInterval: bool = ...,
         CalendarNames: Sequence[str] = ...,
-        TargetLocations: Sequence[TargetLocationTypeDef] = ...,
+        TargetLocations: Sequence[TargetLocationUnionTypeDef] = ...,
         ScheduleOffset: int = ...,
         TargetMaps: Sequence[Mapping[str, Sequence[str]]] = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateAssociationResultTypeDef:
         """
         Updates an association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association)
         """
+
     async def update_association_status(
-        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusTypeDef
+        self, *, Name: str, InstanceId: str, AssociationStatus: AssociationStatusUnionTypeDef
     ) -> UpdateAssociationStatusResultTypeDef:
         """
         Updates the status of the Amazon Web Services Systems Manager document (SSM
         document) associated with the specified managed node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_association_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_association_status)
         """
+
     async def update_document(
         self,
         *,
         Content: str,
         Name: str,
         Attachments: Sequence[AttachmentsSourceTypeDef] = ...,
         DisplayName: str = ...,
@@ -2074,33 +2210,36 @@
     ) -> UpdateDocumentResultTypeDef:
         """
         Updates one or more values for an SSM document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document)
         """
+
     async def update_document_default_version(
         self, *, Name: str, DocumentVersion: str
     ) -> UpdateDocumentDefaultVersionResultTypeDef:
         """
         Set the default version of a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_default_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_default_version)
         """
+
     async def update_document_metadata(
         self, *, Name: str, DocumentReviews: DocumentReviewsTypeDef, DocumentVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates information related to approval reviews for a specific version of a
         change template in Change Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_document_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_document_metadata)
         """
+
     async def update_maintenance_window(
         self,
         *,
         WindowId: str,
         Name: str = ...,
         Description: str = ...,
         StartDate: str = ...,
@@ -2116,521 +2255,581 @@
     ) -> UpdateMaintenanceWindowResultTypeDef:
         """
         Updates an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window)
         """
+
     async def update_maintenance_window_target(
         self,
         *,
         WindowId: str,
         WindowTargetId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         OwnerInformation: str = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...
     ) -> UpdateMaintenanceWindowTargetResultTypeDef:
         """
         Modifies the target of an existing maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_target)
         """
+
     async def update_maintenance_window_task(
         self,
         *,
         WindowId: str,
         WindowTaskId: str,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         TaskArn: str = ...,
         ServiceRoleArn: str = ...,
-        TaskParameters: Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef] = ...,
-        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersTypeDef = ...,
+        TaskParameters: Mapping[
+            str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef
+        ] = ...,
+        TaskInvocationParameters: MaintenanceWindowTaskInvocationParametersUnionTypeDef = ...,
         Priority: int = ...,
         MaxConcurrency: str = ...,
         MaxErrors: str = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Name: str = ...,
         Description: str = ...,
         Replace: bool = ...,
         CutoffBehavior: MaintenanceWindowTaskCutoffBehaviorType = ...,
-        AlarmConfiguration: AlarmConfigurationTypeDef = ...
+        AlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> UpdateMaintenanceWindowTaskResultTypeDef:
         """
         Modifies a task assigned to a maintenance window.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_maintenance_window_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_maintenance_window_task)
         """
+
     async def update_managed_instance_role(
         self, *, InstanceId: str, IamRole: str
     ) -> Dict[str, Any]:
         """
         Changes the Identity and Access Management (IAM) role that is assigned to the
         on-premises server, edge device, or virtual machines (VM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_managed_instance_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_managed_instance_role)
         """
+
     async def update_ops_item(
         self,
         *,
         OpsItemId: str,
         Description: str = ...,
         OperationalData: Mapping[str, OpsItemDataValueTypeDef] = ...,
         OperationalDataToDelete: Sequence[str] = ...,
         Notifications: Sequence[OpsItemNotificationTypeDef] = ...,
         Priority: int = ...,
         RelatedOpsItems: Sequence[RelatedOpsItemTypeDef] = ...,
         Status: OpsItemStatusType = ...,
         Title: str = ...,
         Category: str = ...,
         Severity: str = ...,
-        ActualStartTime: Union[datetime, str] = ...,
-        ActualEndTime: Union[datetime, str] = ...,
-        PlannedStartTime: Union[datetime, str] = ...,
-        PlannedEndTime: Union[datetime, str] = ...,
+        ActualStartTime: TimestampTypeDef = ...,
+        ActualEndTime: TimestampTypeDef = ...,
+        PlannedStartTime: TimestampTypeDef = ...,
+        PlannedEndTime: TimestampTypeDef = ...,
         OpsItemArn: str = ...
     ) -> Dict[str, Any]:
         """
         Edit or change an OpsItem.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_item)
         """
+
     async def update_ops_metadata(
         self,
         *,
         OpsMetadataArn: str,
         MetadataToUpdate: Mapping[str, MetadataValueTypeDef] = ...,
         KeysToDelete: Sequence[str] = ...
     ) -> UpdateOpsMetadataResultTypeDef:
         """
         Amazon Web Services Systems Manager calls this API operation when you edit
         OpsMetadata in Application Manager.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_ops_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_ops_metadata)
         """
+
     async def update_patch_baseline(
         self,
         *,
         BaselineId: str,
         Name: str = ...,
-        GlobalFilters: PatchFilterGroupTypeDef = ...,
-        ApprovalRules: PatchRuleGroupTypeDef = ...,
+        GlobalFilters: PatchFilterGroupUnionTypeDef = ...,
+        ApprovalRules: PatchRuleGroupUnionTypeDef = ...,
         ApprovedPatches: Sequence[str] = ...,
         ApprovedPatchesComplianceLevel: PatchComplianceLevelType = ...,
         ApprovedPatchesEnableNonSecurity: bool = ...,
         RejectedPatches: Sequence[str] = ...,
         RejectedPatchesAction: PatchActionType = ...,
         Description: str = ...,
-        Sources: Sequence[PatchSourceTypeDef] = ...,
+        Sources: Sequence[PatchSourceUnionTypeDef] = ...,
         Replace: bool = ...
     ) -> UpdatePatchBaselineResultTypeDef:
         """
         Modifies an existing patch baseline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_patch_baseline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_patch_baseline)
         """
+
     async def update_resource_data_sync(
         self, *, SyncName: str, SyncType: str, SyncSource: ResourceDataSyncSourceTypeDef
     ) -> Dict[str, Any]:
         """
         Update a resource data sync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_resource_data_sync)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_resource_data_sync)
         """
+
     async def update_service_setting(self, *, SettingId: str, SettingValue: str) -> Dict[str, Any]:
         """
         `ServiceSetting` is an account-level setting for an Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.update_service_setting)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#update_service_setting)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_activations"]
     ) -> DescribeActivationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_execution_targets"]
     ) -> DescribeAssociationExecutionTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_association_executions"]
     ) -> DescribeAssociationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_executions"]
     ) -> DescribeAutomationExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_automation_step_executions"]
     ) -> DescribeAutomationStepExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_available_patches"]
     ) -> DescribeAvailablePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_instance_associations"]
     ) -> DescribeEffectiveInstanceAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_effective_patches_for_patch_baseline"]
     ) -> DescribeEffectivePatchesForPatchBaselinePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_associations_status"]
     ) -> DescribeInstanceAssociationsStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_information"]
     ) -> DescribeInstanceInformationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states"]
     ) -> DescribeInstancePatchStatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patch_states_for_patch_group"]
     ) -> DescribeInstancePatchStatesForPatchGroupPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_instance_patches"]
     ) -> DescribeInstancePatchesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_inventory_deletions"]
     ) -> DescribeInventoryDeletionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_task_invocations"]
     ) -> DescribeMaintenanceWindowExecutionTaskInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_execution_tasks"]
     ) -> DescribeMaintenanceWindowExecutionTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_executions"]
     ) -> DescribeMaintenanceWindowExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_schedule"]
     ) -> DescribeMaintenanceWindowSchedulePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_targets"]
     ) -> DescribeMaintenanceWindowTargetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_window_tasks"]
     ) -> DescribeMaintenanceWindowTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows"]
     ) -> DescribeMaintenanceWindowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_maintenance_windows_for_target"]
     ) -> DescribeMaintenanceWindowsForTargetPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_ops_items"]
     ) -> DescribeOpsItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_parameters"]
     ) -> DescribeParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_baselines"]
     ) -> DescribePatchBaselinesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_groups"]
     ) -> DescribePatchGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_patch_properties"]
     ) -> DescribePatchPropertiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_sessions"]
     ) -> DescribeSessionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_inventory"]) -> GetInventoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_inventory_schema"]
     ) -> GetInventorySchemaPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_ops_summary"]) -> GetOpsSummaryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameter_history"]
     ) -> GetParameterHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_parameters_by_path"]
     ) -> GetParametersByPathPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_resource_policies"]
     ) -> GetResourcePoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_association_versions"]
     ) -> ListAssociationVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_associations"]
     ) -> ListAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_command_invocations"]
     ) -> ListCommandInvocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_commands"]) -> ListCommandsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_items"]
     ) -> ListComplianceItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_compliance_summaries"]
     ) -> ListComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_document_versions"]
     ) -> ListDocumentVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_documents"]) -> ListDocumentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_events"]
     ) -> ListOpsItemEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_item_related_items"]
     ) -> ListOpsItemRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_ops_metadata"]
     ) -> ListOpsMetadataPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_compliance_summaries"]
     ) -> ListResourceComplianceSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_data_sync"]
     ) -> ListResourceDataSyncPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_paginator)
         """
+
     def get_waiter(self, waiter_name: Literal["command_executed"]) -> CommandExecutedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "SSMClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/client/)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/literals.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/literals.pyi` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/paginator.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
@@ -271,15 +271,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
         """
 
 
@@ -291,15 +291,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 
@@ -310,15 +310,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAssociationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 
@@ -328,15 +328,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAutomationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 
@@ -348,15 +348,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAutomationStepExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 
@@ -366,60 +366,60 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 
 class DescribeEffectiveInstanceAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEffectiveInstanceAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
         """
 
 
 class DescribeEffectivePatchesForPatchBaselinePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
     """
 
     def paginate(
-        self, *, BaselineId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BaselineId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEffectivePatchesForPatchBaselineResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
         """
 
 
 class DescribeInstanceAssociationsStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceassociationsstatuspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstanceAssociationsStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceassociationsstatuspaginator)
         """
 
 
@@ -430,30 +430,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 
 class DescribeInstancePatchStatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstancePatchStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatespaginator)
         """
 
 
@@ -464,15 +464,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 
@@ -483,30 +483,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 
 class DescribeInventoryDeletionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
-        self, *, DeletionId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeletionId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInventoryDeletionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinventorydeletionspaginator)
         """
 
 
@@ -518,15 +518,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 
@@ -537,15 +537,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 
@@ -556,15 +556,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 
@@ -574,18 +574,18 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 
@@ -596,15 +596,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 
@@ -615,15 +615,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 
@@ -633,15 +633,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 
@@ -650,17 +650,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 
@@ -670,15 +670,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
         """
 
 
@@ -689,15 +689,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeparameterspaginator)
         """
 
 
@@ -707,15 +707,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 
@@ -725,15 +725,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
         """
 
 
@@ -745,15 +745,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 
@@ -764,15 +764,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describesessionspaginator)
         """
 
 
@@ -784,15 +784,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventorypaginator)
         """
 
 
@@ -804,15 +804,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventoryschemapaginator)
         """
 
 
@@ -825,15 +825,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getopssummarypaginator)
         """
 
 
@@ -844,15 +844,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparameterhistorypaginator)
         """
 
 
@@ -865,45 +865,45 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparametersbypathpaginator)
         """
 
 
 class GetResourcePoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getresourcepoliciespaginator)
         """
 
 
 class ListAssociationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationversionspaginator)
     """
 
     def paginate(
-        self, *, AssociationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AssociationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationversionspaginator)
         """
 
 
@@ -913,15 +913,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
         """
 
 
@@ -934,15 +934,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 
@@ -954,15 +954,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCommandsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandspaginator)
         """
 
 
@@ -974,15 +974,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 
@@ -992,30 +992,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 
 class ListDocumentVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentversionspaginator)
         """
 
 
@@ -1026,15 +1026,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentspaginator)
         """
 
 
@@ -1044,15 +1044,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
         """
 
 
@@ -1063,15 +1063,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 
@@ -1081,15 +1081,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
         """
 
 
@@ -1099,28 +1099,28 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 
 class ListResourceDataSyncPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcedatasyncpaginator)
     """
 
     def paginate(
-        self, *, SyncType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SyncType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceDataSyncResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcedatasyncpaginator)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/paginator.pyi` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     PaginatorConfigTypeDef,
     ParametersFilterTypeDef,
     ParameterStringFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     ResultAttributeTypeDef,
     SessionFilterTypeDef,
     StepExecutionFilterTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
 )
 
 __all__ = (
     "DescribeActivationsPaginator",
     "DescribeAssociationExecutionTargetsPaginator",
     "DescribeAssociationExecutionsPaginator",
     "DescribeAutomationExecutionsPaginator",
@@ -268,15 +268,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[DescribeActivationsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeActivationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeActivations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeactivationspaginator)
         """
 
 class DescribeAssociationExecutionTargetsPaginator(AioPaginator):
@@ -287,15 +287,15 @@
 
     def paginate(
         self,
         *,
         AssociationId: str,
         ExecutionId: str,
         Filters: Sequence[AssociationExecutionTargetsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAssociationExecutionTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutionTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutiontargetspaginator)
         """
 
 class DescribeAssociationExecutionsPaginator(AioPaginator):
@@ -305,15 +305,15 @@
     """
 
     def paginate(
         self,
         *,
         AssociationId: str,
         Filters: Sequence[AssociationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAssociationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAssociationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeassociationexecutionspaginator)
         """
 
 class DescribeAutomationExecutionsPaginator(AioPaginator):
@@ -322,15 +322,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[AutomationExecutionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAutomationExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationexecutionspaginator)
         """
 
 class DescribeAutomationStepExecutionsPaginator(AioPaginator):
@@ -341,15 +341,15 @@
 
     def paginate(
         self,
         *,
         AutomationExecutionId: str,
         Filters: Sequence[StepExecutionFilterTypeDef] = ...,
         ReverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAutomationStepExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAutomationStepExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeautomationstepexecutionspaginator)
         """
 
 class DescribeAvailablePatchesPaginator(AioPaginator):
@@ -358,57 +358,57 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAvailablePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeAvailablePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeavailablepatchespaginator)
         """
 
 class DescribeEffectiveInstanceAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEffectiveInstanceAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectiveInstanceAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectiveinstanceassociationspaginator)
         """
 
 class DescribeEffectivePatchesForPatchBaselinePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
     """
 
     def paginate(
-        self, *, BaselineId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, BaselineId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEffectivePatchesForPatchBaselineResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeEffectivePatchesForPatchBaseline.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeeffectivepatchesforpatchbaselinepaginator)
         """
 
 class DescribeInstanceAssociationsStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceassociationsstatuspaginator)
     """
 
     def paginate(
-        self, *, InstanceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstanceAssociationsStatusResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceAssociationsStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceassociationsstatuspaginator)
         """
 
 class DescribeInstanceInformationPaginator(AioPaginator):
@@ -418,29 +418,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceInformationFilterList: Sequence[InstanceInformationFilterTypeDef] = ...,
         Filters: Sequence[InstanceInformationStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstanceInformationResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceInformation.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstanceinformationpaginator)
         """
 
 class DescribeInstancePatchStatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstancePatchStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatespaginator)
         """
 
 class DescribeInstancePatchStatesForPatchGroupPaginator(AioPaginator):
@@ -450,15 +450,15 @@
     """
 
     def paginate(
         self,
         *,
         PatchGroup: str,
         Filters: Sequence[InstancePatchStateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstancePatchStatesForPatchGroupResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatchStatesForPatchGroup.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchstatesforpatchgrouppaginator)
         """
 
 class DescribeInstancePatchesPaginator(AioPaginator):
@@ -468,29 +468,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceId: str,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 class DescribeInventoryDeletionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
-        self, *, DeletionId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeletionId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeInventoryDeletionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeinventorydeletionspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTaskInvocationsPaginator(AioPaginator):
@@ -501,15 +501,15 @@
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         TaskId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTaskInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskinvocationspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionTasksPaginator(AioPaginator):
@@ -519,15 +519,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowExecutionId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutionTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutiontaskspaginator)
         """
 
 class DescribeMaintenanceWindowExecutionsPaginator(AioPaginator):
@@ -537,15 +537,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowExecutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowexecutionspaginator)
         """
 
 class DescribeMaintenanceWindowSchedulePaginator(AioPaginator):
@@ -554,18 +554,18 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
     """
 
     def paginate(
         self,
         *,
         WindowId: str = ...,
-        Targets: Sequence[TargetTypeDef] = ...,
+        Targets: Sequence[TargetUnionTypeDef] = ...,
         ResourceType: MaintenanceWindowResourceTypeType = ...,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowScheduleResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowSchedule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowschedulepaginator)
         """
 
 class DescribeMaintenanceWindowTargetsPaginator(AioPaginator):
@@ -575,15 +575,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowTargetsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtargetspaginator)
         """
 
 class DescribeMaintenanceWindowTasksPaginator(AioPaginator):
@@ -593,15 +593,15 @@
     """
 
     def paginate(
         self,
         *,
         WindowId: str,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowtaskspaginator)
         """
 
 class DescribeMaintenanceWindowsPaginator(AioPaginator):
@@ -610,15 +610,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[MaintenanceWindowFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowspaginator)
         """
 
 class DescribeMaintenanceWindowsForTargetPaginator(AioPaginator):
@@ -626,17 +626,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
     """
 
     def paginate(
         self,
         *,
-        Targets: Sequence[TargetTypeDef],
+        Targets: Sequence[TargetUnionTypeDef],
         ResourceType: MaintenanceWindowResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMaintenanceWindowsForTargetResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeMaintenanceWindowsForTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describemaintenancewindowsfortargetpaginator)
         """
 
 class DescribeOpsItemsPaginator(AioPaginator):
@@ -645,15 +645,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
     """
 
     def paginate(
         self,
         *,
         OpsItemFilters: Sequence[OpsItemFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOpsItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeOpsItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeopsitemspaginator)
         """
 
 class DescribeParametersPaginator(AioPaginator):
@@ -663,15 +663,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ParametersFilterTypeDef] = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describeparameterspaginator)
         """
 
 class DescribePatchBaselinesPaginator(AioPaginator):
@@ -680,15 +680,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePatchBaselinesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchBaselines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchbaselinespaginator)
         """
 
 class DescribePatchGroupsPaginator(AioPaginator):
@@ -697,15 +697,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PatchOrchestratorFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePatchGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchgroupspaginator)
         """
 
 class DescribePatchPropertiesPaginator(AioPaginator):
@@ -716,15 +716,15 @@
 
     def paginate(
         self,
         *,
         OperatingSystem: OperatingSystemType,
         Property: PatchPropertyType,
         PatchSet: PatchSetType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePatchPropertiesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribePatchProperties.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describepatchpropertiespaginator)
         """
 
 class DescribeSessionsPaginator(AioPaginator):
@@ -734,15 +734,15 @@
     """
 
     def paginate(
         self,
         *,
         State: SessionStateType,
         Filters: Sequence[SessionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#describesessionspaginator)
         """
 
 class GetInventoryPaginator(AioPaginator):
@@ -753,15 +753,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[InventoryFilterTypeDef] = ...,
         Aggregators: Sequence["InventoryAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[ResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetInventoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventorypaginator)
         """
 
 class GetInventorySchemaPaginator(AioPaginator):
@@ -772,15 +772,15 @@
 
     def paginate(
         self,
         *,
         TypeName: str = ...,
         Aggregator: bool = ...,
         SubType: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetInventorySchemaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetInventorySchema.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getinventoryschemapaginator)
         """
 
 class GetOpsSummaryPaginator(AioPaginator):
@@ -792,15 +792,15 @@
     def paginate(
         self,
         *,
         SyncName: str = ...,
         Filters: Sequence[OpsFilterTypeDef] = ...,
         Aggregators: Sequence["OpsAggregatorTypeDef"] = ...,
         ResultAttributes: Sequence[OpsResultAttributeTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetOpsSummaryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetOpsSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getopssummarypaginator)
         """
 
 class GetParameterHistoryPaginator(AioPaginator):
@@ -810,15 +810,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetParameterHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParameterHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparameterhistorypaginator)
         """
 
 class GetParametersByPathPaginator(AioPaginator):
@@ -830,43 +830,43 @@
     def paginate(
         self,
         *,
         Path: str,
         Recursive: bool = ...,
         ParameterFilters: Sequence[ParameterStringFilterTypeDef] = ...,
         WithDecryption: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetParametersByPathResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetParametersByPath.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getparametersbypathpaginator)
         """
 
 class GetResourcePoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.GetResourcePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#getresourcepoliciespaginator)
         """
 
 class ListAssociationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationversionspaginator)
     """
 
     def paginate(
-        self, *, AssociationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AssociationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociationVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationversionspaginator)
         """
 
 class ListAssociationsPaginator(AioPaginator):
@@ -875,15 +875,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         AssociationFilterList: Sequence[AssociationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listassociationspaginator)
         """
 
 class ListCommandInvocationsPaginator(AioPaginator):
@@ -895,15 +895,15 @@
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
         Details: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCommandInvocationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommandInvocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandinvocationspaginator)
         """
 
 class ListCommandsPaginator(AioPaginator):
@@ -914,15 +914,15 @@
 
     def paginate(
         self,
         *,
         CommandId: str = ...,
         InstanceId: str = ...,
         Filters: Sequence[CommandFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCommandsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListCommands.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcommandspaginator)
         """
 
 class ListComplianceItemsPaginator(AioPaginator):
@@ -933,15 +933,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
         ResourceIds: Sequence[str] = ...,
         ResourceTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComplianceItemsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcomplianceitemspaginator)
         """
 
 class ListComplianceSummariesPaginator(AioPaginator):
@@ -950,29 +950,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listcompliancesummariespaginator)
         """
 
 class ListDocumentVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocumentVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentversionspaginator)
         """
 
 class ListDocumentsPaginator(AioPaginator):
@@ -982,15 +982,15 @@
     """
 
     def paginate(
         self,
         *,
         DocumentFilterList: Sequence[DocumentFilterTypeDef] = ...,
         Filters: Sequence[DocumentKeyValuesFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDocumentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListDocuments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listdocumentspaginator)
         """
 
 class ListOpsItemEventsPaginator(AioPaginator):
@@ -999,15 +999,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsItemEventFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpsItemEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemeventspaginator)
         """
 
 class ListOpsItemRelatedItemsPaginator(AioPaginator):
@@ -1017,15 +1017,15 @@
     """
 
     def paginate(
         self,
         *,
         OpsItemId: str = ...,
         Filters: Sequence[OpsItemRelatedItemsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpsItemRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsItemRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsitemrelateditemspaginator)
         """
 
 class ListOpsMetadataPaginator(AioPaginator):
@@ -1034,15 +1034,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[OpsMetadataFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOpsMetadataResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListOpsMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listopsmetadatapaginator)
         """
 
 class ListResourceComplianceSummariesPaginator(AioPaginator):
@@ -1051,27 +1051,27 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[ComplianceStringFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceComplianceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceComplianceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcecompliancesummariespaginator)
         """
 
 class ListResourceDataSyncPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcedatasyncpaginator)
     """
 
     def paginate(
-        self, *, SyncType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SyncType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceDataSyncResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.ListResourceDataSync.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/paginators/#listresourcedatasyncpaginator)
         """
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/type_defs.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ssm.type_defs import AccountSharingInfoTypeDef
 
-    data: AccountSharingInfoTypeDef = {...}
+    data: AccountSharingInfoTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from aiobotocore.response import StreamingBody
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationExecutionFilterKeyType,
     AssociationExecutionTargetsFilterKeyType,
     AssociationFilterKeyType,
     AssociationFilterOperatorTypeType,
@@ -99,299 +101,303 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
-    "AssociationStatusTypeDef",
-    "TargetTypeDef",
+    "AssociationStatusOutputTypeDef",
+    "TargetOutputTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
+    "TimestampTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
+    "BlobTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
-    "CancelMaintenanceWindowExecutionResultTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
-    "NotificationConfigTypeDef",
-    "ComplianceExecutionSummaryTypeDef",
+    "NotificationConfigOutputTypeDef",
+    "ComplianceExecutionSummaryOutputTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
-    "CreateActivationResultTypeDef",
+    "TargetTypeDef",
     "DocumentRequiresTypeDef",
-    "CreateMaintenanceWindowResultTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
-    "CreateOpsItemResponseTypeDef",
     "MetadataValueTypeDef",
-    "CreateOpsMetadataResultTypeDef",
-    "CreatePatchBaselineResultTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
-    "DeleteMaintenanceWindowResultTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
     "DeleteParametersRequestRequestTypeDef",
-    "DeleteParametersResultTypeDef",
     "DeletePatchBaselineRequestRequestTypeDef",
-    "DeletePatchBaselineResultTypeDef",
     "DeleteResourceDataSyncRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeregisterManagedInstanceRequestRequestTypeDef",
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
     "DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     "DescribeActivationsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAssociationRequestRequestTypeDef",
     "StepExecutionFilterTypeDef",
     "PatchOrchestratorFilterTypeDef",
     "PatchTypeDef",
     "DescribeDocumentPermissionRequestRequestTypeDef",
     "DescribeDocumentRequestRequestTypeDef",
-    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     "InstanceAssociationTypeDef",
-    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
-    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
-    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
     "OpsItemFilterTypeDef",
     "ParameterStringFilterTypeDef",
     "ParametersFilterTypeDef",
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
-    "DescribePatchGroupStateResultTypeDef",
-    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
-    "DescribePatchPropertiesResultTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
-    "GetCalendarStateResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetCommandInvocationRequestRequestTypeDef",
     "GetConnectionStatusRequestRequestTypeDef",
-    "GetConnectionStatusResponseTypeDef",
     "GetDefaultPatchBaselineRequestRequestTypeDef",
-    "GetDefaultPatchBaselineResultTypeDef",
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionResultTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
-    "GetMaintenanceWindowResultTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
-    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "GetPatchBaselineForPatchGroupResultTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
-    "LabelParameterVersionResultTypeDef",
-    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationVersionsRequestRequestTypeDef",
     "ListDocumentMetadataHistoryRequestRequestTypeDef",
-    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     "ListDocumentVersionsRequestRequestTypeDef",
-    "ListInventoryEntriesResultTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
-    "MaintenanceWindowLambdaParametersTypeDef",
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
+    "NotificationConfigTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterInlinePolicyTypeDef",
+    "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
-    "PutInventoryResultTypeDef",
-    "PutParameterResultTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
-    "RegisterDefaultPatchBaselineResultTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeSessionRequestRequestTypeDef",
-    "ResumeSessionResponseTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
-    "StartAutomationExecutionResultTypeDef",
-    "StartChangeRequestExecutionResultTypeDef",
     "StartSessionRequestRequestTypeDef",
-    "StartSessionResponseTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionRequestRequestTypeDef",
-    "UnlabelParameterVersionResultTypeDef",
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     "UpdateMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowResultTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
-    "UpdateOpsMetadataResultTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
-    "DescribeDocumentPermissionResponseTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "PutParameterRequestRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
+    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "CancelMaintenanceWindowExecutionResultTypeDef",
+    "CreateActivationResultTypeDef",
+    "CreateMaintenanceWindowResultTypeDef",
+    "CreateOpsItemResponseTypeDef",
+    "CreateOpsMetadataResultTypeDef",
+    "CreatePatchBaselineResultTypeDef",
+    "DeleteMaintenanceWindowResultTypeDef",
+    "DeleteParametersResultTypeDef",
+    "DeletePatchBaselineResultTypeDef",
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
+    "DescribeDocumentPermissionResponseTypeDef",
+    "DescribePatchGroupStateResultTypeDef",
+    "DescribePatchPropertiesResultTypeDef",
+    "GetCalendarStateResponseTypeDef",
+    "GetConnectionStatusResponseTypeDef",
+    "GetDefaultPatchBaselineResultTypeDef",
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    "GetMaintenanceWindowResultTypeDef",
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    "LabelParameterVersionResultTypeDef",
+    "ListInventoryEntriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PutInventoryResultTypeDef",
+    "PutParameterResultTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
+    "ResumeSessionResponseTypeDef",
+    "StartAutomationExecutionResultTypeDef",
+    "StartChangeRequestExecutionResultTypeDef",
+    "StartSessionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
+    "UnlabelParameterVersionResultTypeDef",
+    "UpdateMaintenanceWindowResultTypeDef",
+    "UpdateOpsMetadataResultTypeDef",
     "AssociationTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
-    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
-    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListAssociationsRequestRequestTypeDef",
+    "AssociationStatusTypeDef",
+    "ComplianceExecutionSummaryTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
+    "MaintenanceWindowLambdaParametersTypeDef",
     "GetCommandInvocationResultTypeDef",
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
-    "ListCommandsRequestListCommandsPaginateTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
-    "MaintenanceWindowRunCommandParametersTypeDef",
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     "ComplianceItemTypeDef",
-    "PutComplianceItemsRequestRequestTypeDef",
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
+    "TargetUnionTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
     "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
-    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     "DescribeActivationsRequestRequestTypeDef",
+    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
+    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     "DescribePatchBaselinesRequestRequestTypeDef",
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     "DescribePatchGroupsRequestRequestTypeDef",
     "DescribeAvailablePatchesResultTypeDef",
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
@@ -443,14 +449,15 @@
     "GetInventoryRequestRequestTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
+    "PatchSourceUnionTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
@@ -460,39 +467,56 @@
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
+    "MaintenanceWindowRunCommandParametersTypeDef",
+    "NotificationConfigUnionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionUnionTypeDef",
     "OpsEntityTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
+    "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
+    "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
-    "SendCommandRequestRequestTypeDef",
+    "TargetLocationOutputTypeDef",
+    "AlarmConfigurationUnionTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
+    "AssociationStatusUnionTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    "ComplianceExecutionSummaryUnionTypeDef",
+    "PutComplianceItemsRequestRequestTypeDef",
     "ListCommandInvocationsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "SendCommandRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "ListDocumentsResultTypeDef",
     "DescribeOpsItemsResponseTypeDef",
     "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
@@ -502,69 +526,80 @@
     "InventoryAggregatorTypeDef",
     "DescribeInstanceInformationResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
+    "PatchRuleOutputTypeDef",
+    "PatchFilterGroupUnionTypeDef",
     "PatchRuleTypeDef",
-    "ResourceDataSyncSourceTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
+    "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
+    "CreateAssociationBatchRequestEntryOutputTypeDef",
+    "RunbookOutputTypeDef",
+    "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
-    "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
-    "StartAutomationExecutionRequestRequestTypeDef",
-    "StepExecutionTypeDef",
-    "UpdateAssociationRequestRequestTypeDef",
+    "TargetLocationUnionTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersUnionTypeDef",
+    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
+    "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
-    "ResourceDataSyncItemTypeDef",
     "CreateAssociationResultTypeDef",
     "DescribeAssociationResultTypeDef",
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
+    "CreateAssociationBatchRequestEntryUnionTypeDef",
+    "RunbookUnionTypeDef",
+    "CreateAssociationRequestRequestTypeDef",
+    "StartAutomationExecutionRequestRequestTypeDef",
+    "UpdateAssociationRequestRequestTypeDef",
+    "GetPatchBaselineResultTypeDef",
+    "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
-    "GetPatchBaselineResultTypeDef",
+    "PatchRuleGroupUnionTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
-    "UpdatePatchBaselineResultTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
 AccountSharingInfoTypeDef = TypedDict(
     "AccountSharingInfoTypeDef",
     {
         "AccountId": str,
@@ -602,60 +637,61 @@
         "OpsItemId": str,
         "AssociationType": str,
         "ResourceType": str,
         "ResourceUri": str,
     },
 )
 
-AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AssociationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociationOverviewTypeDef = TypedDict(
     "AssociationOverviewTypeDef",
     {
         "Status": str,
         "DetailedStatus": str,
         "AssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
+_RequiredAssociationStatusOutputTypeDef = TypedDict(
+    "_RequiredAssociationStatusOutputTypeDef",
     {
         "Date": datetime,
         "Name": AssociationStatusNameType,
         "Message": str,
     },
 )
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
+_OptionalAssociationStatusOutputTypeDef = TypedDict(
+    "_OptionalAssociationStatusOutputTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+class AssociationStatusOutputTypeDef(
+    _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
 ):
     pass
 
-
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
     total=False,
 )
 
 AssociationExecutionFilterTypeDef = TypedDict(
     "AssociationExecutionFilterTypeDef",
     {
@@ -686,14 +722,15 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -754,50 +791,41 @@
     {
         "Name": str,
         "Products": Sequence[str],
         "Configuration": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCancelCommandRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCommandRequestRequestTypeDef",
     {
         "CommandId": str,
     },
 )
 _OptionalCancelCommandRequestRequestTypeDef = TypedDict(
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
-
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "CancelMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
     },
     total=False,
@@ -826,46 +854,45 @@
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
     total=False,
 )
 
-NotificationConfigTypeDef = TypedDict(
-    "NotificationConfigTypeDef",
+NotificationConfigOutputTypeDef = TypedDict(
+    "NotificationConfigOutputTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": List[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
-_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryTypeDef",
+_RequiredComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryOutputTypeDef",
     {
         "ExecutionTime": datetime,
     },
 )
-_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryTypeDef",
+_OptionalComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryOutputTypeDef",
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
-
-class ComplianceExecutionSummaryTypeDef(
-    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
+class ComplianceExecutionSummaryOutputTypeDef(
+    _RequiredComplianceExecutionSummaryOutputTypeDef,
+    _OptionalComplianceExecutionSummaryOutputTypeDef,
 ):
     pass
 
-
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -875,21 +902,19 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
-
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -913,21 +938,21 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateActivationResultTypeDef = TypedDict(
-    "CreateActivationResultTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
-        "ActivationId": str,
-        "ActivationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Values": Sequence[str],
     },
+    total=False,
 )
 
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
@@ -938,27 +963,17 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
-
-CreateMaintenanceWindowResultTypeDef = TypedDict(
-    "CreateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
     total=False,
@@ -975,47 +990,22 @@
 RelatedOpsItemTypeDef = TypedDict(
     "RelatedOpsItemTypeDef",
     {
         "OpsItemId": str,
     },
 )
 
-CreateOpsItemResponseTypeDef = TypedDict(
-    "CreateOpsItemResponseTypeDef",
-    {
-        "OpsItemId": str,
-        "OpsItemArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetadataValueTypeDef = TypedDict(
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-CreateOpsMetadataResultTypeDef = TypedDict(
-    "CreateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePatchBaselineResultTypeDef = TypedDict(
-    "CreatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1041,21 +1031,19 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
-
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1064,36 +1052,26 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
-
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-DeleteMaintenanceWindowResultTypeDef = TypedDict(
-    "DeleteMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOpsMetadataRequestRequestTypeDef = TypedDict(
     "DeleteOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 
@@ -1107,60 +1085,41 @@
 DeleteParametersRequestRequestTypeDef = TypedDict(
     "DeleteParametersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
-DeleteParametersResultTypeDef = TypedDict(
-    "DeleteParametersResultTypeDef",
-    {
-        "DeletedParameters": List[str],
-        "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePatchBaselineRequestRequestTypeDef = TypedDict(
     "DeletePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-DeletePatchBaselineResultTypeDef = TypedDict(
-    "DeletePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
-
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1177,23 +1136,14 @@
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
@@ -1201,57 +1151,47 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
-
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
-DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeActivationsFilterTypeDef = TypedDict(
     "DescribeActivationsFilterTypeDef",
     {
         "FilterKey": DescribeActivationsFilterKeysType,
         "FilterValues": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeAssociationRequestRequestTypeDef = TypedDict(
     "DescribeAssociationRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationId": str,
         "AssociationVersion": str,
@@ -1318,22 +1258,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1341,43 +1279,19 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
-
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
-    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
@@ -1385,55 +1299,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
     },
     total=False,
 )
 
-_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "BaselineId": str,
-    },
-)
-_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
-    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
@@ -1441,44 +1331,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
-    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
@@ -1486,22 +1352,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1553,43 +1417,19 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
-
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
-
-_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-    },
-)
-_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
-    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
 _OptionalDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
@@ -1597,22 +1437,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1624,30 +1462,19 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
-
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
-
-DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    {
-        "DeletionId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1753,21 +1580,19 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
-
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1787,57 +1612,14 @@
 DescribePatchGroupStateRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupStateRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 
-DescribePatchGroupStateResultTypeDef = TypedDict(
-    "DescribePatchGroupStateResultTypeDef",
-    {
-        "Instances": int,
-        "InstancesWithInstalledPatches": int,
-        "InstancesWithInstalledOtherPatches": int,
-        "InstancesWithInstalledPendingRebootPatches": int,
-        "InstancesWithInstalledRejectedPatches": int,
-        "InstancesWithMissingPatches": int,
-        "InstancesWithFailedPatches": int,
-        "InstancesWithNotApplicablePatches": int,
-        "InstancesWithUnreportedNotApplicablePatches": int,
-        "InstancesWithCriticalNonCompliantPatches": int,
-        "InstancesWithSecurityNonCompliantPatches": int,
-        "InstancesWithOtherNonCompliantPatches": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "OperatingSystem": OperatingSystemType,
-        "Property": PatchPropertyType,
-    },
-)
-_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "PatchSet": PatchSetType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
-    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribePatchPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -1847,31 +1629,20 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
-
-DescribePatchPropertiesResultTypeDef = TypedDict(
-    "DescribePatchPropertiesResultTypeDef",
-    {
-        "Properties": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
 )
@@ -1995,31 +1766,19 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
-
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
-
-GetCalendarStateResponseTypeDef = TypedDict(
-    "GetCalendarStateResponseTypeDef",
-    {
-        "State": CalendarStateType,
-        "AtTime": str,
-        "NextTransitionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -2036,66 +1795,35 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
-
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
-GetConnectionStatusResponseTypeDef = TypedDict(
-    "GetConnectionStatusResponseTypeDef",
-    {
-        "Target": str,
-        "Status": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetDefaultPatchBaselineRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-GetDefaultPatchBaselineResultTypeDef = TypedDict(
-    "GetDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": str,
-        "SnapshotDownloadUrl": str,
-        "Product": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -2104,21 +1832,19 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
-
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2126,37 +1852,24 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    {
-        "TypeName": str,
-        "Aggregator": bool,
-        "SubType": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInventorySchemaRequestRequestTypeDef = TypedDict(
     "GetInventorySchemaRequestRequestTypeDef",
     {
         "TypeName": str,
         "NextToken": str,
         "MaxResults": int,
         "Aggregator": bool,
@@ -2168,100 +1881,46 @@
 GetMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskIds": List[str],
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "InvocationId": str,
     },
 )
 
-GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskExecutionId": str,
-        "InvocationId": str,
-        "ExecutionId": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "Parameters": str,
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "OwnerInformation": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 
-MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+MaintenanceWindowTaskParameterValueExpressionOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-GetMaintenanceWindowResultTypeDef = TypedDict(
-    "GetMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "NextExecutionTime": str,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -2277,40 +1936,36 @@
     "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
-
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2318,21 +1973,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2340,49 +1993,24 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
-
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
-
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
-    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetParameterHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterHistoryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterHistoryRequestRequestTypeDef = TypedDict(
@@ -2391,43 +2019,39 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
-
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2450,82 +2074,55 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
-
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
-GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
     {
-        "ResourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
     },
-    total=False,
 )
 
-
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2533,22 +2130,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2634,19 +2229,17 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
-
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
-
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2656,21 +2249,19 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
-
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
-
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2678,53 +2269,20 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
-
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
-
-LabelParameterVersionResultTypeDef = TypedDict(
-    "LabelParameterVersionResultTypeDef",
-    {
-        "InvalidLabels": List[str],
-        "ParameterVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
-    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalListAssociationVersionsRequestRequestTypeDef = TypedDict(
@@ -2732,22 +2290,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2757,44 +2313,20 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
-    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -2802,35 +2334,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListInventoryEntriesResultTypeDef = TypedDict(
-    "ListInventoryEntriesResultTypeDef",
-    {
-        "TypeName": str,
-        "InstanceId": str,
-        "SchemaVersion": str,
-        "CaptureTime": str,
-        "Entries": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
     },
@@ -2861,23 +2378,14 @@
         "LastModifiedDate": datetime,
         "LastModifiedUser": str,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
-    {
-        "SyncType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceDataSyncRequestRequestTypeDef = TypedDict(
     "ListResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2888,42 +2396,69 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
+MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Dict[str, List[str]],
+    },
+    total=False,
+)
+
 MaintenanceWindowAutomationParametersTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersTypeDef",
+MaintenanceWindowLambdaParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
     {
         "ClientContext": str,
         "Qualifier": str,
         "Payload": bytes,
     },
     total=False,
 )
 
+NotificationConfigTypeDef = TypedDict(
+    "NotificationConfigTypeDef",
+    {
+        "NotificationArn": str,
+        "NotificationEvents": Sequence[NotificationEventType],
+        "NotificationType": NotificationTypeType,
+    },
+    total=False,
+)
+
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
 )
 
+MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    {
+        "Values": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredModifyDocumentPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDocumentPermissionRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionType": Literal["Share"],
     },
 )
@@ -2933,22 +2468,20 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
-
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
-
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
@@ -2958,56 +2491,37 @@
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
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
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
     total=False,
 )
 
-PatchFilterTypeDef = TypedDict(
-    "PatchFilterTypeDef",
+PatchFilterOutputTypeDef = TypedDict(
+    "PatchFilterOutputTypeDef",
     {
         "Key": PatchFilterKeyType,
-        "Values": Sequence[str],
-    },
-)
-
-PutInventoryResultTypeDef = TypedDict(
-    "PutInventoryResultTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Values": List[str],
     },
 )
 
-PutParameterResultTypeDef = TypedDict(
-    "PutParameterResultTypeDef",
+PatchFilterTypeDef = TypedDict(
+    "PatchFilterTypeDef",
     {
-        "Version": int,
-        "Tier": ParameterTierType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": PatchFilterKeyType,
+        "Values": Sequence[str],
     },
 )
 
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -3019,78 +2533,34 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyHash": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -3115,42 +2585,21 @@
     "ResourceDataSyncDestinationDataSharingTypeDef",
     {
         "DestinationDataSharingType": str,
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
 ResumeSessionRequestRequestTypeDef = TypedDict(
     "ResumeSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-ResumeSessionResponseTypeDef = TypedDict(
-    "ResumeSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendAutomationSignalRequestRequestTypeDef = TypedDict(
     "_RequiredSendAutomationSignalRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
         "SignalType": SignalTypeType,
     },
 )
@@ -3158,22 +2607,20 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
-
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -3182,30 +2629,14 @@
 StartAssociationsOnceRequestRequestTypeDef = TypedDict(
     "StartAssociationsOnceRequestRequestTypeDef",
     {
         "AssociationIds": Sequence[str],
     },
 )
 
-StartAutomationExecutionResultTypeDef = TypedDict(
-    "StartAutomationExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartChangeRequestExecutionResultTypeDef = TypedDict(
-    "StartChangeRequestExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 _OptionalStartSessionRequestRequestTypeDef = TypedDict(
@@ -3214,86 +2645,55 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
-
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnlabelParameterVersionRequestRequestTypeDef = TypedDict(
     "UnlabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "ParameterVersion": int,
         "Labels": Sequence[str],
     },
 )
 
-UnlabelParameterVersionResultTypeDef = TypedDict(
-    "UnlabelParameterVersionResultTypeDef",
-    {
-        "RemovedLabels": List[str],
-        "InvalidLabels": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDocumentDefaultVersionRequestRequestTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
     },
 )
@@ -3319,75 +2719,36 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateMaintenanceWindowResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
 
-UpdateOpsMetadataResultTypeDef = TypedDict(
-    "UpdateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateServiceSettingRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
         "SettingValue": str,
     },
 )
 
-DescribeDocumentPermissionResponseTypeDef = TypedDict(
-    "DescribeDocumentPermissionResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivationTypeDef = TypedDict(
     "ActivationTypeDef",
     {
         "ActivationId": str,
         "Description": str,
         "DefaultInstanceName": str,
         "IamRole": str,
@@ -3430,30 +2791,20 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -3469,20 +2820,37 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
-
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
+_RequiredAlarmConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAlarmConfigurationOutputTypeDef",
+    {
+        "Alarms": List[AlarmTypeDef],
+    },
+)
+_OptionalAlarmConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAlarmConfigurationOutputTypeDef",
+    {
+        "IgnorePollAlarmFailure": bool,
+    },
+    total=False,
+)
+
+class AlarmConfigurationOutputTypeDef(
+    _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
@@ -3490,204 +2858,485 @@
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
-
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
+AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
+        "AssociationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociationTypeDef = TypedDict(
-    "AssociationTypeDef",
+CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "CancelMaintenanceWindowExecutionResultTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationId": str,
-        "AssociationVersion": str,
-        "DocumentVersion": str,
-        "Targets": List[TargetTypeDef],
-        "LastExecutionDate": datetime,
-        "Overview": AssociationOverviewTypeDef,
-        "ScheduleExpression": str,
-        "AssociationName": str,
-        "ScheduleOffset": int,
-        "TargetMaps": List[Dict[str, List[str]]],
+        "WindowExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+CreateActivationResultTypeDef = TypedDict(
+    "CreateActivationResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "ActivationId": str,
+        "ActivationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+
+CreateMaintenanceWindowResultTypeDef = TypedDict(
+    "CreateMaintenanceWindowResultTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateOpsItemResponseTypeDef = TypedDict(
+    "CreateOpsItemResponseTypeDef",
+    {
+        "OpsItemId": str,
+        "OpsItemArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
-
+CreateOpsMetadataResultTypeDef = TypedDict(
+    "CreateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+CreatePatchBaselineResultTypeDef = TypedDict(
+    "CreatePatchBaselineResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+
+DeleteMaintenanceWindowResultTypeDef = TypedDict(
+    "DeleteMaintenanceWindowResultTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DeleteParametersResultTypeDef = TypedDict(
+    "DeleteParametersResultTypeDef",
+    {
+        "DeletedParameters": List[str],
+        "InvalidParameters": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
+DeletePatchBaselineResultTypeDef = TypedDict(
+    "DeletePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-MaintenanceWindowTargetTypeDef = TypedDict(
-    "MaintenanceWindowTargetTypeDef",
+DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": List[TargetTypeDef],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetTypeDef],
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+
+DescribeDocumentPermissionResponseTypeDef = TypedDict(
+    "DescribeDocumentPermissionResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchGroupStateResultTypeDef = TypedDict(
+    "DescribePatchGroupStateResultTypeDef",
+    {
+        "Instances": int,
+        "InstancesWithInstalledPatches": int,
+        "InstancesWithInstalledOtherPatches": int,
+        "InstancesWithInstalledPendingRebootPatches": int,
+        "InstancesWithInstalledRejectedPatches": int,
+        "InstancesWithMissingPatches": int,
+        "InstancesWithFailedPatches": int,
+        "InstancesWithNotApplicablePatches": int,
+        "InstancesWithUnreportedNotApplicablePatches": int,
+        "InstancesWithCriticalNonCompliantPatches": int,
+        "InstancesWithSecurityNonCompliantPatches": int,
+        "InstancesWithOtherNonCompliantPatches": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchPropertiesResultTypeDef = TypedDict(
+    "DescribePatchPropertiesResultTypeDef",
+    {
+        "Properties": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalendarStateResponseTypeDef = TypedDict(
+    "GetCalendarStateResponseTypeDef",
+    {
+        "State": CalendarStateType,
+        "AtTime": str,
+        "NextTransitionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectionStatusResponseTypeDef = TypedDict(
+    "GetConnectionStatusResponseTypeDef",
+    {
+        "Target": str,
+        "Status": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDefaultPatchBaselineResultTypeDef = TypedDict(
+    "GetDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": str,
+        "SnapshotDownloadUrl": str,
+        "Product": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionResultTypeDef",
     {
+        "WindowExecutionId": str,
+        "TaskIds": List[str],
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskExecutionId": str,
+        "InvocationId": str,
+        "ExecutionId": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "Parameters": str,
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "OwnerInformation": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowResultTypeDef = TypedDict(
+    "GetMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "ClientToken": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "NextExecutionTime": str,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+LabelParameterVersionResultTypeDef = TypedDict(
+    "LabelParameterVersionResultTypeDef",
+    {
+        "InvalidLabels": List[str],
+        "ParameterVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
+ListInventoryEntriesResultTypeDef = TypedDict(
+    "ListInventoryEntriesResultTypeDef",
+    {
+        "TypeName": str,
+        "InstanceId": str,
+        "SchemaVersion": str,
+        "CaptureTime": str,
+        "Entries": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+PutInventoryResultTypeDef = TypedDict(
+    "PutInventoryResultTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutParameterResultTypeDef = TypedDict(
+    "PutParameterResultTypeDef",
+    {
+        "Version": int,
+        "Tier": ParameterTierType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyHash": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
     {
-        "WindowId": str,
         "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+
+RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "OwnerInformation": str,
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResumeSessionResponseTypeDef = TypedDict(
+    "ResumeSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAutomationExecutionResultTypeDef = TypedDict(
+    "StartAutomationExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartChangeRequestExecutionResultTypeDef = TypedDict(
+    "StartChangeRequestExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnlabelParameterVersionResultTypeDef = TypedDict(
+    "UnlabelParameterVersionResultTypeDef",
+    {
+        "RemovedLabels": List[str],
+        "InvalidLabels": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceWindowResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "Replace": bool,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateOpsMetadataResultTypeDef = TypedDict(
+    "UpdateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
+AssociationTypeDef = TypedDict(
+    "AssociationTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationId": str,
+        "AssociationVersion": str,
+        "DocumentVersion": str,
+        "Targets": List[TargetOutputTypeDef],
+        "LastExecutionDate": datetime,
+        "Overview": AssociationOverviewTypeDef,
+        "ScheduleExpression": str,
+        "AssociationName": str,
+        "ScheduleOffset": int,
+        "TargetMaps": List[Dict[str, List[str]]],
+    },
+    total=False,
+)
 
+MaintenanceWindowTargetTypeDef = TypedDict(
+    "MaintenanceWindowTargetTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": List[TargetOutputTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+    },
+    total=False,
+)
 
 UpdateMaintenanceWindowTargetResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTargetResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "AssociationId": str,
-        },
-    )
-)
-_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "Filters": Sequence[AssociationExecutionFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
@@ -3696,22 +3345,20 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3720,38 +3367,14 @@
         "DetailedStatus": str,
         "LastExecutionDate": datetime,
         "OutputSource": OutputSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "AssociationId": str,
-        "ExecutionId": str,
-    },
-)
-_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef",
     {
         "AssociationId": str,
         "ExecutionId": str,
     },
 )
@@ -3761,41 +3384,71 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
-
-ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+ListAssociationsRequestRequestTypeDef = TypedDict(
+    "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-ListAssociationsRequestRequestTypeDef = TypedDict(
-    "ListAssociationsRequestRequestTypeDef",
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
     {
-        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "Date": TimestampTypeDef,
+        "Name": AssociationStatusNameType,
+        "Message": str,
+    },
+)
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
+    {
+        "AdditionalInfo": str,
+    },
+    total=False,
+)
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+):
+    pass
+
+_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionTime": TimestampTypeDef,
+    },
+)
+_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionId": str,
+        "ExecutionType": str,
     },
     total=False,
 )
 
+class ComplianceExecutionSummaryTypeDef(
+    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
+):
+    pass
+
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3808,36 +3461,35 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-
-DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestRequestTypeDef",
+MaintenanceWindowLambdaParametersTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersTypeDef",
     {
-        "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": BlobTypeDef,
     },
     total=False,
 )
 
 GetCommandInvocationResultTypeDef = TypedDict(
     "GetCommandInvocationResultTypeDef",
     {
@@ -3854,28 +3506,16 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "Details": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
@@ -3883,25 +3523,14 @@
         "NextToken": str,
         "Filters": Sequence[CommandFilterTypeDef],
         "Details": bool,
     },
     total=False,
 )
 
-ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCommandsRequestRequestTypeDef = TypedDict(
     "ListCommandsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -3923,29 +3552,29 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
     },
     total=False,
 )
 
-MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersTypeDef",
+MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     {
         "Comment": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
@@ -3957,98 +3586,42 @@
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Id": str,
         "Title": str,
         "Status": ComplianceStatusType,
         "Severity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ComplianceType": str,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
-        "Items": Sequence[ComplianceItemEntryTypeDef],
-    },
-)
-_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ItemContentHash": str,
-        "UploadType": ComplianceUploadTypeType,
-    },
-    total=False,
-)
-
-
-class PutComplianceItemsRequestRequestTypeDef(
-    _RequiredPutComplianceItemsRequestRequestTypeDef,
-    _OptionalPutComplianceItemsRequestRequestTypeDef,
-):
-    pass
-
-
-ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "ResourceIds": Sequence[str],
-        "ResourceTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -4081,28 +3654,27 @@
 )
 _OptionalCreateActivationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateActivationRequestRequestTypeDef",
     {
         "Description": str,
         "DefaultInstanceName": str,
         "RegistrationLimit": int,
-        "ExpirationDate": Union[datetime, str],
+        "ExpirationDate": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
-
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
-
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -4117,21 +3689,19 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
-
 DocumentIdentifierTypeDef = TypedDict(
     "DocumentIdentifierTypeDef",
     {
         "Name": str,
         "CreatedDate": datetime,
         "DisplayName": str,
         "Owner": str,
@@ -4162,15 +3732,15 @@
         "StatusInformation": str,
         "Content": str,
         "DocumentType": DocumentTypeType,
         "DocumentFormat": DocumentFormatType,
         "Requires": List[DocumentRequiresTypeDef],
         "AttachmentsContent": List[AttachmentContentTypeDef],
         "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpsItemSummaryTypeDef = TypedDict(
     "OpsItemSummaryTypeDef",
     {
         "CreatedBy": str,
@@ -4209,30 +3779,28 @@
         "OperationalData": Mapping[str, OpsItemDataValueTypeDef],
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Tags": Sequence[TagTypeDef],
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 OpsItemTypeDef = TypedDict(
     "OpsItemTypeDef",
     {
         "CreatedBy": str,
         "OpsItemType": str,
         "CreatedTime": datetime,
         "Description": str,
@@ -4273,30 +3841,28 @@
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Status": OpsItemStatusType,
         "Title": str,
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "OpsItemArn": str,
     },
     total=False,
 )
 
-
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -4304,28 +3870,26 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
@@ -4336,36 +3900,363 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+DescribeActivationsRequestRequestTypeDef = TypedDict(
+    "DescribeActivationsRequestRequestTypeDef",
+    {
+        "Filters": Sequence[DescribeActivationsFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
 
 DescribeActivationsRequestDescribeActivationsPaginateTypeDef = TypedDict(
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeActivationsRequestRequestTypeDef = TypedDict(
-    "DescribeActivationsRequestRequestTypeDef",
+_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     {
-        "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "AssociationId": str,
+        "ExecutionId": str,
+    },
+)
+_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "AssociationId": str,
+        },
+    )
+)
+_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "Filters": Sequence[AssociationExecutionFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+):
+    pass
+
+DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    {
+        "Filters": Sequence[AutomationExecutionFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
+    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "BaselineId": str,
+    },
+)
+_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
+    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
+    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+    },
+)
+_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
+    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+):
+    pass
+
+DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    {
+        "DeletionId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "OperatingSystem": OperatingSystemType,
+        "Property": PatchPropertyType,
+    },
+)
+_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "PatchSet": PatchSetType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
+    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+):
+    pass
+
+GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    {
+        "TypeName": str,
+        "Aggregator": bool,
+        "SubType": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "WithDecryption": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
+    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
+    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+):
+    pass
+
+ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    {
+        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "Details": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "ResourceIds": Sequence[str],
+        "ResourceTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
+    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    {
+        "SyncType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
@@ -4373,27 +4264,25 @@
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4403,27 +4292,25 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
-
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeAvailablePatchesRequestRequestTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestRequestTypeDef",
     {
@@ -4440,27 +4327,25 @@
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4469,54 +4354,25 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
-    TypedDict(
-        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-        {
-            "WindowId": str,
-            "Targets": Sequence[TargetTypeDef],
-            "ResourceType": MaintenanceWindowResourceTypeType,
-            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchBaselinesRequestRequestTypeDef = TypedDict(
     "DescribePatchBaselinesRequestRequestTypeDef",
     {
@@ -4527,15 +4383,15 @@
     total=False,
 )
 
 DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef = TypedDict(
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchGroupsRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupsRequestRequestTypeDef",
     {
@@ -4547,33 +4403,33 @@
 )
 
 DescribeAvailablePatchesResultTypeDef = TypedDict(
     "DescribeAvailablePatchesResultTypeDef",
     {
         "Patches": List[PatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEffectiveInstanceAssociationsResultTypeDef = TypedDict(
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     {
         "Associations": List[InstanceAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef = TypedDict(
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     {
         "InstanceInformationFilterList": Sequence[InstanceInformationFilterTypeDef],
         "Filters": Sequence[InstanceInformationStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeInstanceInformationRequestRequestTypeDef = TypedDict(
     "DescribeInstanceInformationRequestRequestTypeDef",
     {
@@ -4591,27 +4447,25 @@
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4620,73 +4474,69 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchStatesResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchesResultTypeDef = TypedDict(
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4696,45 +4546,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4743,45 +4589,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4790,45 +4632,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4837,45 +4675,41 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4884,27 +4718,25 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeMaintenanceWindowsRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestRequestTypeDef",
     {
@@ -4918,59 +4750,59 @@
 DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef",
     {
         "WindowExecutionTaskInvocationIdentities": List[
             MaintenanceWindowExecutionTaskInvocationIdentityTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionsResultTypeDef",
     {
         "WindowExecutions": List[MaintenanceWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowScheduleResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleResultTypeDef",
     {
         "ScheduledWindowExecutions": List[ScheduledWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsForTargetResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsForTargetResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityForTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef = TypedDict(
     "DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef",
     {
         "OpsItemFilters": Sequence[OpsItemFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeOpsItemsRequestRequestTypeDef = TypedDict(
     "DescribeOpsItemsRequestRequestTypeDef",
     {
@@ -4989,27 +4821,25 @@
 )
 _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef = TypedDict(
     "_OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef",
     {
         "Recursive": bool,
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -5020,28 +4850,26 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeParametersRequestRequestTypeDef = TypedDict(
     "DescribeParametersRequestRequestTypeDef",
     {
@@ -5054,15 +4882,15 @@
 )
 
 DescribePatchBaselinesResultTypeDef = TypedDict(
     "DescribePatchBaselinesResultTypeDef",
     {
         "BaselineIdentities": List[PatchBaselineIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PatchGroupPatchBaselineMappingTypeDef = TypedDict(
     "PatchGroupPatchBaselineMappingTypeDef",
     {
         "PatchGroup": str,
@@ -5077,27 +4905,25 @@
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
         "Filters": Sequence[SessionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -5106,26 +4932,24 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
-
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
-
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
@@ -5163,15 +4987,15 @@
 )
 
 ListDocumentsRequestListDocumentsPaginateTypeDef = TypedDict(
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     {
         "DocumentFilterList": Sequence[DocumentFilterTypeDef],
         "Filters": Sequence[DocumentKeyValuesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
@@ -5205,25 +5029,23 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
-
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
-
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EffectivePatchTypeDef = TypedDict(
     "EffectivePatchTypeDef",
     {
         "Patch": PatchTypeDef,
@@ -5244,22 +5066,20 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
-
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5277,29 +5097,27 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetInventoryRequestRequestTypeDef = TypedDict(
     "GetInventoryRequestRequestTypeDef",
     {
@@ -5328,15 +5146,15 @@
 GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef = TypedDict(
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     {
         "SyncName": str,
         "Filters": Sequence[OpsFilterTypeDef],
         "Aggregators": Sequence["OpsAggregatorTypeDef"],
         "ResultAttributes": Sequence[OpsResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetOpsSummaryRequestRequestTypeDef = TypedDict(
     "GetOpsSummaryRequestRequestTypeDef",
     {
@@ -5350,58 +5168,59 @@
     total=False,
 )
 
 GetParameterResultTypeDef = TypedDict(
     "GetParameterResultTypeDef",
     {
         "Parameter": ParameterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersByPathResultTypeDef = TypedDict(
     "GetParametersByPathResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersResultTypeDef = TypedDict(
     "GetParametersResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PatchSourceUnionTypeDef = Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceSettingResultTypeDef = TypedDict(
     "GetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetServiceSettingResultTypeDef = TypedDict(
     "ResetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceInformationTypeDef = TypedDict(
     "InstanceInformationTypeDef",
     {
         "InstanceId": str,
@@ -5467,21 +5286,19 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
-
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
-
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5495,15 +5312,15 @@
     total=False,
 )
 
 ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef = TypedDict(
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     {
         "Filters": Sequence[OpsItemEventFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemEventsRequestRequestTypeDef = TypedDict(
     "ListOpsItemEventsRequestRequestTypeDef",
     {
@@ -5515,15 +5332,15 @@
 )
 
 ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     {
         "OpsItemId": str,
         "Filters": Sequence[OpsItemRelatedItemsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemRelatedItemsRequestRequestTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     {
@@ -5535,15 +5352,15 @@
     total=False,
 )
 
 ListOpsMetadataRequestListOpsMetadataPaginateTypeDef = TypedDict(
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     {
         "Filters": Sequence[OpsMetadataFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsMetadataRequestRequestTypeDef = TypedDict(
     "ListOpsMetadataRequestRequestTypeDef",
     {
@@ -5555,18 +5372,41 @@
 )
 
 ListOpsMetadataResultTypeDef = TypedDict(
     "ListOpsMetadataResultTypeDef",
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersTypeDef",
+    {
+        "Comment": str,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "DocumentVersion": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ServiceRoleArn": str,
+        "TimeoutSeconds": int,
     },
+    total=False,
 )
 
+NotificationConfigUnionTypeDef = Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef]
+MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+]
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
@@ -5636,43 +5476,68 @@
         "Tier": ParameterTierType,
         "Policies": List[ParameterInlinePolicyTypeDef],
         "DataType": str,
     },
     total=False,
 )
 
+PatchFilterGroupOutputTypeDef = TypedDict(
+    "PatchFilterGroupOutputTypeDef",
+    {
+        "PatchFilters": List[PatchFilterOutputTypeDef],
+    },
+)
+
 PatchFilterGroupTypeDef = TypedDict(
     "PatchFilterGroupTypeDef",
     {
         "PatchFilters": Sequence[PatchFilterTypeDef],
     },
 )
 
+_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationSourceType": str,
+    },
+)
+_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
+    },
+    total=False,
+)
+
+class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
+    _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+    _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+):
+    pass
+
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
-
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
-
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5683,21 +5548,19 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
-
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5713,30 +5576,30 @@
 )
 
 DescribeActivationsResultTypeDef = TypedDict(
     "DescribeActivationsResultTypeDef",
     {
         "ActivationList": List[ActivationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationExecutionTypeDef = TypedDict(
     "AssociationExecutionTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "Status": str,
         "DetailedStatus": str,
         "CreatedTime": datetime,
         "LastExecutionDate": datetime,
         "ResourceCountByStatus": str,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
@@ -5744,135 +5607,114 @@
         "CommandId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "Comment": str,
         "ExpiresAfter": datetime,
         "Parameters": Dict[str, List[str]],
         "InstanceIds": List[str],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "RequestedDateTime": datetime,
         "Status": CommandStatusType,
         "StatusDetails": str,
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "TimeoutSeconds": int,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 GetMaintenanceWindowExecutionTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "TaskArn": str,
         "ServiceRole": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "TaskParameters": List[Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],
+        "TaskParameters": List[
+            Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]
+        ],
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 MaintenanceWindowTaskTypeDef = TypedDict(
     "MaintenanceWindowTaskTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "Targets": List[TargetTypeDef],
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "Targets": List[TargetOutputTypeDef],
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "Priority": int,
         "LoggingInfo": LoggingInfoTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredSendCommandRequestRequestTypeDef = TypedDict(
-    "_RequiredSendCommandRequestRequestTypeDef",
+TargetLocationOutputTypeDef = TypedDict(
+    "TargetLocationOutputTypeDef",
     {
-        "DocumentName": str,
-    },
-)
-_OptionalSendCommandRequestRequestTypeDef = TypedDict(
-    "_OptionalSendCommandRequestRequestTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "Targets": Sequence[TargetTypeDef],
-        "DocumentVersion": str,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "TimeoutSeconds": int,
-        "Comment": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "ServiceRoleArn": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "Accounts": List[str],
+        "Regions": List[str],
+        "TargetLocationMaxConcurrency": str,
+        "TargetLocationMaxErrors": str,
+        "ExecutionRoleName": str,
+        "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
-class SendCommandRequestRequestTypeDef(
-    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
-):
-    pass
-
-
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5883,62 +5725,100 @@
 )
 
 ListAssociationsResultTypeDef = TypedDict(
     "ListAssociationsResultTypeDef",
     {
         "Associations": List[AssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTargetsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     {
         "Targets": List[MaintenanceWindowTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionTargetsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionTargetsResultTypeDef",
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AssociationStatusUnionTypeDef = Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
+    },
+)
+
+ComplianceExecutionSummaryUnionTypeDef = Union[
+    ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
+]
+_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ComplianceType": str,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "Items": Sequence[ComplianceItemEntryTypeDef],
+    },
+)
+_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ItemContentHash": str,
+        "UploadType": ComplianceUploadTypeType,
+    },
+    total=False,
+)
+
+class PutComplianceItemsRequestRequestTypeDef(
+    _RequiredPutComplianceItemsRequestRequestTypeDef,
+    _OptionalPutComplianceItemsRequestRequestTypeDef,
+):
+    pass
+
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     {
-        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersTypeDef,
+        "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
         "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
         "ComplianceItems": List[ComplianceItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryItemTypeDef = TypedDict(
     "ComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
@@ -5952,77 +5832,232 @@
     "ResourceComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Status": ComplianceStatusType,
         "OverallSeverity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
+DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
+    TypedDict(
+        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+        {
+            "WindowId": str,
+            "Targets": Sequence[TargetUnionTypeDef],
+            "ResourceType": MaintenanceWindowResourceTypeType,
+            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetUnionTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSendCommandRequestRequestTypeDef = TypedDict(
+    "_RequiredSendCommandRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalSendCommandRequestRequestTypeDef = TypedDict(
+    "_OptionalSendCommandRequestRequestTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "DocumentVersion": str,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "TimeoutSeconds": int,
+        "Comment": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "ServiceRoleArn": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class SendCommandRequestRequestTypeDef(
+    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOpsItemsResponseTypeDef = TypedDict(
     "DescribeOpsItemsResponseTypeDef",
     {
         "NextToken": str,
         "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOpsItemResponseTypeDef = TypedDict(
     "GetOpsItemResponseTypeDef",
     {
         "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePatchGroupsResultTypeDef = TypedDict(
     "DescribePatchGroupsResultTypeDef",
     {
         "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDocumentResultTypeDef = TypedDict(
     "DescribeDocumentResultTypeDef",
     {
         "Document": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDocumentResultTypeDef = TypedDict(
     "UpdateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataResponseInfoTypeDef = TypedDict(
     "DocumentMetadataResponseInfoTypeDef",
     {
         "ReviewerResponse": List[DocumentReviewerResponseSourceTypeDef],
@@ -6041,28 +6076,26 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
-
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryAggregatorTypeDef = TypedDict(
     "InventoryAggregatorTypeDef",
     {
         "Expression": str,
@@ -6073,15 +6106,15 @@
 )
 
 DescribeInstanceInformationResultTypeDef = TypedDict(
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": str,
@@ -6102,15 +6135,15 @@
 
 DeleteInventoryResultTypeDef = TypedDict(
     "DeleteInventoryResultTypeDef",
     {
         "DeletionId": str,
         "TypeName": str,
         "DeletionSummary": InventoryDeletionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDeletionStatusItemTypeDef = TypedDict(
     "InventoryDeletionStatusItemTypeDef",
     {
         "DeletionId": str,
@@ -6125,72 +6158,104 @@
 )
 
 GetInventorySchemaResultTypeDef = TypedDict(
     "GetInventorySchemaResultTypeDef",
     {
         "Schemas": List[InventoryItemSchemaTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInventoryResultTypeDef = TypedDict(
     "GetInventoryResultTypeDef",
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    {
+        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
     },
+    total=False,
 )
 
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemRelatedItemsResponseTypeDef = TypedDict(
     "ListOpsItemRelatedItemsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParametersResultTypeDef = TypedDict(
     "DescribeParametersResultTypeDef",
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPatchRuleOutputTypeDef = TypedDict(
+    "_RequiredPatchRuleOutputTypeDef",
+    {
+        "PatchFilterGroup": PatchFilterGroupOutputTypeDef,
+    },
+)
+_OptionalPatchRuleOutputTypeDef = TypedDict(
+    "_OptionalPatchRuleOutputTypeDef",
+    {
+        "ComplianceLevel": PatchComplianceLevelType,
+        "ApproveAfterDays": int,
+        "ApproveUntilDate": str,
+        "EnableNonSecurity": bool,
     },
+    total=False,
 )
 
+class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
+    pass
+
+PatchFilterGroupUnionTypeDef = Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef]
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -6200,18 +6265,29 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
-
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
+ResourceDataSyncSourceWithStateTypeDef = TypedDict(
+    "ResourceDataSyncSourceWithStateTypeDef",
+    {
+        "SourceType": str,
+        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+        "SourceRegions": List[str],
+        "IncludeFutureRegions": bool,
+        "State": str,
+        "EnableAllOpsDataSources": bool,
+    },
+    total=False,
+)
 
 _RequiredResourceDataSyncSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncSourceTypeDef",
     {
         "SourceType": str,
         "SourceRegions": Sequence[str],
     },
@@ -6222,285 +6298,194 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
-
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
-
-ResourceDataSyncSourceWithStateTypeDef = TypedDict(
-    "ResourceDataSyncSourceWithStateTypeDef",
-    {
-        "SourceType": str,
-        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
-        "SourceRegions": List[str],
-        "IncludeFutureRegions": bool,
-        "State": str,
-        "EnableAllOpsDataSources": bool,
-    },
-    total=False,
-)
-
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionsResultTypeDef",
     {
         "AssociationExecutions": List[AssociationExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandsResultTypeDef = TypedDict(
     "ListCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "Command": CommandTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     {
         "WindowExecutionTaskIdentities": List[MaintenanceWindowExecutionTaskIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTasksResultTypeDef",
     {
         "Tasks": List[MaintenanceWindowTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationDescriptionTypeDef = TypedDict(
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationVersion": str,
         "Date": datetime,
         "LastUpdateAssociationDate": datetime,
-        "Status": AssociationStatusTypeDef,
+        "Status": AssociationStatusOutputTypeDef,
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 AssociationVersionInfoTypeDef = TypedDict(
     "AssociationVersionInfoTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
-_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
+_RequiredCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
+_OptionalCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryOutputTypeDef",
     {
         "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
+        "Parameters": Dict[str, List[str]],
         "AutomationTargetParameterName": str,
         "DocumentVersion": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAssociationBatchRequestEntryTypeDef(
-    _RequiredCreateAssociationBatchRequestEntryTypeDef,
-    _OptionalCreateAssociationBatchRequestEntryTypeDef,
-):
-    pass
-
-
-_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssociationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssociationRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[TargetTypeDef],
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "AssociationName": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "CalendarNames": List[str],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "TargetMaps": List[Dict[str, List[str]]],
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
-class CreateAssociationRequestRequestTypeDef(
-    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+class CreateAssociationBatchRequestEntryOutputTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
 ):
     pass
 
-
-_RequiredRunbookTypeDef = TypedDict(
-    "_RequiredRunbookTypeDef",
+_RequiredRunbookOutputTypeDef = TypedDict(
+    "_RequiredRunbookOutputTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalRunbookTypeDef = TypedDict(
-    "_OptionalRunbookTypeDef",
+_OptionalRunbookOutputTypeDef = TypedDict(
+    "_OptionalRunbookOutputTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
     },
     total=False,
 )
 
-
-class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
+class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
     pass
 
-
-_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ClientToken": str,
-        "Mode": ExecutionModeType,
-        "TargetParameterName": str,
-        "Targets": Sequence[TargetTypeDef],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class StartAutomationExecutionRequestRequestTypeDef(
-    _RequiredStartAutomationExecutionRequestRequestTypeDef,
-    _OptionalStartAutomationExecutionRequestRequestTypeDef,
-):
-    pass
-
-
 StepExecutionTypeDef = TypedDict(
     "StepExecutionTypeDef",
     {
         "StepName": str,
         "Action": str,
         "TimeoutSeconds": int,
         "OnFailure": str,
@@ -6516,232 +6501,279 @@
         "FailureDetails": FailureDetailsTypeDef,
         "StepExecutionId": str,
         "OverriddenParameters": Dict[str, List[str]],
         "IsEnd": bool,
         "NextStep": str,
         "IsCritical": bool,
         "ValidNextSteps": List[str],
-        "Targets": List[TargetTypeDef],
-        "TargetLocation": TargetLocationTypeDef,
+        "Targets": List[TargetOutputTypeDef],
+        "TargetLocation": TargetLocationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAssociationRequestRequestTypeDef",
+_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
     {
-        "AssociationId": str,
+        "Name": str,
     },
 )
-_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAssociationRequestRequestTypeDef",
+_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
     {
+        "InstanceId": str,
         "Parameters": Mapping[str, Sequence[str]],
+        "AutomationTargetParameterName": str,
         "DocumentVersion": str,
+        "Targets": Sequence[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "Name": str,
-        "Targets": Sequence[TargetTypeDef],
         "AssociationName": str,
-        "AssociationVersion": str,
-        "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
         "TargetLocations": Sequence[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class UpdateAssociationRequestRequestTypeDef(
-    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
+class CreateAssociationBatchRequestEntryTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
-
-GetMaintenanceWindowTaskResultTypeDef = TypedDict(
-    "GetMaintenanceWindowTaskResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
-        "TaskArn": str,
-        "ServiceRoleArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+_RequiredRunbookTypeDef = TypedDict(
+    "_RequiredRunbookTypeDef",
     {
-        "WindowId": str,
-        "TaskArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
+        "DocumentName": str,
     },
 )
-_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+_OptionalRunbookTypeDef = TypedDict(
+    "_OptionalRunbookTypeDef",
     {
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "TargetParameterName": str,
         "Targets": Sequence[TargetTypeDef],
-        "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "TargetLocations": Sequence[TargetLocationTypeDef],
     },
     total=False,
 )
 
-
-class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-):
+class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
-
-_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+TargetLocationUnionTypeDef = Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]
+GetMaintenanceWindowTaskResultTypeDef = TypedDict(
+    "GetMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
-        "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceSummariesResultTypeDef = TypedDict(
     "ListComplianceSummariesResultTypeDef",
     {
         "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceComplianceSummariesResultTypeDef = TypedDict(
     "ListResourceComplianceSummariesResultTypeDef",
     {
         "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
     "ListDocumentMetadataHistoryResponseTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
         "Author": str,
         "Metadata": DocumentMetadataResponseInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
     "DescribeInstanceAssociationsStatusResultTypeDef",
     {
         "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInventoryDeletionsResultTypeDef = TypedDict(
     "DescribeInventoryDeletionsResultTypeDef",
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
+    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+]
+_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "TaskArn": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+    },
+)
+_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ServiceRoleArn": str,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTaskId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "TaskArn": str,
+        "ServiceRoleArn": str,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+):
+    pass
+
+PatchRuleGroupOutputTypeDef = TypedDict(
+    "PatchRuleGroupOutputTypeDef",
+    {
+        "PatchRules": List[PatchRuleOutputTypeDef],
     },
 )
 
 PatchRuleGroupTypeDef = TypedDict(
     "PatchRuleGroupTypeDef",
     {
         "PatchRules": Sequence[PatchRuleTypeDef],
     },
 )
 
+ResourceDataSyncItemTypeDef = TypedDict(
+    "ResourceDataSyncItemTypeDef",
+    {
+        "SyncName": str,
+        "SyncType": str,
+        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
+        "LastSyncTime": datetime,
+        "LastSuccessfulSyncTime": datetime,
+        "SyncLastModifiedTime": datetime,
+        "LastStatus": LastResourceDataSyncStatusType,
+        "SyncCreatedTime": datetime,
+        "LastSyncStatusMessage": str,
+    },
+    total=False,
+)
+
 _RequiredCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
@@ -6750,100 +6782,74 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
-
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
 )
 
-ResourceDataSyncItemTypeDef = TypedDict(
-    "ResourceDataSyncItemTypeDef",
-    {
-        "SyncName": str,
-        "SyncType": str,
-        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
-        "LastSyncTime": datetime,
-        "LastSuccessfulSyncTime": datetime,
-        "SyncLastModifiedTime": datetime,
-        "LastStatus": LastResourceDataSyncStatusType,
-        "SyncCreatedTime": datetime,
-        "LastSyncStatusMessage": str,
-    },
-    total=False,
-)
-
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationResultTypeDef = TypedDict(
     "DescribeAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationResultTypeDef = TypedDict(
     "UpdateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationStatusResultTypeDef = TypedDict(
     "UpdateAssociationStatusResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociationVersionsResultTypeDef = TypedDict(
     "ListAssociationVersionsResultTypeDef",
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
-    {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedCreateAssociationTypeDef = TypedDict(
     "FailedCreateAssociationTypeDef",
     {
-        "Entry": CreateAssociationBatchRequestEntryTypeDef,
+        "Entry": CreateAssociationBatchRequestEntryOutputTypeDef,
         "Message": str,
         "Fault": FaultType,
     },
     total=False,
 )
 
 AutomationExecutionMetadataTypeDef = TypedDict(
@@ -6860,64 +6866,33 @@
         "Outputs": Dict[str, List[str]],
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "FailureMessage": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
         "AutomationType": AutomationTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-        "Runbooks": Sequence[RunbookTypeDef],
-    },
-)
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "ScheduledTime": Union[datetime, str],
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
-        "ClientToken": str,
-        "AutoApprove": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": Union[datetime, str],
-        "ChangeDetails": str,
-    },
-    total=False,
-)
-
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
-):
-    pass
-
-
 AutomationExecutionTypeDef = TypedDict(
     "AutomationExecutionTypeDef",
     {
         "AutomationExecutionId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "ExecutionStartTime": datetime,
@@ -6930,40 +6905,192 @@
         "FailureMessage": str,
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "ExecutedBy": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ProgressCounters": ProgressCountersTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
 DescribeAutomationStepExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationStepExecutionsResultTypeDef",
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssociationBatchRequestEntryUnionTypeDef = Union[
+    CreateAssociationBatchRequestEntryTypeDef, CreateAssociationBatchRequestEntryOutputTypeDef
+]
+RunbookUnionTypeDef = Union[RunbookTypeDef, RunbookOutputTypeDef]
+_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssociationRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssociationRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "InstanceId": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "AssociationName": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateAssociationRequestRequestTypeDef(
+    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+):
+    pass
+
+_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ClientToken": str,
+        "Mode": ExecutionModeType,
+        "TargetParameterName": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class StartAutomationExecutionRequestRequestTypeDef(
+    _RequiredStartAutomationExecutionRequestRequestTypeDef,
+    _OptionalStartAutomationExecutionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAssociationRequestRequestTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAssociationRequestRequestTypeDef",
+    {
+        "Parameters": Mapping[str, Sequence[str]],
+        "DocumentVersion": str,
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "Name": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "AssociationName": str,
+        "AssociationVersion": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateAssociationRequestRequestTypeDef(
+    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
+):
+    pass
+
+GetPatchBaselineResultTypeDef = TypedDict(
+    "GetPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "PatchGroups": List[str],
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePatchBaselineResultTypeDef = TypedDict(
+    "UpdatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
@@ -6993,51 +7120,28 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
-GetPatchBaselineResultTypeDef = TypedDict(
-    "GetPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "PatchGroups": List[str],
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+PatchRuleGroupUnionTypeDef = Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef]
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -7048,84 +7152,97 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
-
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-
-UpdatePatchBaselineResultTypeDef = TypedDict(
-    "UpdatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssociationBatchResultTypeDef = TypedDict(
     "CreateAssociationBatchResultTypeDef",
     {
         "Successful": List[AssociationDescriptionTypeDef],
         "Failed": List[FailedCreateAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAutomationExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationExecutionsResultTypeDef",
     {
         "AutomationExecutionMetadataList": List[AutomationExecutionMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutomationExecutionResultTypeDef = TypedDict(
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],
+    },
+)
+
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookUnionTypeDef],
+    },
+)
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": TimestampTypeDef,
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": TimestampTypeDef,
+        "ChangeDetails": str,
     },
+    total=False,
 )
 
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SnapshotId": str,
     },
 )
@@ -7133,13 +7250,12 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
-
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/type_defs.pyi` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ssm.type_defs import AccountSharingInfoTypeDef
 
-    data: AccountSharingInfoTypeDef = {...}
+    data: AccountSharingInfoTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from aiobotocore.response import StreamingBody
 
 from .literals import (
     AssociationComplianceSeverityType,
     AssociationExecutionFilterKeyType,
     AssociationExecutionTargetsFilterKeyType,
     AssociationFilterKeyType,
     AssociationFilterOperatorTypeType,
@@ -99,298 +101,304 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountSharingInfoTypeDef",
     "TagTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
-    "AssociationStatusTypeDef",
-    "TargetTypeDef",
+    "AssociationStatusOutputTypeDef",
+    "TargetOutputTypeDef",
     "AssociationExecutionFilterTypeDef",
     "OutputSourceTypeDef",
     "AssociationExecutionTargetsFilterTypeDef",
     "AssociationFilterTypeDef",
+    "TimestampTypeDef",
     "AttachmentContentTypeDef",
     "AttachmentInformationTypeDef",
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
+    "BlobTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
-    "CancelMaintenanceWindowExecutionResultTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
-    "NotificationConfigTypeDef",
-    "ComplianceExecutionSummaryTypeDef",
+    "NotificationConfigOutputTypeDef",
+    "ComplianceExecutionSummaryOutputTypeDef",
     "ComplianceItemEntryTypeDef",
     "ComplianceStringFilterTypeDef",
     "SeveritySummaryTypeDef",
     "RegistrationMetadataItemTypeDef",
-    "CreateActivationResultTypeDef",
+    "TargetTypeDef",
     "DocumentRequiresTypeDef",
-    "CreateMaintenanceWindowResultTypeDef",
     "OpsItemDataValueTypeDef",
     "OpsItemNotificationTypeDef",
     "RelatedOpsItemTypeDef",
-    "CreateOpsItemResponseTypeDef",
     "MetadataValueTypeDef",
-    "CreateOpsMetadataResultTypeDef",
-    "CreatePatchBaselineResultTypeDef",
     "DeleteActivationRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteInventoryRequestRequestTypeDef",
     "DeleteMaintenanceWindowRequestRequestTypeDef",
-    "DeleteMaintenanceWindowResultTypeDef",
     "DeleteOpsMetadataRequestRequestTypeDef",
     "DeleteParameterRequestRequestTypeDef",
     "DeleteParametersRequestRequestTypeDef",
-    "DeleteParametersResultTypeDef",
     "DeletePatchBaselineRequestRequestTypeDef",
-    "DeletePatchBaselineResultTypeDef",
     "DeleteResourceDataSyncRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeregisterManagedInstanceRequestRequestTypeDef",
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
     "DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     "DescribeActivationsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAssociationRequestRequestTypeDef",
     "StepExecutionFilterTypeDef",
     "PatchOrchestratorFilterTypeDef",
     "PatchTypeDef",
     "DescribeDocumentPermissionRequestRequestTypeDef",
     "DescribeDocumentRequestRequestTypeDef",
-    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     "InstanceAssociationTypeDef",
-    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
     "DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
-    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
-    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
     "OpsItemFilterTypeDef",
     "ParameterStringFilterTypeDef",
     "ParametersFilterTypeDef",
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
-    "DescribePatchGroupStateResultTypeDef",
-    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
-    "DescribePatchPropertiesResultTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
-    "GetCalendarStateResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetCommandInvocationRequestRequestTypeDef",
     "GetConnectionStatusRequestRequestTypeDef",
-    "GetConnectionStatusResponseTypeDef",
     "GetDefaultPatchBaselineRequestRequestTypeDef",
-    "GetDefaultPatchBaselineResultTypeDef",
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "InventoryFilterTypeDef",
     "ResultAttributeTypeDef",
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionResultTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
-    "GetMaintenanceWindowResultTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
-    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "GetPatchBaselineForPatchGroupResultTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
-    "LabelParameterVersionResultTypeDef",
-    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
     "ListAssociationVersionsRequestRequestTypeDef",
     "ListDocumentMetadataHistoryRequestRequestTypeDef",
-    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
     "ListDocumentVersionsRequestRequestTypeDef",
-    "ListInventoryEntriesResultTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
-    "MaintenanceWindowLambdaParametersTypeDef",
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
+    "NotificationConfigTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
     "OpsItemIdentityTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterInlinePolicyTypeDef",
+    "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
-    "PutInventoryResultTypeDef",
-    "PutParameterResultTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
-    "RegisterDefaultPatchBaselineResultTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeSessionRequestRequestTypeDef",
-    "ResumeSessionResponseTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
-    "StartAutomationExecutionResultTypeDef",
-    "StartChangeRequestExecutionResultTypeDef",
     "StartSessionRequestRequestTypeDef",
-    "StartSessionResponseTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UnlabelParameterVersionRequestRequestTypeDef",
-    "UnlabelParameterVersionResultTypeDef",
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     "UpdateMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowResultTypeDef",
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
-    "UpdateOpsMetadataResultTypeDef",
     "UpdateServiceSettingRequestRequestTypeDef",
-    "DescribeDocumentPermissionResponseTypeDef",
     "ActivationTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateMaintenanceWindowRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "PutParameterRequestRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
-    "UpdateAssociationStatusRequestRequestTypeDef",
+    "AssociateOpsItemRelatedItemResponseTypeDef",
+    "CancelMaintenanceWindowExecutionResultTypeDef",
+    "CreateActivationResultTypeDef",
+    "CreateMaintenanceWindowResultTypeDef",
+    "CreateOpsItemResponseTypeDef",
+    "CreateOpsMetadataResultTypeDef",
+    "CreatePatchBaselineResultTypeDef",
+    "DeleteMaintenanceWindowResultTypeDef",
+    "DeleteParametersResultTypeDef",
+    "DeletePatchBaselineResultTypeDef",
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
+    "DescribeDocumentPermissionResponseTypeDef",
+    "DescribePatchGroupStateResultTypeDef",
+    "DescribePatchPropertiesResultTypeDef",
+    "GetCalendarStateResponseTypeDef",
+    "GetConnectionStatusResponseTypeDef",
+    "GetDefaultPatchBaselineResultTypeDef",
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    "GetMaintenanceWindowResultTypeDef",
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    "LabelParameterVersionResultTypeDef",
+    "ListInventoryEntriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "PutInventoryResultTypeDef",
+    "PutParameterResultTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
+    "ResumeSessionResponseTypeDef",
+    "StartAutomationExecutionResultTypeDef",
+    "StartChangeRequestExecutionResultTypeDef",
+    "StartSessionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
+    "UnlabelParameterVersionResultTypeDef",
+    "UpdateMaintenanceWindowResultTypeDef",
+    "UpdateOpsMetadataResultTypeDef",
     "AssociationTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
-    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "MaintenanceWindowTargetTypeDef",
-    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetResultTypeDef",
-    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestRequestTypeDef",
     "AssociationExecutionTargetTypeDef",
-    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestRequestTypeDef",
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
     "ListAssociationsRequestRequestTypeDef",
+    "AssociationStatusTypeDef",
+    "ComplianceExecutionSummaryTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestRequestTypeDef",
+    "MaintenanceWindowLambdaParametersTypeDef",
     "GetCommandInvocationResultTypeDef",
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
     "ListCommandInvocationsRequestRequestTypeDef",
-    "ListCommandsRequestListCommandsPaginateTypeDef",
     "ListCommandsRequestRequestTypeDef",
     "CommandInvocationTypeDef",
-    "MaintenanceWindowRunCommandParametersTypeDef",
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     "ComplianceItemTypeDef",
-    "PutComplianceItemsRequestRequestTypeDef",
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
     "ListComplianceItemsRequestRequestTypeDef",
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
     "ListComplianceSummariesRequestRequestTypeDef",
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
+    "TargetUnionTypeDef",
     "CreateDocumentRequestRequestTypeDef",
     "DocumentIdentifierTypeDef",
     "GetDocumentResultTypeDef",
     "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
     "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
     "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
-    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     "DescribeActivationsRequestRequestTypeDef",
+    "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
+    "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    "DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    "DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    "DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    "DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    "GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    "ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     "DescribeAutomationStepExecutionsRequestRequestTypeDef",
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     "DescribeAvailablePatchesRequestRequestTypeDef",
     "DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     "DescribeInstancePatchesRequestRequestTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     "DescribePatchBaselinesRequestRequestTypeDef",
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     "DescribePatchGroupsRequestRequestTypeDef",
     "DescribeAvailablePatchesResultTypeDef",
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
@@ -442,14 +450,15 @@
     "GetInventoryRequestRequestTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
+    "PatchSourceUnionTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
@@ -459,39 +468,56 @@
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     "ListOpsItemEventsRequestRequestTypeDef",
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
+    "MaintenanceWindowRunCommandParametersTypeDef",
+    "NotificationConfigUnionTypeDef",
+    "MaintenanceWindowTaskParameterValueExpressionUnionTypeDef",
     "OpsEntityTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
+    "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
+    "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     "MaintenanceWindowTaskTypeDef",
-    "SendCommandRequestRequestTypeDef",
+    "TargetLocationOutputTypeDef",
+    "AlarmConfigurationUnionTypeDef",
     "TargetLocationTypeDef",
     "ListAssociationsResultTypeDef",
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
+    "AssociationStatusUnionTypeDef",
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    "ComplianceExecutionSummaryUnionTypeDef",
+    "PutComplianceItemsRequestRequestTypeDef",
     "ListCommandInvocationsResultTypeDef",
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    "SendCommandRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "ListDocumentsResultTypeDef",
     "DescribeOpsItemsResponseTypeDef",
     "GetOpsItemResponseTypeDef",
     "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
@@ -501,69 +527,80 @@
     "InventoryAggregatorTypeDef",
     "DescribeInstanceInformationResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
+    "PatchRuleOutputTypeDef",
+    "PatchFilterGroupUnionTypeDef",
     "PatchRuleTypeDef",
-    "ResourceDataSyncSourceTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
+    "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
     "DescribeAssociationExecutionsResultTypeDef",
     "ListCommandsResultTypeDef",
     "SendCommandResultTypeDef",
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     "DescribeMaintenanceWindowTasksResultTypeDef",
     "AssociationDescriptionTypeDef",
     "AssociationVersionInfoTypeDef",
+    "CreateAssociationBatchRequestEntryOutputTypeDef",
+    "RunbookOutputTypeDef",
+    "StepExecutionTypeDef",
     "CreateAssociationBatchRequestEntryTypeDef",
-    "CreateAssociationRequestRequestTypeDef",
     "RunbookTypeDef",
-    "StartAutomationExecutionRequestRequestTypeDef",
-    "StepExecutionTypeDef",
-    "UpdateAssociationRequestRequestTypeDef",
+    "TargetLocationUnionTypeDef",
     "GetMaintenanceWindowTaskResultTypeDef",
-    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
-    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
     "UpdateMaintenanceWindowTaskResultTypeDef",
     "ListComplianceSummariesResultTypeDef",
     "ListResourceComplianceSummariesResultTypeDef",
     "ListDocumentMetadataHistoryResponseTypeDef",
     "DescribeInstanceAssociationsStatusResultTypeDef",
     "DescribeInventoryDeletionsResultTypeDef",
+    "MaintenanceWindowTaskInvocationParametersUnionTypeDef",
+    "RegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    "UpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    "PatchRuleGroupOutputTypeDef",
     "PatchRuleGroupTypeDef",
+    "ResourceDataSyncItemTypeDef",
     "CreateResourceDataSyncRequestRequestTypeDef",
     "UpdateResourceDataSyncRequestRequestTypeDef",
-    "ResourceDataSyncItemTypeDef",
     "CreateAssociationResultTypeDef",
     "DescribeAssociationResultTypeDef",
     "UpdateAssociationResultTypeDef",
     "UpdateAssociationStatusResultTypeDef",
     "ListAssociationVersionsResultTypeDef",
-    "CreateAssociationBatchRequestRequestTypeDef",
     "FailedCreateAssociationTypeDef",
     "AutomationExecutionMetadataTypeDef",
-    "StartChangeRequestExecutionRequestRequestTypeDef",
     "AutomationExecutionTypeDef",
     "DescribeAutomationStepExecutionsResultTypeDef",
+    "CreateAssociationBatchRequestEntryUnionTypeDef",
+    "RunbookUnionTypeDef",
+    "CreateAssociationRequestRequestTypeDef",
+    "StartAutomationExecutionRequestRequestTypeDef",
+    "UpdateAssociationRequestRequestTypeDef",
+    "GetPatchBaselineResultTypeDef",
+    "UpdatePatchBaselineResultTypeDef",
     "BaselineOverrideTypeDef",
     "CreatePatchBaselineRequestRequestTypeDef",
-    "GetPatchBaselineResultTypeDef",
+    "PatchRuleGroupUnionTypeDef",
     "UpdatePatchBaselineRequestRequestTypeDef",
-    "UpdatePatchBaselineResultTypeDef",
     "ListResourceDataSyncResultTypeDef",
     "CreateAssociationBatchResultTypeDef",
     "DescribeAutomationExecutionsResultTypeDef",
     "GetAutomationExecutionResultTypeDef",
+    "CreateAssociationBatchRequestRequestTypeDef",
+    "StartChangeRequestExecutionRequestRequestTypeDef",
     "GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
 )
 
 AccountSharingInfoTypeDef = TypedDict(
     "AccountSharingInfoTypeDef",
     {
         "AccountId": str,
@@ -601,58 +638,63 @@
         "OpsItemId": str,
         "AssociationType": str,
         "ResourceType": str,
         "ResourceUri": str,
     },
 )
 
-AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
-    "AssociateOpsItemRelatedItemResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AssociationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociationOverviewTypeDef = TypedDict(
     "AssociationOverviewTypeDef",
     {
         "Status": str,
         "DetailedStatus": str,
         "AssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredAssociationStatusTypeDef = TypedDict(
-    "_RequiredAssociationStatusTypeDef",
+_RequiredAssociationStatusOutputTypeDef = TypedDict(
+    "_RequiredAssociationStatusOutputTypeDef",
     {
         "Date": datetime,
         "Name": AssociationStatusNameType,
         "Message": str,
     },
 )
-_OptionalAssociationStatusTypeDef = TypedDict(
-    "_OptionalAssociationStatusTypeDef",
+_OptionalAssociationStatusOutputTypeDef = TypedDict(
+    "_OptionalAssociationStatusOutputTypeDef",
     {
         "AdditionalInfo": str,
     },
     total=False,
 )
 
-class AssociationStatusTypeDef(
-    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+
+class AssociationStatusOutputTypeDef(
+    _RequiredAssociationStatusOutputTypeDef, _OptionalAssociationStatusOutputTypeDef
 ):
     pass
 
-TargetTypeDef = TypedDict(
-    "TargetTypeDef",
+
+TargetOutputTypeDef = TypedDict(
+    "TargetOutputTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
     total=False,
 )
 
 AssociationExecutionFilterTypeDef = TypedDict(
     "AssociationExecutionFilterTypeDef",
     {
@@ -683,14 +725,15 @@
     "AssociationFilterTypeDef",
     {
         "key": AssociationFilterKeyType,
         "value": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 AttachmentContentTypeDef = TypedDict(
     "AttachmentContentTypeDef",
     {
         "Name": str,
         "Size": int,
         "Hash": str,
         "HashType": Literal["Sha256"],
@@ -751,48 +794,43 @@
     {
         "Name": str,
         "Products": Sequence[str],
         "Configuration": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCancelCommandRequestRequestTypeDef = TypedDict(
     "_RequiredCancelCommandRequestRequestTypeDef",
     {
         "CommandId": str,
     },
 )
 _OptionalCancelCommandRequestRequestTypeDef = TypedDict(
     "_OptionalCancelCommandRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CancelCommandRequestRequestTypeDef(
     _RequiredCancelCommandRequestRequestTypeDef, _OptionalCancelCommandRequestRequestTypeDef
 ):
     pass
 
+
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "CancelMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
     },
     total=False,
@@ -821,44 +859,47 @@
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
     total=False,
 )
 
-NotificationConfigTypeDef = TypedDict(
-    "NotificationConfigTypeDef",
+NotificationConfigOutputTypeDef = TypedDict(
+    "NotificationConfigOutputTypeDef",
     {
         "NotificationArn": str,
         "NotificationEvents": List[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
-_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
-    "_RequiredComplianceExecutionSummaryTypeDef",
+_RequiredComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryOutputTypeDef",
     {
         "ExecutionTime": datetime,
     },
 )
-_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
-    "_OptionalComplianceExecutionSummaryTypeDef",
+_OptionalComplianceExecutionSummaryOutputTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryOutputTypeDef",
     {
         "ExecutionId": str,
         "ExecutionType": str,
     },
     total=False,
 )
 
-class ComplianceExecutionSummaryTypeDef(
-    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
+
+class ComplianceExecutionSummaryOutputTypeDef(
+    _RequiredComplianceExecutionSummaryOutputTypeDef,
+    _OptionalComplianceExecutionSummaryOutputTypeDef,
 ):
     pass
 
+
 _RequiredComplianceItemEntryTypeDef = TypedDict(
     "_RequiredComplianceItemEntryTypeDef",
     {
         "Severity": ComplianceSeverityType,
         "Status": ComplianceStatusType,
     },
 )
@@ -868,19 +909,21 @@
         "Id": str,
         "Title": str,
         "Details": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ComplianceItemEntryTypeDef(
     _RequiredComplianceItemEntryTypeDef, _OptionalComplianceItemEntryTypeDef
 ):
     pass
 
+
 ComplianceStringFilterTypeDef = TypedDict(
     "ComplianceStringFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "Type": ComplianceQueryOperatorTypeType,
     },
@@ -904,21 +947,21 @@
     "RegistrationMetadataItemTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateActivationResultTypeDef = TypedDict(
-    "CreateActivationResultTypeDef",
+TargetTypeDef = TypedDict(
+    "TargetTypeDef",
     {
-        "ActivationId": str,
-        "ActivationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Values": Sequence[str],
     },
+    total=False,
 )
 
 _RequiredDocumentRequiresTypeDef = TypedDict(
     "_RequiredDocumentRequiresTypeDef",
     {
         "Name": str,
     },
@@ -929,24 +972,18 @@
         "Version": str,
         "RequireType": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DocumentRequiresTypeDef(_RequiredDocumentRequiresTypeDef, _OptionalDocumentRequiresTypeDef):
     pass
 
-CreateMaintenanceWindowResultTypeDef = TypedDict(
-    "CreateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 OpsItemDataValueTypeDef = TypedDict(
     "OpsItemDataValueTypeDef",
     {
         "Value": str,
         "Type": OpsItemDataTypeType,
     },
@@ -964,47 +1001,22 @@
 RelatedOpsItemTypeDef = TypedDict(
     "RelatedOpsItemTypeDef",
     {
         "OpsItemId": str,
     },
 )
 
-CreateOpsItemResponseTypeDef = TypedDict(
-    "CreateOpsItemResponseTypeDef",
-    {
-        "OpsItemId": str,
-        "OpsItemArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetadataValueTypeDef = TypedDict(
     "MetadataValueTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-CreateOpsMetadataResultTypeDef = TypedDict(
-    "CreateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePatchBaselineResultTypeDef = TypedDict(
-    "CreatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivationRequestRequestTypeDef = TypedDict(
     "DeleteActivationRequestRequestTypeDef",
     {
         "ActivationId": str,
     },
 )
 
@@ -1030,19 +1042,21 @@
         "DocumentVersion": str,
         "VersionName": str,
         "Force": bool,
     },
     total=False,
 )
 
+
 class DeleteDocumentRequestRequestTypeDef(
     _RequiredDeleteDocumentRequestRequestTypeDef, _OptionalDeleteDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteInventoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteInventoryRequestRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalDeleteInventoryRequestRequestTypeDef = TypedDict(
@@ -1051,34 +1065,28 @@
         "SchemaDeleteOption": InventorySchemaDeleteOptionType,
         "DryRun": bool,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteInventoryRequestRequestTypeDef(
     _RequiredDeleteInventoryRequestRequestTypeDef, _OptionalDeleteInventoryRequestRequestTypeDef
 ):
     pass
 
+
 DeleteMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeleteMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-DeleteMaintenanceWindowResultTypeDef = TypedDict(
-    "DeleteMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteOpsMetadataRequestRequestTypeDef = TypedDict(
     "DeleteOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 
@@ -1092,58 +1100,43 @@
 DeleteParametersRequestRequestTypeDef = TypedDict(
     "DeleteParametersRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
-DeleteParametersResultTypeDef = TypedDict(
-    "DeleteParametersResultTypeDef",
-    {
-        "DeletedParameters": List[str],
-        "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeletePatchBaselineRequestRequestTypeDef = TypedDict(
     "DeletePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-DeletePatchBaselineResultTypeDef = TypedDict(
-    "DeletePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalDeleteResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
     },
     total=False,
 )
 
+
 class DeleteResourceDataSyncRequestRequestTypeDef(
     _RequiredDeleteResourceDataSyncRequestRequestTypeDef,
     _OptionalDeleteResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "PolicyId": str,
         "PolicyHash": str,
     },
@@ -1160,23 +1153,14 @@
     "DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
     },
 )
@@ -1184,55 +1168,49 @@
     "_OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef",
     {
         "Safe": bool,
     },
     total=False,
 )
 
+
 class DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef(
     _RequiredDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
     _OptionalDeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
-    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeActivationsFilterTypeDef = TypedDict(
     "DescribeActivationsFilterTypeDef",
     {
         "FilterKey": DescribeActivationsFilterKeysType,
         "FilterValues": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeAssociationRequestRequestTypeDef = TypedDict(
     "DescribeAssociationRequestRequestTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationId": str,
         "AssociationVersion": str,
@@ -1299,20 +1277,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentPermissionRequestRequestTypeDef(
     _RequiredDescribeDocumentPermissionRequestRequestTypeDef,
     _OptionalDescribeDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeDocumentRequestRequestTypeDef = TypedDict(
@@ -1320,38 +1300,20 @@
     {
         "DocumentVersion": str,
         "VersionName": str,
     },
     total=False,
 )
 
+
 class DescribeDocumentRequestRequestTypeDef(
     _RequiredDescribeDocumentRequestRequestTypeDef, _OptionalDescribeDocumentRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
-    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
@@ -1360,51 +1322,33 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectiveInstanceAssociationsRequestRequestTypeDef(
     _RequiredDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     _OptionalDescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceAssociationTypeDef = TypedDict(
     "InstanceAssociationTypeDef",
     {
         "AssociationId": str,
         "InstanceId": str,
         "Content": str,
         "AssociationVersion": str,
     },
     total=False,
 )
 
-_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "BaselineId": str,
-    },
-)
-_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
-    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
-    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef = TypedDict(
@@ -1412,39 +1356,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef(
     _RequiredDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
     _OptionalDescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
-    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
@@ -1453,20 +1379,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeInstanceAssociationsStatusRequestRequestTypeDef(
     _RequiredDescribeInstanceAssociationsStatusRequestRequestTypeDef,
     _OptionalDescribeInstanceAssociationsStatusRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceInformationFilterTypeDef = TypedDict(
     "InstanceInformationFilterTypeDef",
     {
         "key": InstanceInformationFilterKeyType,
         "valueSet": Sequence[str],
     },
 )
@@ -1518,38 +1446,20 @@
         "CriticalNonCompliantCount": int,
         "SecurityNonCompliantCount": int,
         "OtherNonCompliantCount": int,
     },
     total=False,
 )
 
+
 class InstancePatchStateTypeDef(
     _RequiredInstancePatchStateTypeDef, _OptionalInstancePatchStateTypeDef
 ):
     pass
 
-_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-    },
-)
-_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
-    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeInstancePatchStatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesRequestRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
     },
 )
@@ -1558,20 +1468,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPatchComplianceDataTypeDef = TypedDict(
     "_RequiredPatchComplianceDataTypeDef",
     {
         "Title": str,
         "KBId": str,
         "Classification": str,
         "Severity": str,
@@ -1583,27 +1495,20 @@
     "_OptionalPatchComplianceDataTypeDef",
     {
         "CVEIds": str,
     },
     total=False,
 )
 
+
 class PatchComplianceDataTypeDef(
     _RequiredPatchComplianceDataTypeDef, _OptionalPatchComplianceDataTypeDef
 ):
     pass
 
-DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
-    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
-    {
-        "DeletionId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": str,
         "NextToken": str,
         "MaxResults": int,
@@ -1710,19 +1615,21 @@
     {
         "Option": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
+
 class ParameterStringFilterTypeDef(
     _RequiredParameterStringFilterTypeDef, _OptionalParameterStringFilterTypeDef
 ):
     pass
 
+
 ParametersFilterTypeDef = TypedDict(
     "ParametersFilterTypeDef",
     {
         "Key": ParametersFilterKeyType,
         "Values": Sequence[str],
     },
 )
@@ -1742,55 +1649,14 @@
 DescribePatchGroupStateRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupStateRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 
-DescribePatchGroupStateResultTypeDef = TypedDict(
-    "DescribePatchGroupStateResultTypeDef",
-    {
-        "Instances": int,
-        "InstancesWithInstalledPatches": int,
-        "InstancesWithInstalledOtherPatches": int,
-        "InstancesWithInstalledPendingRebootPatches": int,
-        "InstancesWithInstalledRejectedPatches": int,
-        "InstancesWithMissingPatches": int,
-        "InstancesWithFailedPatches": int,
-        "InstancesWithNotApplicablePatches": int,
-        "InstancesWithUnreportedNotApplicablePatches": int,
-        "InstancesWithCriticalNonCompliantPatches": int,
-        "InstancesWithSecurityNonCompliantPatches": int,
-        "InstancesWithOtherNonCompliantPatches": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "OperatingSystem": OperatingSystemType,
-        "Property": PatchPropertyType,
-    },
-)
-_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
-    {
-        "PatchSet": PatchSetType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
-    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribePatchPropertiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribePatchPropertiesRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
         "Property": PatchPropertyType,
     },
 )
@@ -1800,28 +1666,21 @@
         "PatchSet": PatchSetType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribePatchPropertiesRequestRequestTypeDef(
     _RequiredDescribePatchPropertiesRequestRequestTypeDef,
     _OptionalDescribePatchPropertiesRequestRequestTypeDef,
 ):
     pass
 
-DescribePatchPropertiesResultTypeDef = TypedDict(
-    "DescribePatchPropertiesResultTypeDef",
-    {
-        "Properties": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SessionFilterTypeDef = TypedDict(
     "SessionFilterTypeDef",
     {
         "key": SessionFilterKeyType,
         "value": str,
     },
@@ -1946,28 +1805,20 @@
     "_OptionalGetCalendarStateRequestRequestTypeDef",
     {
         "AtTime": str,
     },
     total=False,
 )
 
+
 class GetCalendarStateRequestRequestTypeDef(
     _RequiredGetCalendarStateRequestRequestTypeDef, _OptionalGetCalendarStateRequestRequestTypeDef
 ):
     pass
 
-GetCalendarStateResponseTypeDef = TypedDict(
-    "GetCalendarStateResponseTypeDef",
-    {
-        "State": CalendarStateType,
-        "AtTime": str,
-        "NextTransitionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
@@ -1985,64 +1836,37 @@
     "_OptionalGetCommandInvocationRequestRequestTypeDef",
     {
         "PluginName": str,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestRequestTypeDef(
     _RequiredGetCommandInvocationRequestRequestTypeDef,
     _OptionalGetCommandInvocationRequestRequestTypeDef,
 ):
     pass
 
+
 GetConnectionStatusRequestRequestTypeDef = TypedDict(
     "GetConnectionStatusRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 
-GetConnectionStatusResponseTypeDef = TypedDict(
-    "GetConnectionStatusResponseTypeDef",
-    {
-        "Target": str,
-        "Status": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetDefaultPatchBaselineRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
-GetDefaultPatchBaselineResultTypeDef = TypedDict(
-    "GetDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
-    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
-    {
-        "InstanceId": str,
-        "SnapshotId": str,
-        "SnapshotDownloadUrl": str,
-        "Product": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDocumentRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDocumentRequestRequestTypeDef = TypedDict(
@@ -2051,19 +1875,21 @@
         "VersionName": str,
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
     },
     total=False,
 )
 
+
 class GetDocumentRequestRequestTypeDef(
     _RequiredGetDocumentRequestRequestTypeDef, _OptionalGetDocumentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredInventoryFilterTypeDef = TypedDict(
     "_RequiredInventoryFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2071,35 +1897,26 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Type": InventoryQueryOperatorTypeType,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 ResultAttributeTypeDef = TypedDict(
     "ResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
-    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
-    {
-        "TypeName": str,
-        "Aggregator": bool,
-        "SubType": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInventorySchemaRequestRequestTypeDef = TypedDict(
     "GetInventorySchemaRequestRequestTypeDef",
     {
         "TypeName": str,
         "NextToken": str,
         "MaxResults": int,
         "Aggregator": bool,
@@ -2111,100 +1928,46 @@
 GetMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskIds": List[str],
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "InvocationId": str,
     },
 )
 
-GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
-    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
-    {
-        "WindowExecutionId": str,
-        "TaskExecutionId": str,
-        "InvocationId": str,
-        "ExecutionId": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "Parameters": str,
-        "Status": MaintenanceWindowExecutionStatusType,
-        "StatusDetails": str,
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "OwnerInformation": str,
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowExecutionTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 
-MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
-    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+MaintenanceWindowTaskParameterValueExpressionOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     {
         "Values": List[str],
     },
     total=False,
 )
 
 GetMaintenanceWindowRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 
-GetMaintenanceWindowResultTypeDef = TypedDict(
-    "GetMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "NextExecutionTime": str,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
@@ -2220,36 +1983,40 @@
     "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
+
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalGetOpsItemRequestRequestTypeDef = TypedDict(
     "_OptionalGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class GetOpsItemRequestRequestTypeDef(
     _RequiredGetOpsItemRequestRequestTypeDef, _OptionalGetOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalGetOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -2257,19 +2024,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2277,45 +2046,26 @@
     "_OptionalOpsFilterTypeDef",
     {
         "Type": OpsFilterOperatorTypeType,
     },
     total=False,
 )
 
+
 class OpsFilterTypeDef(_RequiredOpsFilterTypeDef, _OptionalOpsFilterTypeDef):
     pass
 
+
 OpsResultAttributeTypeDef = TypedDict(
     "OpsResultAttributeTypeDef",
     {
         "TypeName": str,
     },
 )
 
-_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
-    {
-        "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
-    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetParameterHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterHistoryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterHistoryRequestRequestTypeDef = TypedDict(
@@ -2324,39 +2074,43 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParameterHistoryRequestRequestTypeDef(
     _RequiredGetParameterHistoryRequestRequestTypeDef,
     _OptionalGetParameterHistoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetParameterRequestRequestTypeDef = TypedDict(
     "_RequiredGetParameterRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetParameterRequestRequestTypeDef = TypedDict(
     "_OptionalGetParameterRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParameterRequestRequestTypeDef(
     _RequiredGetParameterRequestRequestTypeDef, _OptionalGetParameterRequestRequestTypeDef
 ):
     pass
 
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "Value": str,
         "Version": int,
@@ -2379,76 +2133,59 @@
     "_OptionalGetParametersRequestRequestTypeDef",
     {
         "WithDecryption": bool,
     },
     total=False,
 )
 
+
 class GetParametersRequestRequestTypeDef(
     _RequiredGetParametersRequestRequestTypeDef, _OptionalGetParametersRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "_OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
     },
     total=False,
 )
 
+
 class GetPatchBaselineForPatchGroupRequestRequestTypeDef(
     _RequiredGetPatchBaselineForPatchGroupRequestRequestTypeDef,
     _OptionalGetPatchBaselineForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
-GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "GetPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "OperatingSystem": OperatingSystemType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetPatchBaselineRequestRequestTypeDef = TypedDict(
     "GetPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+PatchSourceOutputTypeDef = TypedDict(
+    "PatchSourceOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
+        "Products": List[str],
+        "Configuration": str,
     },
-    total=False,
 )
 
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -2456,20 +2193,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseEntryTypeDef = TypedDict(
     "GetResourcePoliciesResponseEntryTypeDef",
     {
         "PolicyId": str,
         "PolicyHash": str,
         "Policy": str,
     },
@@ -2555,17 +2294,19 @@
         "ContentHash": str,
         "Content": Sequence[Mapping[str, str]],
         "Context": Mapping[str, str],
     },
     total=False,
 )
 
+
 class InventoryItemTypeDef(_RequiredInventoryItemTypeDef, _OptionalInventoryItemTypeDef):
     pass
 
+
 _RequiredInventoryResultItemTypeDef = TypedDict(
     "_RequiredInventoryResultItemTypeDef",
     {
         "TypeName": str,
         "SchemaVersion": str,
         "Content": List[Dict[str, str]],
     },
@@ -2575,19 +2316,21 @@
     {
         "CaptureTime": str,
         "ContentHash": str,
     },
     total=False,
 )
 
+
 class InventoryResultItemTypeDef(
     _RequiredInventoryResultItemTypeDef, _OptionalInventoryResultItemTypeDef
 ):
     pass
 
+
 _RequiredLabelParameterVersionRequestRequestTypeDef = TypedDict(
     "_RequiredLabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "Labels": Sequence[str],
     },
 )
@@ -2595,48 +2338,21 @@
     "_OptionalLabelParameterVersionRequestRequestTypeDef",
     {
         "ParameterVersion": int,
     },
     total=False,
 )
 
+
 class LabelParameterVersionRequestRequestTypeDef(
     _RequiredLabelParameterVersionRequestRequestTypeDef,
     _OptionalLabelParameterVersionRequestRequestTypeDef,
 ):
     pass
 
-LabelParameterVersionResultTypeDef = TypedDict(
-    "LabelParameterVersionResultTypeDef",
-    {
-        "InvalidLabels": List[str],
-        "ParameterVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "AssociationId": str,
-    },
-)
-_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
-    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListAssociationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociationVersionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
@@ -2645,20 +2361,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationVersionsRequestRequestTypeDef(
     _RequiredListAssociationVersionsRequestRequestTypeDef,
     _OptionalListAssociationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDocumentMetadataHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentMetadataHistoryRequestRequestTypeDef",
     {
         "Name": str,
         "Metadata": Literal["DocumentReviews"],
     },
 )
@@ -2668,39 +2386,21 @@
         "DocumentVersion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDocumentMetadataHistoryRequestRequestTypeDef(
     _RequiredListDocumentMetadataHistoryRequestRequestTypeDef,
     _OptionalListDocumentMetadataHistoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
-    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDocumentVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
@@ -2709,32 +2409,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDocumentVersionsRequestRequestTypeDef(
     _RequiredListDocumentVersionsRequestRequestTypeDef,
     _OptionalListDocumentVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListInventoryEntriesResultTypeDef = TypedDict(
-    "ListInventoryEntriesResultTypeDef",
-    {
-        "TypeName": str,
-        "InstanceId": str,
-        "SchemaVersion": str,
-        "CaptureTime": str,
-        "Entries": List[Dict[str, str]],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 OpsItemEventFilterTypeDef = TypedDict(
     "OpsItemEventFilterTypeDef",
     {
         "Key": Literal["OpsItemId"],
         "Values": Sequence[str],
         "Operator": Literal["Equal"],
@@ -2766,23 +2455,14 @@
         "LastModifiedDate": datetime,
         "LastModifiedUser": str,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
-    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
-    {
-        "SyncType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceDataSyncRequestRequestTypeDef = TypedDict(
     "ListResourceDataSyncRequestRequestTypeDef",
     {
         "SyncType": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2793,42 +2473,69 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
+MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowAutomationParametersOutputTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Dict[str, List[str]],
+    },
+    total=False,
+)
+
 MaintenanceWindowAutomationParametersTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersTypeDef",
     {
         "DocumentVersion": str,
-        "Parameters": Dict[str, List[str]],
+        "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-MaintenanceWindowLambdaParametersTypeDef = TypedDict(
-    "MaintenanceWindowLambdaParametersTypeDef",
+MaintenanceWindowLambdaParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersOutputTypeDef",
     {
         "ClientContext": str,
         "Qualifier": str,
         "Payload": bytes,
     },
     total=False,
 )
 
+NotificationConfigTypeDef = TypedDict(
+    "NotificationConfigTypeDef",
+    {
+        "NotificationArn": str,
+        "NotificationEvents": Sequence[NotificationEventType],
+        "NotificationType": NotificationTypeType,
+    },
+    total=False,
+)
+
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
 )
 
+MaintenanceWindowTaskParameterValueExpressionTypeDef = TypedDict(
+    "MaintenanceWindowTaskParameterValueExpressionTypeDef",
+    {
+        "Values": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredModifyDocumentPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredModifyDocumentPermissionRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionType": Literal["Share"],
     },
 )
@@ -2838,20 +2545,22 @@
         "AccountIdsToAdd": Sequence[str],
         "AccountIdsToRemove": Sequence[str],
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
+
 class ModifyDocumentPermissionRequestRequestTypeDef(
     _RequiredModifyDocumentPermissionRequestRequestTypeDef,
     _OptionalModifyDocumentPermissionRequestRequestTypeDef,
 ):
     pass
 
+
 OpsEntityItemTypeDef = TypedDict(
     "OpsEntityItemTypeDef",
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
@@ -2861,56 +2570,37 @@
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
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
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
     total=False,
 )
 
-PatchFilterTypeDef = TypedDict(
-    "PatchFilterTypeDef",
+PatchFilterOutputTypeDef = TypedDict(
+    "PatchFilterOutputTypeDef",
     {
         "Key": PatchFilterKeyType,
-        "Values": Sequence[str],
-    },
-)
-
-PutInventoryResultTypeDef = TypedDict(
-    "PutInventoryResultTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Values": List[str],
     },
 )
 
-PutParameterResultTypeDef = TypedDict(
-    "PutParameterResultTypeDef",
+PatchFilterTypeDef = TypedDict(
+    "PatchFilterTypeDef",
     {
-        "Version": int,
-        "Tier": ParameterTierType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": PatchFilterKeyType,
+        "Values": Sequence[str],
     },
 )
 
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -2922,76 +2612,36 @@
     {
         "PolicyId": str,
         "PolicyHash": str,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "PolicyId": str,
-        "PolicyHash": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 RegisterDefaultPatchBaselineRequestRequestTypeDef = TypedDict(
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 
-RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
-    "RegisterDefaultPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterPatchBaselineForPatchGroupRequestRequestTypeDef = TypedDict(
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     {
         "BaselineId": str,
         "PatchGroup": str,
     },
 )
 
-RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
-    "RegisterPatchBaselineForPatchGroupResultTypeDef",
-    {
-        "BaselineId": str,
-        "PatchGroup": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTargetWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTargetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
-    "RegisterTaskWithMaintenanceWindowResultTypeDef",
-    {
-        "WindowTaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -3016,42 +2666,21 @@
     "ResourceDataSyncDestinationDataSharingTypeDef",
     {
         "DestinationDataSharingType": str,
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
 ResumeSessionRequestRequestTypeDef = TypedDict(
     "ResumeSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-ResumeSessionResponseTypeDef = TypedDict(
-    "ResumeSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendAutomationSignalRequestRequestTypeDef = TypedDict(
     "_RequiredSendAutomationSignalRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
         "SignalType": SignalTypeType,
     },
 )
@@ -3059,20 +2688,22 @@
     "_OptionalSendAutomationSignalRequestRequestTypeDef",
     {
         "Payload": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class SendAutomationSignalRequestRequestTypeDef(
     _RequiredSendAutomationSignalRequestRequestTypeDef,
     _OptionalSendAutomationSignalRequestRequestTypeDef,
 ):
     pass
 
+
 SessionManagerOutputUrlTypeDef = TypedDict(
     "SessionManagerOutputUrlTypeDef",
     {
         "S3OutputUrl": str,
         "CloudWatchOutputUrl": str,
     },
     total=False,
@@ -3081,30 +2712,14 @@
 StartAssociationsOnceRequestRequestTypeDef = TypedDict(
     "StartAssociationsOnceRequestRequestTypeDef",
     {
         "AssociationIds": Sequence[str],
     },
 )
 
-StartAutomationExecutionResultTypeDef = TypedDict(
-    "StartAutomationExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartChangeRequestExecutionResultTypeDef = TypedDict(
-    "StartChangeRequestExecutionResultTypeDef",
-    {
-        "AutomationExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "Target": str,
     },
 )
 _OptionalStartSessionRequestRequestTypeDef = TypedDict(
@@ -3113,28 +2728,20 @@
         "DocumentName": str,
         "Reason": str,
         "Parameters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class StartSessionRequestRequestTypeDef(
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "TokenValue": str,
-        "StreamUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStopAutomationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStopAutomationExecutionRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
@@ -3142,53 +2749,38 @@
     "_OptionalStopAutomationExecutionRequestRequestTypeDef",
     {
         "Type": StopTypeType,
     },
     total=False,
 )
 
+
 class StopAutomationExecutionRequestRequestTypeDef(
     _RequiredStopAutomationExecutionRequestRequestTypeDef,
     _OptionalStopAutomationExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnlabelParameterVersionRequestRequestTypeDef = TypedDict(
     "UnlabelParameterVersionRequestRequestTypeDef",
     {
         "Name": str,
         "ParameterVersion": int,
         "Labels": Sequence[str],
     },
 )
 
-UnlabelParameterVersionResultTypeDef = TypedDict(
-    "UnlabelParameterVersionResultTypeDef",
-    {
-        "RemovedLabels": List[str],
-        "InvalidLabels": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDocumentDefaultVersionRequestRequestTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionRequestRequestTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
     },
 )
@@ -3214,73 +2806,38 @@
         "AllowUnassociatedTargets": bool,
         "Enabled": bool,
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdateMaintenanceWindowRequestRequestTypeDef(
     _RequiredUpdateMaintenanceWindowRequestRequestTypeDef,
     _OptionalUpdateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-UpdateMaintenanceWindowResultTypeDef = TypedDict(
-    "UpdateMaintenanceWindowResultTypeDef",
-    {
-        "WindowId": str,
-        "Name": str,
-        "Description": str,
-        "StartDate": str,
-        "EndDate": str,
-        "Schedule": str,
-        "ScheduleTimezone": str,
-        "ScheduleOffset": int,
-        "Duration": int,
-        "Cutoff": int,
-        "AllowUnassociatedTargets": bool,
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateManagedInstanceRoleRequestRequestTypeDef = TypedDict(
     "UpdateManagedInstanceRoleRequestRequestTypeDef",
     {
         "InstanceId": str,
         "IamRole": str,
     },
 )
 
-UpdateOpsMetadataResultTypeDef = TypedDict(
-    "UpdateOpsMetadataResultTypeDef",
-    {
-        "OpsMetadataArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateServiceSettingRequestRequestTypeDef = TypedDict(
     "UpdateServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
         "SettingValue": str,
     },
 )
 
-DescribeDocumentPermissionResponseTypeDef = TypedDict(
-    "DescribeDocumentPermissionResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivationTypeDef = TypedDict(
     "ActivationTypeDef",
     {
         "ActivationId": str,
         "Description": str,
         "DefaultInstanceName": str,
         "IamRole": str,
@@ -3323,27 +2880,21 @@
         "ScheduleOffset": int,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMaintenanceWindowRequestRequestTypeDef(
     _RequiredCreateMaintenanceWindowRequestRequestTypeDef,
     _OptionalCreateMaintenanceWindowRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutParameterRequestRequestTypeDef = TypedDict(
     "_RequiredPutParameterRequestRequestTypeDef",
     {
         "Name": str,
         "Value": str,
     },
@@ -3360,211 +2911,529 @@
         "Tier": ParameterTierType,
         "Policies": str,
         "DataType": str,
     },
     total=False,
 )
 
+
 class PutParameterRequestRequestTypeDef(
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredAlarmConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAlarmConfigurationOutputTypeDef",
+    {
+        "Alarms": List[AlarmTypeDef],
+    },
+)
+_OptionalAlarmConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAlarmConfigurationOutputTypeDef",
+    {
+        "IgnorePollAlarmFailure": bool,
+    },
+    total=False,
+)
+
+
+class AlarmConfigurationOutputTypeDef(
+    _RequiredAlarmConfigurationOutputTypeDef, _OptionalAlarmConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredAlarmConfigurationTypeDef = TypedDict(
     "_RequiredAlarmConfigurationTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationTypeDef = TypedDict(
     "_OptionalAlarmConfigurationTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
     total=False,
 )
 
+
 class AlarmConfigurationTypeDef(
     _RequiredAlarmConfigurationTypeDef, _OptionalAlarmConfigurationTypeDef
 ):
     pass
 
-UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
-    "UpdateAssociationStatusRequestRequestTypeDef",
+
+AssociateOpsItemRelatedItemResponseTypeDef = TypedDict(
+    "AssociateOpsItemRelatedItemResponseTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationStatus": AssociationStatusTypeDef,
+        "AssociationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociationTypeDef = TypedDict(
-    "AssociationTypeDef",
+CancelMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "CancelMaintenanceWindowExecutionResultTypeDef",
     {
-        "Name": str,
-        "InstanceId": str,
-        "AssociationId": str,
-        "AssociationVersion": str,
-        "DocumentVersion": str,
-        "Targets": List[TargetTypeDef],
-        "LastExecutionDate": datetime,
-        "Overview": AssociationOverviewTypeDef,
-        "ScheduleExpression": str,
-        "AssociationName": str,
-        "ScheduleOffset": int,
-        "TargetMaps": List[Dict[str, List[str]]],
+        "WindowExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+CreateActivationResultTypeDef = TypedDict(
+    "CreateActivationResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "ActivationId": str,
+        "ActivationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+
+CreateMaintenanceWindowResultTypeDef = TypedDict(
+    "CreateMaintenanceWindowResultTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-):
-    pass
+CreateOpsItemResponseTypeDef = TypedDict(
+    "CreateOpsItemResponseTypeDef",
+    {
+        "OpsItemId": str,
+        "OpsItemArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+CreateOpsMetadataResultTypeDef = TypedDict(
+    "CreateOpsMetadataResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+
+CreatePatchBaselineResultTypeDef = TypedDict(
+    "CreatePatchBaselineResultTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
-    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
-):
-    pass
+DeleteMaintenanceWindowResultTypeDef = TypedDict(
+    "DeleteMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-MaintenanceWindowTargetTypeDef = TypedDict(
-    "MaintenanceWindowTargetTypeDef",
+DeleteParametersResultTypeDef = TypedDict(
+    "DeleteParametersResultTypeDef",
+    {
+        "DeletedParameters": List[str],
+        "InvalidParameters": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePatchBaselineResultTypeDef = TypedDict(
+    "DeletePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "DeregisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterTargetFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTargetFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": List[TargetTypeDef],
-        "OwnerInformation": str,
-        "Name": str,
-        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+DeregisterTaskFromMaintenanceWindowResultTypeDef = TypedDict(
+    "DeregisterTaskFromMaintenanceWindowResultTypeDef",
     {
         "WindowId": str,
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Targets": Sequence[TargetTypeDef],
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+
+DescribeDocumentPermissionResponseTypeDef = TypedDict(
+    "DescribeDocumentPermissionResponseTypeDef",
+    {
+        "AccountIds": List[str],
+        "AccountSharingInfoList": List[AccountSharingInfoTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchGroupStateResultTypeDef = TypedDict(
+    "DescribePatchGroupStateResultTypeDef",
     {
+        "Instances": int,
+        "InstancesWithInstalledPatches": int,
+        "InstancesWithInstalledOtherPatches": int,
+        "InstancesWithInstalledPendingRebootPatches": int,
+        "InstancesWithInstalledRejectedPatches": int,
+        "InstancesWithMissingPatches": int,
+        "InstancesWithFailedPatches": int,
+        "InstancesWithNotApplicablePatches": int,
+        "InstancesWithUnreportedNotApplicablePatches": int,
+        "InstancesWithCriticalNonCompliantPatches": int,
+        "InstancesWithSecurityNonCompliantPatches": int,
+        "InstancesWithOtherNonCompliantPatches": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchPropertiesResultTypeDef = TypedDict(
+    "DescribePatchPropertiesResultTypeDef",
+    {
+        "Properties": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalendarStateResponseTypeDef = TypedDict(
+    "GetCalendarStateResponseTypeDef",
+    {
+        "State": CalendarStateType,
+        "AtTime": str,
+        "NextTransitionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConnectionStatusResponseTypeDef = TypedDict(
+    "GetConnectionStatusResponseTypeDef",
+    {
+        "Target": str,
+        "Status": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDefaultPatchBaselineResultTypeDef = TypedDict(
+    "GetDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeployablePatchSnapshotForInstanceResultTypeDef = TypedDict(
+    "GetDeployablePatchSnapshotForInstanceResultTypeDef",
+    {
+        "InstanceId": str,
+        "SnapshotId": str,
+        "SnapshotDownloadUrl": str,
+        "Product": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskIds": List[str],
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowExecutionTaskInvocationResultTypeDef = TypedDict(
+    "GetMaintenanceWindowExecutionTaskInvocationResultTypeDef",
+    {
+        "WindowExecutionId": str,
+        "TaskExecutionId": str,
+        "InvocationId": str,
+        "ExecutionId": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "Parameters": str,
+        "Status": MaintenanceWindowExecutionStatusType,
+        "StatusDetails": str,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "OwnerInformation": str,
+        "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMaintenanceWindowResultTypeDef = TypedDict(
+    "GetMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "ClientToken": str,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "NextExecutionTime": str,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-):
-    pass
+GetPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "GetPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "OperatingSystem": OperatingSystemType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+LabelParameterVersionResultTypeDef = TypedDict(
+    "LabelParameterVersionResultTypeDef",
+    {
+        "InvalidLabels": List[str],
+        "ParameterVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListInventoryEntriesResultTypeDef = TypedDict(
+    "ListInventoryEntriesResultTypeDef",
+    {
+        "TypeName": str,
+        "InstanceId": str,
+        "SchemaVersion": str,
+        "CaptureTime": str,
+        "Entries": List[Dict[str, str]],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutInventoryResultTypeDef = TypedDict(
+    "PutInventoryResultTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutParameterResultTypeDef = TypedDict(
+    "PutParameterResultTypeDef",
+    {
+        "Version": int,
+        "Tier": ParameterTierType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyHash": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDefaultPatchBaselineResultTypeDef = TypedDict(
+    "RegisterDefaultPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPatchBaselineForPatchGroupResultTypeDef = TypedDict(
+    "RegisterPatchBaselineForPatchGroupResultTypeDef",
+    {
+        "BaselineId": str,
+        "PatchGroup": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTargetWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTargetWithMaintenanceWindowResultTypeDef",
     {
-        "WindowId": str,
         "WindowTargetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+
+RegisterTaskWithMaintenanceWindowResultTypeDef = TypedDict(
+    "RegisterTaskWithMaintenanceWindowResultTypeDef",
     {
-        "Targets": Sequence[TargetTypeDef],
-        "OwnerInformation": str,
+        "WindowTaskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResumeSessionResponseTypeDef = TypedDict(
+    "ResumeSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAutomationExecutionResultTypeDef = TypedDict(
+    "StartAutomationExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartChangeRequestExecutionResultTypeDef = TypedDict(
+    "StartChangeRequestExecutionResultTypeDef",
+    {
+        "AutomationExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "TokenValue": str,
+        "StreamUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnlabelParameterVersionResultTypeDef = TypedDict(
+    "UnlabelParameterVersionResultTypeDef",
+    {
+        "RemovedLabels": List[str],
+        "InvalidLabels": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceWindowResultTypeDef = TypedDict(
+    "UpdateMaintenanceWindowResultTypeDef",
+    {
+        "WindowId": str,
         "Name": str,
         "Description": str,
-        "Replace": bool,
+        "StartDate": str,
+        "EndDate": str,
+        "Schedule": str,
+        "ScheduleTimezone": str,
+        "ScheduleOffset": int,
+        "Duration": int,
+        "Cutoff": int,
+        "AllowUnassociatedTargets": bool,
+        "Enabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateOpsMetadataResultTypeDef = TypedDict(
+    "UpdateOpsMetadataResultTypeDef",
+    {
+        "OpsMetadataArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociationTypeDef = TypedDict(
+    "AssociationTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationId": str,
+        "AssociationVersion": str,
+        "DocumentVersion": str,
+        "Targets": List[TargetOutputTypeDef],
+        "LastExecutionDate": datetime,
+        "Overview": AssociationOverviewTypeDef,
+        "ScheduleExpression": str,
+        "AssociationName": str,
+        "ScheduleOffset": int,
+        "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
-class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
-):
-    pass
+MaintenanceWindowTargetTypeDef = TypedDict(
+    "MaintenanceWindowTargetTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": List[TargetOutputTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+    },
+    total=False,
+)
 
 UpdateMaintenanceWindowTargetResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTargetResultTypeDef",
     {
         "WindowId": str,
         "WindowTargetId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "OwnerInformation": str,
         "Name": str,
         "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "AssociationId": str,
-        },
-    )
-)
-_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
-        {
-            "Filters": Sequence[AssociationExecutionFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionsRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDescribeAssociationExecutionsRequestRequestTypeDef = TypedDict(
@@ -3573,20 +3442,22 @@
         "Filters": Sequence[AssociationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 AssociationExecutionTargetTypeDef = TypedDict(
     "AssociationExecutionTargetTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "ResourceId": str,
@@ -3595,36 +3466,14 @@
         "DetailedStatus": str,
         "LastExecutionDate": datetime,
         "OutputSource": OutputSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "AssociationId": str,
-        "ExecutionId": str,
-    },
-)
-_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
-    {
-        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
-    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef",
     {
         "AssociationId": str,
         "ExecutionId": str,
     },
 )
@@ -3634,39 +3483,77 @@
         "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeAssociationExecutionTargetsRequestRequestTypeDef(
     _RequiredDescribeAssociationExecutionTargetsRequestRequestTypeDef,
     _OptionalDescribeAssociationExecutionTargetsRequestRequestTypeDef,
 ):
     pass
 
-ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
-    "ListAssociationsRequestListAssociationsPaginateTypeDef",
-    {
-        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListAssociationsRequestRequestTypeDef = TypedDict(
     "ListAssociationsRequestRequestTypeDef",
     {
         "AssociationFilterList": Sequence[AssociationFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredAssociationStatusTypeDef = TypedDict(
+    "_RequiredAssociationStatusTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Name": AssociationStatusNameType,
+        "Message": str,
+    },
+)
+_OptionalAssociationStatusTypeDef = TypedDict(
+    "_OptionalAssociationStatusTypeDef",
+    {
+        "AdditionalInfo": str,
+    },
+    total=False,
+)
+
+
+class AssociationStatusTypeDef(
+    _RequiredAssociationStatusTypeDef, _OptionalAssociationStatusTypeDef
+):
+    pass
+
+
+_RequiredComplianceExecutionSummaryTypeDef = TypedDict(
+    "_RequiredComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionTime": TimestampTypeDef,
+    },
+)
+_OptionalComplianceExecutionSummaryTypeDef = TypedDict(
+    "_OptionalComplianceExecutionSummaryTypeDef",
+    {
+        "ExecutionId": str,
+        "ExecutionType": str,
+    },
+    total=False,
+)
+
+
+class ComplianceExecutionSummaryTypeDef(
+    _RequiredComplianceExecutionSummaryTypeDef, _OptionalComplianceExecutionSummaryTypeDef
+):
+    pass
+
+
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3679,38 +3566,41 @@
         "DocumentVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentRequestRequestTypeDef(
     _RequiredUpdateDocumentRequestRequestTypeDef, _OptionalUpdateDocumentRequestRequestTypeDef
 ):
     pass
 
-DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
-    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
-    {
-        "Filters": Sequence[AutomationExecutionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeAutomationExecutionsRequestRequestTypeDef = TypedDict(
     "DescribeAutomationExecutionsRequestRequestTypeDef",
     {
         "Filters": Sequence[AutomationExecutionFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+MaintenanceWindowLambdaParametersTypeDef = TypedDict(
+    "MaintenanceWindowLambdaParametersTypeDef",
+    {
+        "ClientContext": str,
+        "Qualifier": str,
+        "Payload": BlobTypeDef,
+    },
+    total=False,
+)
+
 GetCommandInvocationResultTypeDef = TypedDict(
     "GetCommandInvocationResultTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "Comment": str,
         "DocumentName": str,
@@ -3723,54 +3613,31 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
-    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "Details": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[CommandFilterTypeDef],
         "Details": bool,
     },
     total=False,
 )
 
-ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
-    "ListCommandsRequestListCommandsPaginateTypeDef",
-    {
-        "CommandId": str,
-        "InstanceId": str,
-        "Filters": Sequence[CommandFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCommandsRequestRequestTypeDef = TypedDict(
     "ListCommandsRequestRequestTypeDef",
     {
         "CommandId": str,
         "InstanceId": str,
         "MaxResults": int,
         "NextToken": str,
@@ -3792,29 +3659,29 @@
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
     },
     total=False,
 )
 
-MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
-    "MaintenanceWindowRunCommandParametersTypeDef",
+MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersOutputTypeDef",
     {
         "Comment": str,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
         "ServiceRoleArn": str,
         "TimeoutSeconds": int,
     },
     total=False,
@@ -3826,96 +3693,42 @@
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Id": str,
         "Title": str,
         "Status": ComplianceStatusType,
         "Severity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "Details": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": str,
-        "ComplianceType": str,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
-        "Items": Sequence[ComplianceItemEntryTypeDef],
-    },
-)
-_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutComplianceItemsRequestRequestTypeDef",
-    {
-        "ItemContentHash": str,
-        "UploadType": ComplianceUploadTypeType,
-    },
-    total=False,
-)
-
-class PutComplianceItemsRequestRequestTypeDef(
-    _RequiredPutComplianceItemsRequestRequestTypeDef,
-    _OptionalPutComplianceItemsRequestRequestTypeDef,
-):
-    pass
-
-ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
-    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "ResourceIds": Sequence[str],
-        "ResourceTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceItemsRequestRequestTypeDef = TypedDict(
     "ListComplianceItemsRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "ResourceIds": Sequence[str],
         "ResourceTypes": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
-    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
-    {
-        "Filters": Sequence[ComplianceStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourceComplianceSummariesRequestRequestTypeDef = TypedDict(
     "ListResourceComplianceSummariesRequestRequestTypeDef",
     {
         "Filters": Sequence[ComplianceStringFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -3948,26 +3761,29 @@
 )
 _OptionalCreateActivationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateActivationRequestRequestTypeDef",
     {
         "Description": str,
         "DefaultInstanceName": str,
         "RegistrationLimit": int,
-        "ExpirationDate": Union[datetime, str],
+        "ExpirationDate": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "RegistrationMetadata": Sequence[RegistrationMetadataItemTypeDef],
     },
     total=False,
 )
 
+
 class CreateActivationRequestRequestTypeDef(
     _RequiredCreateActivationRequestRequestTypeDef, _OptionalCreateActivationRequestRequestTypeDef
 ):
     pass
 
+
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredCreateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDocumentRequestRequestTypeDef",
     {
         "Content": str,
         "Name": str,
     },
 )
@@ -3982,19 +3798,21 @@
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
+
 DocumentIdentifierTypeDef = TypedDict(
     "DocumentIdentifierTypeDef",
     {
         "Name": str,
         "CreatedDate": datetime,
         "DisplayName": str,
         "Owner": str,
@@ -4025,15 +3843,15 @@
         "StatusInformation": str,
         "Content": str,
         "DocumentType": DocumentTypeType,
         "DocumentFormat": DocumentFormatType,
         "Requires": List[DocumentRequiresTypeDef],
         "AttachmentsContent": List[AttachmentContentTypeDef],
         "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpsItemSummaryTypeDef = TypedDict(
     "OpsItemSummaryTypeDef",
     {
         "CreatedBy": str,
@@ -4072,28 +3890,30 @@
         "OperationalData": Mapping[str, OpsItemDataValueTypeDef],
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Tags": Sequence[TagTypeDef],
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 OpsItemTypeDef = TypedDict(
     "OpsItemTypeDef",
     {
         "CreatedBy": str,
         "OpsItemType": str,
         "CreatedTime": datetime,
         "Description": str,
@@ -4134,28 +3954,30 @@
         "Notifications": Sequence[OpsItemNotificationTypeDef],
         "Priority": int,
         "RelatedOpsItems": Sequence[RelatedOpsItemTypeDef],
         "Status": OpsItemStatusType,
         "Title": str,
         "Category": str,
         "Severity": str,
-        "ActualStartTime": Union[datetime, str],
-        "ActualEndTime": Union[datetime, str],
-        "PlannedStartTime": Union[datetime, str],
-        "PlannedEndTime": Union[datetime, str],
+        "ActualStartTime": TimestampTypeDef,
+        "ActualEndTime": TimestampTypeDef,
+        "PlannedStartTime": TimestampTypeDef,
+        "PlannedEndTime": TimestampTypeDef,
         "OpsItemArn": str,
     },
     total=False,
 )
 
+
 class UpdateOpsItemRequestRequestTypeDef(
     _RequiredUpdateOpsItemRequestRequestTypeDef, _OptionalUpdateOpsItemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsMetadataRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalCreateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -4163,26 +3985,28 @@
     {
         "Metadata": Mapping[str, MetadataValueTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
 GetOpsMetadataResultTypeDef = TypedDict(
     "GetOpsMetadataResultTypeDef",
     {
         "ResourceId": str,
         "Metadata": Dict[str, MetadataValueTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
@@ -4193,34 +4017,387 @@
     {
         "MetadataToUpdate": Mapping[str, MetadataValueTypeDef],
         "KeysToDelete": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateOpsMetadataRequestRequestTypeDef(
     _RequiredUpdateOpsMetadataRequestRequestTypeDef, _OptionalUpdateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+
+DescribeActivationsRequestRequestTypeDef = TypedDict(
+    "DescribeActivationsRequestRequestTypeDef",
+    {
+        "Filters": Sequence[DescribeActivationsFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeActivationsRequestDescribeActivationsPaginateTypeDef = TypedDict(
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     {
         "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeActivationsRequestRequestTypeDef = TypedDict(
-    "DescribeActivationsRequestRequestTypeDef",
+_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     {
-        "Filters": Sequence[DescribeActivationsFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "AssociationId": str,
+        "ExecutionId": str,
+    },
+)
+_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
+    {
+        "Filters": Sequence[AssociationExecutionTargetsFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "AssociationId": str,
+        },
+    )
+)
+_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
+        {
+            "Filters": Sequence[AssociationExecutionFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef(
+    _RequiredDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    _OptionalDescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+):
+    pass
+
+
+DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef = TypedDict(
+    "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
+    {
+        "Filters": Sequence[AutomationExecutionFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef(
+    _RequiredDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    _OptionalDescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "BaselineId": str,
+    },
+)
+_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef = TypedDict(
+    "_OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef(
+    _RequiredDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    _OptionalDescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef(
+    _RequiredDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    _OptionalDescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+    },
+)
+_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef(
+    _RequiredDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    _OptionalDescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+):
+    pass
+
+
+DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef = TypedDict(
+    "DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef",
+    {
+        "DeletionId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "OperatingSystem": OperatingSystemType,
+        "Property": PatchPropertyType,
+    },
+)
+_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef",
+    {
+        "PatchSet": PatchSetType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef(
+    _RequiredDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    _OptionalDescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+):
+    pass
+
+
+GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef = TypedDict(
+    "GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef",
+    {
+        "TypeName": str,
+        "Aggregator": bool,
+        "SubType": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef",
+    {
+        "WithDecryption": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef(
+    _RequiredGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    _OptionalGetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef(
+    _RequiredListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    _OptionalListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListAssociationsRequestListAssociationsPaginateTypeDef = TypedDict(
+    "ListAssociationsRequestListAssociationsPaginateTypeDef",
+    {
+        "AssociationFilterList": Sequence[AssociationFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef = TypedDict(
+    "ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "Details": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCommandsRequestListCommandsPaginateTypeDef = TypedDict(
+    "ListCommandsRequestListCommandsPaginateTypeDef",
+    {
+        "CommandId": str,
+        "InstanceId": str,
+        "Filters": Sequence[CommandFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceItemsRequestListComplianceItemsPaginateTypeDef = TypedDict(
+    "ListComplianceItemsRequestListComplianceItemsPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "ResourceIds": Sequence[str],
+        "ResourceTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef(
+    _RequiredListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    _OptionalListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef = TypedDict(
+    "ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef",
+    {
+        "Filters": Sequence[ComplianceStringFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef = TypedDict(
+    "ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef",
+    {
+        "SyncType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
@@ -4228,25 +4405,27 @@
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[StepExecutionFilterTypeDef],
         "ReverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef",
     {
         "AutomationExecutionId": str,
     },
 )
 _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef = TypedDict(
@@ -4256,25 +4435,27 @@
         "NextToken": str,
         "MaxResults": int,
         "ReverseOrder": bool,
     },
     total=False,
 )
 
+
 class DescribeAutomationStepExecutionsRequestRequestTypeDef(
     _RequiredDescribeAutomationStepExecutionsRequestRequestTypeDef,
     _OptionalDescribeAutomationStepExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeAvailablePatchesRequestRequestTypeDef = TypedDict(
     "DescribeAvailablePatchesRequestRequestTypeDef",
     {
@@ -4291,25 +4472,27 @@
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef(
     _RequiredDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     _OptionalDescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchesRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 _OptionalDescribeInstancePatchesRequestRequestTypeDef = TypedDict(
@@ -4318,52 +4501,27 @@
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchesRequestRequestTypeDef(
     _RequiredDescribeInstancePatchesRequestRequestTypeDef,
     _OptionalDescribeInstancePatchesRequestRequestTypeDef,
 ):
     pass
 
-DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
-    TypedDict(
-        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
-        {
-            "WindowId": str,
-            "Targets": Sequence[TargetTypeDef],
-            "ResourceType": MaintenanceWindowResourceTypeType,
-            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
-    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
-    {
-        "WindowId": str,
-        "Targets": Sequence[TargetTypeDef],
-        "ResourceType": MaintenanceWindowResourceTypeType,
-        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
 
 DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef = TypedDict(
     "DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchBaselinesRequestRequestTypeDef = TypedDict(
     "DescribePatchBaselinesRequestRequestTypeDef",
     {
@@ -4374,15 +4532,15 @@
     total=False,
 )
 
 DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef = TypedDict(
     "DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef",
     {
         "Filters": Sequence[PatchOrchestratorFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribePatchGroupsRequestRequestTypeDef = TypedDict(
     "DescribePatchGroupsRequestRequestTypeDef",
     {
@@ -4394,33 +4552,33 @@
 )
 
 DescribeAvailablePatchesResultTypeDef = TypedDict(
     "DescribeAvailablePatchesResultTypeDef",
     {
         "Patches": List[PatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEffectiveInstanceAssociationsResultTypeDef = TypedDict(
     "DescribeEffectiveInstanceAssociationsResultTypeDef",
     {
         "Associations": List[InstanceAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef = TypedDict(
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     {
         "InstanceInformationFilterList": Sequence[InstanceInformationFilterTypeDef],
         "Filters": Sequence[InstanceInformationStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeInstanceInformationRequestRequestTypeDef = TypedDict(
     "DescribeInstanceInformationRequestRequestTypeDef",
     {
@@ -4438,25 +4596,27 @@
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef = TypedDict(
     "_OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     {
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     {
         "PatchGroup": str,
     },
 )
 _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef = TypedDict(
@@ -4465,69 +4625,73 @@
         "Filters": Sequence[InstancePatchStateFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef(
     _RequiredDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
     _OptionalDescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInstancePatchStatesForPatchGroupResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchStatesResultTypeDef = TypedDict(
     "DescribeInstancePatchStatesResultTypeDef",
     {
         "InstancePatchStates": List[InstancePatchStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstancePatchesResultTypeDef = TypedDict(
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
     },
 )
@@ -4537,41 +4701,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef = TypedDict(
@@ -4580,41 +4748,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef = TypedDict(
@@ -4623,41 +4795,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowExecutionsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowExecutionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef = TypedDict(
@@ -4666,41 +4842,45 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTargetsRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef = TypedDict(
     "_OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestDescribeMaintenanceWindowTasksPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef",
     {
         "WindowId": str,
     },
 )
 _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef = TypedDict(
@@ -4709,25 +4889,27 @@
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeMaintenanceWindowTasksRequestRequestTypeDef(
     _RequiredDescribeMaintenanceWindowTasksRequestRequestTypeDef,
     _OptionalDescribeMaintenanceWindowTasksRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestDescribeMaintenanceWindowsPaginateTypeDef",
     {
         "Filters": Sequence[MaintenanceWindowFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeMaintenanceWindowsRequestRequestTypeDef = TypedDict(
     "DescribeMaintenanceWindowsRequestRequestTypeDef",
     {
@@ -4741,59 +4923,59 @@
 DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef",
     {
         "WindowExecutionTaskInvocationIdentities": List[
             MaintenanceWindowExecutionTaskInvocationIdentityTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionsResultTypeDef",
     {
         "WindowExecutions": List[MaintenanceWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowScheduleResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowScheduleResultTypeDef",
     {
         "ScheduledWindowExecutions": List[ScheduledWindowExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsForTargetResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsForTargetResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityForTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowsResultTypeDef",
     {
         "WindowIdentities": List[MaintenanceWindowIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef = TypedDict(
     "DescribeOpsItemsRequestDescribeOpsItemsPaginateTypeDef",
     {
         "OpsItemFilters": Sequence[OpsItemFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeOpsItemsRequestRequestTypeDef = TypedDict(
     "DescribeOpsItemsRequestRequestTypeDef",
     {
@@ -4812,25 +4994,27 @@
 )
 _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef = TypedDict(
     "_OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef",
     {
         "Recursive": bool,
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
         "WithDecryption": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestGetParametersByPathPaginateTypeDef(
     _RequiredGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
     _OptionalGetParametersByPathRequestGetParametersByPathPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetParametersByPathRequestRequestTypeDef = TypedDict(
     "_RequiredGetParametersByPathRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalGetParametersByPathRequestRequestTypeDef = TypedDict(
@@ -4841,26 +5025,28 @@
         "WithDecryption": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetParametersByPathRequestRequestTypeDef(
     _RequiredGetParametersByPathRequestRequestTypeDef,
     _OptionalGetParametersByPathRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     {
         "Filters": Sequence[ParametersFilterTypeDef],
         "ParameterFilters": Sequence[ParameterStringFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeParametersRequestRequestTypeDef = TypedDict(
     "DescribeParametersRequestRequestTypeDef",
     {
@@ -4873,15 +5059,15 @@
 )
 
 DescribePatchBaselinesResultTypeDef = TypedDict(
     "DescribePatchBaselinesResultTypeDef",
     {
         "BaselineIdentities": List[PatchBaselineIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PatchGroupPatchBaselineMappingTypeDef = TypedDict(
     "PatchGroupPatchBaselineMappingTypeDef",
     {
         "PatchGroup": str,
@@ -4896,25 +5082,27 @@
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef = TypedDict(
     "_OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     {
         "Filters": Sequence[SessionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestDescribeSessionsPaginateTypeDef(
     _RequiredDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     _OptionalDescribeSessionsRequestDescribeSessionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSessionsRequestRequestTypeDef",
     {
         "State": SessionStateType,
     },
 )
 _OptionalDescribeSessionsRequestRequestTypeDef = TypedDict(
@@ -4923,24 +5111,26 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[SessionFilterTypeDef],
     },
     total=False,
 )
 
+
 class DescribeSessionsRequestRequestTypeDef(
     _RequiredDescribeSessionsRequestRequestTypeDef, _OptionalDescribeSessionsRequestRequestTypeDef
 ):
     pass
 
+
 UpdateDocumentDefaultVersionResultTypeDef = TypedDict(
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
@@ -4978,15 +5168,15 @@
 )
 
 ListDocumentsRequestListDocumentsPaginateTypeDef = TypedDict(
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     {
         "DocumentFilterList": Sequence[DocumentFilterTypeDef],
         "Filters": Sequence[DocumentKeyValuesFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDocumentsRequestRequestTypeDef = TypedDict(
     "ListDocumentsRequestRequestTypeDef",
     {
@@ -5020,23 +5210,25 @@
     "_OptionalDocumentReviewsTypeDef",
     {
         "Comment": Sequence[DocumentReviewCommentSourceTypeDef],
     },
     total=False,
 )
 
+
 class DocumentReviewsTypeDef(_RequiredDocumentReviewsTypeDef, _OptionalDocumentReviewsTypeDef):
     pass
 
+
 ListDocumentVersionsResultTypeDef = TypedDict(
     "ListDocumentVersionsResultTypeDef",
     {
         "DocumentVersions": List[DocumentVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EffectivePatchTypeDef = TypedDict(
     "EffectivePatchTypeDef",
     {
         "Patch": PatchTypeDef,
@@ -5057,20 +5249,22 @@
     {
         "PluginName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCommandInvocationRequestCommandExecutedWaitTypeDef(
     _RequiredGetCommandInvocationRequestCommandExecutedWaitTypeDef,
     _OptionalGetCommandInvocationRequestCommandExecutedWaitTypeDef,
 ):
     pass
 
+
 InventoryGroupTypeDef = TypedDict(
     "InventoryGroupTypeDef",
     {
         "Name": str,
         "Filters": Sequence[InventoryFilterTypeDef],
     },
 )
@@ -5088,27 +5282,29 @@
         "Filters": Sequence[InventoryFilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListInventoryEntriesRequestRequestTypeDef(
     _RequiredListInventoryEntriesRequestRequestTypeDef,
     _OptionalListInventoryEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 GetInventoryRequestGetInventoryPaginateTypeDef = TypedDict(
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "Aggregators": Sequence["InventoryAggregatorTypeDef"],
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetInventoryRequestRequestTypeDef = TypedDict(
     "GetInventoryRequestRequestTypeDef",
     {
@@ -5137,15 +5333,15 @@
 GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef = TypedDict(
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     {
         "SyncName": str,
         "Filters": Sequence[OpsFilterTypeDef],
         "Aggregators": Sequence["OpsAggregatorTypeDef"],
         "ResultAttributes": Sequence[OpsResultAttributeTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetOpsSummaryRequestRequestTypeDef = TypedDict(
     "GetOpsSummaryRequestRequestTypeDef",
     {
@@ -5159,58 +5355,59 @@
     total=False,
 )
 
 GetParameterResultTypeDef = TypedDict(
     "GetParameterResultTypeDef",
     {
         "Parameter": ParameterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersByPathResultTypeDef = TypedDict(
     "GetParametersByPathResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParametersResultTypeDef = TypedDict(
     "GetParametersResultTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "InvalidParameters": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PatchSourceUnionTypeDef = Union[PatchSourceTypeDef, PatchSourceOutputTypeDef]
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "NextToken": str,
         "Policies": List[GetResourcePoliciesResponseEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceSettingResultTypeDef = TypedDict(
     "GetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetServiceSettingResultTypeDef = TypedDict(
     "ResetServiceSettingResultTypeDef",
     {
         "ServiceSetting": ServiceSettingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceInformationTypeDef = TypedDict(
     "InstanceInformationTypeDef",
     {
         "InstanceId": str,
@@ -5276,19 +5473,21 @@
     {
         "Version": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+
 class InventoryItemSchemaTypeDef(
     _RequiredInventoryItemSchemaTypeDef, _OptionalInventoryItemSchemaTypeDef
 ):
     pass
 
+
 PutInventoryRequestRequestTypeDef = TypedDict(
     "PutInventoryRequestRequestTypeDef",
     {
         "InstanceId": str,
         "Items": Sequence[InventoryItemTypeDef],
     },
 )
@@ -5302,15 +5501,15 @@
     total=False,
 )
 
 ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef = TypedDict(
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
     {
         "Filters": Sequence[OpsItemEventFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemEventsRequestRequestTypeDef = TypedDict(
     "ListOpsItemEventsRequestRequestTypeDef",
     {
@@ -5322,15 +5521,15 @@
 )
 
 ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     {
         "OpsItemId": str,
         "Filters": Sequence[OpsItemRelatedItemsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsItemRelatedItemsRequestRequestTypeDef = TypedDict(
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     {
@@ -5342,15 +5541,15 @@
     total=False,
 )
 
 ListOpsMetadataRequestListOpsMetadataPaginateTypeDef = TypedDict(
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     {
         "Filters": Sequence[OpsMetadataFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListOpsMetadataRequestRequestTypeDef = TypedDict(
     "ListOpsMetadataRequestRequestTypeDef",
     {
@@ -5362,18 +5561,41 @@
 )
 
 ListOpsMetadataResultTypeDef = TypedDict(
     "ListOpsMetadataResultTypeDef",
     {
         "OpsMetadataList": List[OpsMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MaintenanceWindowRunCommandParametersTypeDef = TypedDict(
+    "MaintenanceWindowRunCommandParametersTypeDef",
+    {
+        "Comment": str,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "DocumentVersion": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ServiceRoleArn": str,
+        "TimeoutSeconds": int,
+    },
+    total=False,
+)
+
+NotificationConfigUnionTypeDef = Union[NotificationConfigTypeDef, NotificationConfigOutputTypeDef]
+MaintenanceWindowTaskParameterValueExpressionUnionTypeDef = Union[
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
+]
 OpsEntityTypeDef = TypedDict(
     "OpsEntityTypeDef",
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
@@ -5443,41 +5665,72 @@
         "Tier": ParameterTierType,
         "Policies": List[ParameterInlinePolicyTypeDef],
         "DataType": str,
     },
     total=False,
 )
 
+PatchFilterGroupOutputTypeDef = TypedDict(
+    "PatchFilterGroupOutputTypeDef",
+    {
+        "PatchFilters": List[PatchFilterOutputTypeDef],
+    },
+)
+
 PatchFilterGroupTypeDef = TypedDict(
     "PatchFilterGroupTypeDef",
     {
         "PatchFilters": Sequence[PatchFilterTypeDef],
     },
 )
 
+_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationSourceType": str,
+    },
+)
+_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
+    "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
+    {
+        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
+    },
+    total=False,
+)
+
+
+class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
+    _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+    _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+):
+    pass
+
+
 _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceTypeDef",
     {
         "OrganizationalUnits": Sequence[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
+
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
+
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5488,19 +5741,21 @@
         "Prefix": str,
         "AWSKMSKeyARN": str,
         "DestinationDataSharing": ResourceDataSyncDestinationDataSharingTypeDef,
     },
     total=False,
 )
 
+
 class ResourceDataSyncS3DestinationTypeDef(
     _RequiredResourceDataSyncS3DestinationTypeDef, _OptionalResourceDataSyncS3DestinationTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "SessionId": str,
         "Target": str,
         "Status": SessionStatusType,
         "StartDate": datetime,
@@ -5516,30 +5771,30 @@
 )
 
 DescribeActivationsResultTypeDef = TypedDict(
     "DescribeActivationsResultTypeDef",
     {
         "ActivationList": List[ActivationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationExecutionTypeDef = TypedDict(
     "AssociationExecutionTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "ExecutionId": str,
         "Status": str,
         "DetailedStatus": str,
         "CreatedTime": datetime,
         "LastExecutionDate": datetime,
         "ResourceCountByStatus": str,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
@@ -5547,133 +5802,114 @@
         "CommandId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "Comment": str,
         "ExpiresAfter": datetime,
         "Parameters": Dict[str, List[str]],
         "InstanceIds": List[str],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "RequestedDateTime": datetime,
         "Status": CommandStatusType,
         "StatusDetails": str,
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
-        "NotificationConfig": NotificationConfigTypeDef,
+        "NotificationConfig": NotificationConfigOutputTypeDef,
         "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "TimeoutSeconds": int,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 GetMaintenanceWindowExecutionTaskResultTypeDef = TypedDict(
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "TaskArn": str,
         "ServiceRole": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "TaskParameters": List[Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef]],
+        "TaskParameters": List[
+            Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef]
+        ],
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MaintenanceWindowExecutionTaskIdentityTypeDef = TypedDict(
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
     {
         "WindowExecutionId": str,
         "TaskExecutionId": str,
         "Status": MaintenanceWindowExecutionStatusType,
         "StatusDetails": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "TaskArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 MaintenanceWindowTaskTypeDef = TypedDict(
     "MaintenanceWindowTaskTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
-        "Targets": List[TargetTypeDef],
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
+        "Targets": List[TargetOutputTypeDef],
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "Priority": int,
         "LoggingInfo": LoggingInfoTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredSendCommandRequestRequestTypeDef = TypedDict(
-    "_RequiredSendCommandRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalSendCommandRequestRequestTypeDef = TypedDict(
-    "_OptionalSendCommandRequestRequestTypeDef",
+TargetLocationOutputTypeDef = TypedDict(
+    "TargetLocationOutputTypeDef",
     {
-        "InstanceIds": Sequence[str],
-        "Targets": Sequence[TargetTypeDef],
-        "DocumentVersion": str,
-        "DocumentHash": str,
-        "DocumentHashType": DocumentHashTypeType,
-        "TimeoutSeconds": int,
-        "Comment": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "ServiceRoleArn": str,
-        "NotificationConfig": NotificationConfigTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "Accounts": List[str],
+        "Regions": List[str],
+        "TargetLocationMaxConcurrency": str,
+        "TargetLocationMaxErrors": str,
+        "ExecutionRoleName": str,
+        "TargetLocationAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class SendCommandRequestRequestTypeDef(
-    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
-):
-    pass
-
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
 TargetLocationTypeDef = TypedDict(
     "TargetLocationTypeDef",
     {
         "Accounts": Sequence[str],
         "Regions": Sequence[str],
         "TargetLocationMaxConcurrency": str,
         "TargetLocationMaxErrors": str,
@@ -5684,62 +5920,102 @@
 )
 
 ListAssociationsResultTypeDef = TypedDict(
     "ListAssociationsResultTypeDef",
     {
         "Associations": List[AssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTargetsResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     {
         "Targets": List[MaintenanceWindowTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionTargetsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionTargetsResultTypeDef",
     {
         "AssociationExecutionTargets": List[AssociationExecutionTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociationStatusUnionTypeDef = Union[AssociationStatusTypeDef, AssociationStatusOutputTypeDef]
+UpdateAssociationStatusRequestRequestTypeDef = TypedDict(
+    "UpdateAssociationStatusRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceId": str,
+        "AssociationStatus": AssociationStatusTypeDef,
     },
 )
 
+ComplianceExecutionSummaryUnionTypeDef = Union[
+    ComplianceExecutionSummaryTypeDef, ComplianceExecutionSummaryOutputTypeDef
+]
+_RequiredPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": str,
+        "ComplianceType": str,
+        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "Items": Sequence[ComplianceItemEntryTypeDef],
+    },
+)
+_OptionalPutComplianceItemsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutComplianceItemsRequestRequestTypeDef",
+    {
+        "ItemContentHash": str,
+        "UploadType": ComplianceUploadTypeType,
+    },
+    total=False,
+)
+
+
+class PutComplianceItemsRequestRequestTypeDef(
+    _RequiredPutComplianceItemsRequestRequestTypeDef,
+    _OptionalPutComplianceItemsRequestRequestTypeDef,
+):
+    pass
+
+
 ListCommandInvocationsResultTypeDef = TypedDict(
     "ListCommandInvocationsResultTypeDef",
     {
         "CommandInvocations": List[CommandInvocationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
-    "MaintenanceWindowTaskInvocationParametersTypeDef",
+MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     {
-        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
-        "Automation": MaintenanceWindowAutomationParametersTypeDef,
+        "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
         "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
-        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
     {
         "ComplianceItems": List[ComplianceItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryItemTypeDef = TypedDict(
     "ComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
@@ -5753,77 +6029,242 @@
     "ResourceComplianceSummaryItemTypeDef",
     {
         "ComplianceType": str,
         "ResourceType": str,
         "ResourceId": str,
         "Status": ComplianceStatusType,
         "OverallSeverity": ComplianceSeverityType,
-        "ExecutionSummary": ComplianceExecutionSummaryTypeDef,
+        "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
+DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef = (
+    TypedDict(
+        "DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef",
+        {
+            "WindowId": str,
+            "Targets": Sequence[TargetUnionTypeDef],
+            "ResourceType": MaintenanceWindowResourceTypeType,
+            "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeMaintenanceWindowScheduleRequestRequestTypeDef = TypedDict(
+    "DescribeMaintenanceWindowScheduleRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Filters": Sequence[PatchOrchestratorFilterTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ResourceType": MaintenanceWindowResourceTypeType,
+    },
+)
+_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeMaintenanceWindowsForTargetRequestRequestTypeDef(
+    _RequiredDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    _OptionalDescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "ResourceType": MaintenanceWindowResourceTypeType,
+        "Targets": Sequence[TargetUnionTypeDef],
+    },
+)
+_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class RegisterTargetWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSendCommandRequestRequestTypeDef = TypedDict(
+    "_RequiredSendCommandRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalSendCommandRequestRequestTypeDef = TypedDict(
+    "_OptionalSendCommandRequestRequestTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "DocumentVersion": str,
+        "DocumentHash": str,
+        "DocumentHashType": DocumentHashTypeType,
+        "TimeoutSeconds": int,
+        "Comment": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "OutputS3Region": str,
+        "OutputS3BucketName": str,
+        "OutputS3KeyPrefix": str,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "ServiceRoleArn": str,
+        "NotificationConfig": NotificationConfigTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class SendCommandRequestRequestTypeDef(
+    _RequiredSendCommandRequestRequestTypeDef, _OptionalSendCommandRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTargetId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "OwnerInformation": str,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+    },
+    total=False,
+)
+
+
+class UpdateMaintenanceWindowTargetRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTargetRequestRequestTypeDef,
+):
+    pass
+
+
 ListDocumentsResultTypeDef = TypedDict(
     "ListDocumentsResultTypeDef",
     {
         "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOpsItemsResponseTypeDef = TypedDict(
     "DescribeOpsItemsResponseTypeDef",
     {
         "NextToken": str,
         "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOpsItemResponseTypeDef = TypedDict(
     "GetOpsItemResponseTypeDef",
     {
         "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePatchGroupsResultTypeDef = TypedDict(
     "DescribePatchGroupsResultTypeDef",
     {
         "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDocumentResultTypeDef = TypedDict(
     "DescribeDocumentResultTypeDef",
     {
         "Document": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDocumentResultTypeDef = TypedDict(
     "UpdateDocumentResultTypeDef",
     {
         "DocumentDescription": DocumentDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataResponseInfoTypeDef = TypedDict(
     "DocumentMetadataResponseInfoTypeDef",
     {
         "ReviewerResponse": List[DocumentReviewerResponseSourceTypeDef],
@@ -5842,26 +6283,28 @@
     "_OptionalUpdateDocumentMetadataRequestRequestTypeDef",
     {
         "DocumentVersion": str,
     },
     total=False,
 )
 
+
 class UpdateDocumentMetadataRequestRequestTypeDef(
     _RequiredUpdateDocumentMetadataRequestRequestTypeDef,
     _OptionalUpdateDocumentMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeEffectivePatchesForPatchBaselineResultTypeDef = TypedDict(
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     {
         "EffectivePatches": List[EffectivePatchTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryAggregatorTypeDef = TypedDict(
     "InventoryAggregatorTypeDef",
     {
         "Expression": str,
@@ -5872,15 +6315,15 @@
 )
 
 DescribeInstanceInformationResultTypeDef = TypedDict(
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": str,
@@ -5901,15 +6344,15 @@
 
 DeleteInventoryResultTypeDef = TypedDict(
     "DeleteInventoryResultTypeDef",
     {
         "DeletionId": str,
         "TypeName": str,
         "DeletionSummary": InventoryDeletionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InventoryDeletionStatusItemTypeDef = TypedDict(
     "InventoryDeletionStatusItemTypeDef",
     {
         "DeletionId": str,
@@ -5924,72 +6367,106 @@
 )
 
 GetInventorySchemaResultTypeDef = TypedDict(
     "GetInventorySchemaResultTypeDef",
     {
         "Schemas": List[InventoryItemSchemaTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInventoryResultTypeDef = TypedDict(
     "GetInventoryResultTypeDef",
     {
         "Entities": List[InventoryResultEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MaintenanceWindowTaskInvocationParametersTypeDef = TypedDict(
+    "MaintenanceWindowTaskInvocationParametersTypeDef",
+    {
+        "RunCommand": MaintenanceWindowRunCommandParametersTypeDef,
+        "Automation": MaintenanceWindowAutomationParametersTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
+        "Lambda": MaintenanceWindowLambdaParametersTypeDef,
     },
+    total=False,
 )
 
 GetOpsSummaryResultTypeDef = TypedDict(
     "GetOpsSummaryResultTypeDef",
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOpsItemRelatedItemsResponseTypeDef = TypedDict(
     "ListOpsItemRelatedItemsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParametersResultTypeDef = TypedDict(
     "DescribeParametersResultTypeDef",
     {
         "Parameters": List[ParameterMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPatchRuleOutputTypeDef = TypedDict(
+    "_RequiredPatchRuleOutputTypeDef",
+    {
+        "PatchFilterGroup": PatchFilterGroupOutputTypeDef,
+    },
+)
+_OptionalPatchRuleOutputTypeDef = TypedDict(
+    "_OptionalPatchRuleOutputTypeDef",
+    {
+        "ComplianceLevel": PatchComplianceLevelType,
+        "ApproveAfterDays": int,
+        "ApproveUntilDate": str,
+        "EnableNonSecurity": bool,
+    },
+    total=False,
+)
+
+
+class PatchRuleOutputTypeDef(_RequiredPatchRuleOutputTypeDef, _OptionalPatchRuleOutputTypeDef):
+    pass
+
+
+PatchFilterGroupUnionTypeDef = Union[PatchFilterGroupTypeDef, PatchFilterGroupOutputTypeDef]
 _RequiredPatchRuleTypeDef = TypedDict(
     "_RequiredPatchRuleTypeDef",
     {
         "PatchFilterGroup": PatchFilterGroupTypeDef,
     },
 )
 _OptionalPatchRuleTypeDef = TypedDict(
@@ -5999,17 +6476,32 @@
         "ApproveAfterDays": int,
         "ApproveUntilDate": str,
         "EnableNonSecurity": bool,
     },
     total=False,
 )
 
+
 class PatchRuleTypeDef(_RequiredPatchRuleTypeDef, _OptionalPatchRuleTypeDef):
     pass
 
+
+ResourceDataSyncSourceWithStateTypeDef = TypedDict(
+    "ResourceDataSyncSourceWithStateTypeDef",
+    {
+        "SourceType": str,
+        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
+        "SourceRegions": List[str],
+        "IncludeFutureRegions": bool,
+        "State": str,
+        "EnableAllOpsDataSources": bool,
+    },
+    total=False,
+)
+
 _RequiredResourceDataSyncSourceTypeDef = TypedDict(
     "_RequiredResourceDataSyncSourceTypeDef",
     {
         "SourceType": str,
         "SourceRegions": Sequence[str],
     },
 )
@@ -6019,275 +6511,200 @@
         "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
         "IncludeFutureRegions": bool,
         "EnableAllOpsDataSources": bool,
     },
     total=False,
 )
 
+
 class ResourceDataSyncSourceTypeDef(
     _RequiredResourceDataSyncSourceTypeDef, _OptionalResourceDataSyncSourceTypeDef
 ):
     pass
 
-ResourceDataSyncSourceWithStateTypeDef = TypedDict(
-    "ResourceDataSyncSourceWithStateTypeDef",
-    {
-        "SourceType": str,
-        "AwsOrganizationsSource": ResourceDataSyncAwsOrganizationsSourceTypeDef,
-        "SourceRegions": List[str],
-        "IncludeFutureRegions": bool,
-        "State": str,
-        "EnableAllOpsDataSources": bool,
-    },
-    total=False,
-)
 
 DescribeSessionsResponseTypeDef = TypedDict(
     "DescribeSessionsResponseTypeDef",
     {
         "Sessions": List[SessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationExecutionsResultTypeDef = TypedDict(
     "DescribeAssociationExecutionsResultTypeDef",
     {
         "AssociationExecutions": List[AssociationExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandsResultTypeDef = TypedDict(
     "ListCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "Command": CommandTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowExecutionTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTasksResultTypeDef",
     {
         "WindowExecutionTaskIdentities": List[MaintenanceWindowExecutionTaskIdentityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMaintenanceWindowTasksResultTypeDef = TypedDict(
     "DescribeMaintenanceWindowTasksResultTypeDef",
     {
         "Tasks": List[MaintenanceWindowTaskTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationDescriptionTypeDef = TypedDict(
     "AssociationDescriptionTypeDef",
     {
         "Name": str,
         "InstanceId": str,
         "AssociationVersion": str,
         "Date": datetime,
         "LastUpdateAssociationDate": datetime,
-        "Status": AssociationStatusTypeDef,
+        "Status": AssociationStatusOutputTypeDef,
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
 AssociationVersionInfoTypeDef = TypedDict(
     "AssociationVersionInfoTypeDef",
     {
         "AssociationId": str,
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": List[Dict[str, List[str]]],
     },
     total=False,
 )
 
-_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
+_RequiredCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
-    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
+_OptionalCreateAssociationBatchRequestEntryOutputTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryOutputTypeDef",
     {
         "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
+        "Parameters": Dict[str, List[str]],
         "AutomationTargetParameterName": str,
         "DocumentVersion": str,
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
+        "CalendarNames": List[str],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "TargetMaps": List[Dict[str, List[str]]],
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class CreateAssociationBatchRequestEntryTypeDef(
-    _RequiredCreateAssociationBatchRequestEntryTypeDef,
-    _OptionalCreateAssociationBatchRequestEntryTypeDef,
-):
-    pass
 
-_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssociationRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssociationRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "InstanceId": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "Targets": Sequence[TargetTypeDef],
-        "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "AssociationName": str,
-        "AutomationTargetParameterName": str,
-        "MaxErrors": str,
-        "MaxConcurrency": str,
-        "ComplianceSeverity": AssociationComplianceSeverityType,
-        "SyncCompliance": AssociationSyncComplianceType,
-        "ApplyOnlyAtCronInterval": bool,
-        "CalendarNames": Sequence[str],
-        "TargetLocations": Sequence[TargetLocationTypeDef],
-        "ScheduleOffset": int,
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateAssociationRequestRequestTypeDef(
-    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+class CreateAssociationBatchRequestEntryOutputTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryOutputTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryOutputTypeDef,
 ):
     pass
 
-_RequiredRunbookTypeDef = TypedDict(
-    "_RequiredRunbookTypeDef",
+
+_RequiredRunbookOutputTypeDef = TypedDict(
+    "_RequiredRunbookOutputTypeDef",
     {
         "DocumentName": str,
     },
 )
-_OptionalRunbookTypeDef = TypedDict(
-    "_OptionalRunbookTypeDef",
+_OptionalRunbookOutputTypeDef = TypedDict(
+    "_OptionalRunbookOutputTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
     },
     total=False,
 )
 
-class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
-    pass
-
-_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-    },
-)
-_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
-    {
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ClientToken": str,
-        "Mode": ExecutionModeType,
-        "TargetParameterName": str,
-        "Targets": Sequence[TargetTypeDef],
-        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "TargetLocations": Sequence[TargetLocationTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-    },
-    total=False,
-)
 
-class StartAutomationExecutionRequestRequestTypeDef(
-    _RequiredStartAutomationExecutionRequestRequestTypeDef,
-    _OptionalStartAutomationExecutionRequestRequestTypeDef,
-):
+class RunbookOutputTypeDef(_RequiredRunbookOutputTypeDef, _OptionalRunbookOutputTypeDef):
     pass
 
+
 StepExecutionTypeDef = TypedDict(
     "StepExecutionTypeDef",
     {
         "StepName": str,
         "Action": str,
         "TimeoutSeconds": int,
         "OnFailure": str,
@@ -6303,226 +6720,287 @@
         "FailureDetails": FailureDetailsTypeDef,
         "StepExecutionId": str,
         "OverriddenParameters": Dict[str, List[str]],
         "IsEnd": bool,
         "NextStep": str,
         "IsCritical": bool,
         "ValidNextSteps": List[str],
-        "Targets": List[TargetTypeDef],
-        "TargetLocation": TargetLocationTypeDef,
+        "Targets": List[TargetOutputTypeDef],
+        "TargetLocation": TargetLocationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
-_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAssociationRequestRequestTypeDef",
+_RequiredCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_RequiredCreateAssociationBatchRequestEntryTypeDef",
     {
-        "AssociationId": str,
+        "Name": str,
     },
 )
-_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAssociationRequestRequestTypeDef",
+_OptionalCreateAssociationBatchRequestEntryTypeDef = TypedDict(
+    "_OptionalCreateAssociationBatchRequestEntryTypeDef",
     {
+        "InstanceId": str,
         "Parameters": Mapping[str, Sequence[str]],
+        "AutomationTargetParameterName": str,
         "DocumentVersion": str,
+        "Targets": Sequence[TargetTypeDef],
         "ScheduleExpression": str,
         "OutputLocation": InstanceAssociationOutputLocationTypeDef,
-        "Name": str,
-        "Targets": Sequence[TargetTypeDef],
         "AssociationName": str,
-        "AssociationVersion": str,
-        "AutomationTargetParameterName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": Sequence[str],
         "TargetLocations": Sequence[TargetLocationTypeDef],
         "ScheduleOffset": int,
         "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "AlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-class UpdateAssociationRequestRequestTypeDef(
-    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
+
+class CreateAssociationBatchRequestEntryTypeDef(
+    _RequiredCreateAssociationBatchRequestEntryTypeDef,
+    _OptionalCreateAssociationBatchRequestEntryTypeDef,
 ):
     pass
 
-GetMaintenanceWindowTaskResultTypeDef = TypedDict(
-    "GetMaintenanceWindowTaskResultTypeDef",
-    {
-        "WindowId": str,
-        "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
-        "TaskArn": str,
-        "ServiceRoleArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
-        "MaxConcurrency": str,
-        "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+_RequiredRunbookTypeDef = TypedDict(
+    "_RequiredRunbookTypeDef",
     {
-        "WindowId": str,
-        "TaskArn": str,
-        "TaskType": MaintenanceWindowTaskTypeType,
+        "DocumentName": str,
     },
 )
-_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+_OptionalRunbookTypeDef = TypedDict(
+    "_OptionalRunbookTypeDef",
     {
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "TargetParameterName": str,
         "Targets": Sequence[TargetTypeDef],
-        "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
-        "Priority": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoTypeDef,
-        "Name": str,
-        "Description": str,
-        "ClientToken": str,
-        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "TargetLocations": Sequence[TargetLocationTypeDef],
     },
     total=False,
 )
 
-class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
-    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-):
+
+class RunbookTypeDef(_RequiredRunbookTypeDef, _OptionalRunbookTypeDef):
     pass
 
-_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+
+TargetLocationUnionTypeDef = Union[TargetLocationTypeDef, TargetLocationOutputTypeDef]
+GetMaintenanceWindowTaskResultTypeDef = TypedDict(
+    "GetMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-    },
-)
-_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
-    {
-        "Targets": Sequence[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "TaskType": MaintenanceWindowTaskTypeType,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
-        "Replace": bool,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
-    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
-):
-    pass
-
 UpdateMaintenanceWindowTaskResultTypeDef = TypedDict(
     "UpdateMaintenanceWindowTaskResultTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TaskArn": str,
         "ServiceRoleArn": str,
-        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionTypeDef],
-        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceSummariesResultTypeDef = TypedDict(
     "ListComplianceSummariesResultTypeDef",
     {
         "ComplianceSummaryItems": List[ComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceComplianceSummariesResultTypeDef = TypedDict(
     "ListResourceComplianceSummariesResultTypeDef",
     {
         "ResourceComplianceSummaryItems": List[ResourceComplianceSummaryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDocumentMetadataHistoryResponseTypeDef = TypedDict(
     "ListDocumentMetadataHistoryResponseTypeDef",
     {
         "Name": str,
         "DocumentVersion": str,
         "Author": str,
         "Metadata": DocumentMetadataResponseInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceAssociationsStatusResultTypeDef = TypedDict(
     "DescribeInstanceAssociationsStatusResultTypeDef",
     {
         "InstanceAssociationStatusInfos": List[InstanceAssociationStatusInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInventoryDeletionsResultTypeDef = TypedDict(
     "DescribeInventoryDeletionsResultTypeDef",
     {
         "InventoryDeletions": List[InventoryDeletionStatusItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MaintenanceWindowTaskInvocationParametersUnionTypeDef = Union[
+    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
+]
+_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "TaskArn": str,
+        "TaskType": MaintenanceWindowTaskTypeType,
+    },
+)
+_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ServiceRoleArn": str,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "ClientToken": str,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class RegisterTaskWithMaintenanceWindowRequestRequestTypeDef(
+    _RequiredRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    _OptionalRegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    {
+        "WindowId": str,
+        "WindowTaskId": str,
+    },
+)
+_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef",
+    {
+        "Targets": Sequence[TargetUnionTypeDef],
+        "TaskArn": str,
+        "ServiceRoleArn": str,
+        "TaskParameters": Mapping[str, MaintenanceWindowTaskParameterValueExpressionUnionTypeDef],
+        "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersTypeDef,
+        "Priority": int,
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "LoggingInfo": LoggingInfoTypeDef,
+        "Name": str,
+        "Description": str,
+        "Replace": bool,
+        "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateMaintenanceWindowTaskRequestRequestTypeDef(
+    _RequiredUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    _OptionalUpdateMaintenanceWindowTaskRequestRequestTypeDef,
+):
+    pass
+
+
+PatchRuleGroupOutputTypeDef = TypedDict(
+    "PatchRuleGroupOutputTypeDef",
+    {
+        "PatchRules": List[PatchRuleOutputTypeDef],
     },
 )
 
 PatchRuleGroupTypeDef = TypedDict(
     "PatchRuleGroupTypeDef",
     {
         "PatchRules": Sequence[PatchRuleTypeDef],
     },
 )
 
+ResourceDataSyncItemTypeDef = TypedDict(
+    "ResourceDataSyncItemTypeDef",
+    {
+        "SyncName": str,
+        "SyncType": str,
+        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
+        "LastSyncTime": datetime,
+        "LastSuccessfulSyncTime": datetime,
+        "SyncLastModifiedTime": datetime,
+        "LastStatus": LastResourceDataSyncStatusType,
+        "SyncCreatedTime": datetime,
+        "LastSyncStatusMessage": str,
+    },
+    total=False,
+)
+
 _RequiredCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
     },
 )
 _OptionalCreateResourceDataSyncRequestRequestTypeDef = TypedDict(
@@ -6531,98 +7009,76 @@
         "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
     total=False,
 )
 
+
 class CreateResourceDataSyncRequestRequestTypeDef(
     _RequiredCreateResourceDataSyncRequestRequestTypeDef,
     _OptionalCreateResourceDataSyncRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateResourceDataSyncRequestRequestTypeDef = TypedDict(
     "UpdateResourceDataSyncRequestRequestTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceTypeDef,
     },
 )
 
-ResourceDataSyncItemTypeDef = TypedDict(
-    "ResourceDataSyncItemTypeDef",
-    {
-        "SyncName": str,
-        "SyncType": str,
-        "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
-        "LastSyncTime": datetime,
-        "LastSuccessfulSyncTime": datetime,
-        "SyncLastModifiedTime": datetime,
-        "LastStatus": LastResourceDataSyncStatusType,
-        "SyncCreatedTime": datetime,
-        "LastSyncStatusMessage": str,
-    },
-    total=False,
-)
-
 CreateAssociationResultTypeDef = TypedDict(
     "CreateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAssociationResultTypeDef = TypedDict(
     "DescribeAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationResultTypeDef = TypedDict(
     "UpdateAssociationResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssociationStatusResultTypeDef = TypedDict(
     "UpdateAssociationStatusResultTypeDef",
     {
         "AssociationDescription": AssociationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociationVersionsResultTypeDef = TypedDict(
     "ListAssociationVersionsResultTypeDef",
     {
         "AssociationVersions": List[AssociationVersionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAssociationBatchRequestRequestTypeDef = TypedDict(
-    "CreateAssociationBatchRequestRequestTypeDef",
-    {
-        "Entries": Sequence[CreateAssociationBatchRequestEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedCreateAssociationTypeDef = TypedDict(
     "FailedCreateAssociationTypeDef",
     {
-        "Entry": CreateAssociationBatchRequestEntryTypeDef,
+        "Entry": CreateAssociationBatchRequestEntryOutputTypeDef,
         "Message": str,
         "Fault": FaultType,
     },
     total=False,
 )
 
 AutomationExecutionMetadataTypeDef = TypedDict(
@@ -6639,62 +7095,33 @@
         "Outputs": Dict[str, List[str]],
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "FailureMessage": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
         "AutomationType": AutomationTypeType,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
-_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "DocumentName": str,
-        "Runbooks": Sequence[RunbookTypeDef],
-    },
-)
-_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
-    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
-    {
-        "ScheduledTime": Union[datetime, str],
-        "DocumentVersion": str,
-        "Parameters": Mapping[str, Sequence[str]],
-        "ChangeRequestName": str,
-        "ClientToken": str,
-        "AutoApprove": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ScheduledEndTime": Union[datetime, str],
-        "ChangeDetails": str,
-    },
-    total=False,
-)
-
-class StartChangeRequestExecutionRequestRequestTypeDef(
-    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
-    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
-):
-    pass
-
 AutomationExecutionTypeDef = TypedDict(
     "AutomationExecutionTypeDef",
     {
         "AutomationExecutionId": str,
         "DocumentName": str,
         "DocumentVersion": str,
         "ExecutionStartTime": datetime,
@@ -6707,40 +7134,198 @@
         "FailureMessage": str,
         "Mode": ExecutionModeType,
         "ParentAutomationExecutionId": str,
         "ExecutedBy": str,
         "CurrentStepName": str,
         "CurrentAction": str,
         "TargetParameterName": str,
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "TargetMaps": List[Dict[str, List[str]]],
         "ResolvedTargets": ResolvedTargetsTypeDef,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Target": str,
-        "TargetLocations": List[TargetLocationTypeDef],
+        "TargetLocations": List[TargetLocationOutputTypeDef],
         "ProgressCounters": ProgressCountersTypeDef,
-        "AlarmConfiguration": AlarmConfigurationTypeDef,
+        "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
         "AutomationSubtype": Literal["ChangeRequest"],
         "ScheduledTime": datetime,
-        "Runbooks": List[RunbookTypeDef],
+        "Runbooks": List[RunbookOutputTypeDef],
         "OpsItemId": str,
         "AssociationId": str,
         "ChangeRequestName": str,
     },
     total=False,
 )
 
 DescribeAutomationStepExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationStepExecutionsResultTypeDef",
     {
         "StepExecutions": List[StepExecutionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssociationBatchRequestEntryUnionTypeDef = Union[
+    CreateAssociationBatchRequestEntryTypeDef, CreateAssociationBatchRequestEntryOutputTypeDef
+]
+RunbookUnionTypeDef = Union[RunbookTypeDef, RunbookOutputTypeDef]
+_RequiredCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssociationRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssociationRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "InstanceId": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "Targets": Sequence[TargetUnionTypeDef],
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "AssociationName": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAssociationRequestRequestTypeDef(
+    _RequiredCreateAssociationRequestRequestTypeDef, _OptionalCreateAssociationRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+    },
+)
+_OptionalStartAutomationExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartAutomationExecutionRequestRequestTypeDef",
+    {
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ClientToken": str,
+        "Mode": ExecutionModeType,
+        "TargetParameterName": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "MaxConcurrency": str,
+        "MaxErrors": str,
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class StartAutomationExecutionRequestRequestTypeDef(
+    _RequiredStartAutomationExecutionRequestRequestTypeDef,
+    _OptionalStartAutomationExecutionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAssociationRequestRequestTypeDef",
+    {
+        "AssociationId": str,
+    },
+)
+_OptionalUpdateAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAssociationRequestRequestTypeDef",
+    {
+        "Parameters": Mapping[str, Sequence[str]],
+        "DocumentVersion": str,
+        "ScheduleExpression": str,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
+        "Name": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+        "AssociationName": str,
+        "AssociationVersion": str,
+        "AutomationTargetParameterName": str,
+        "MaxErrors": str,
+        "MaxConcurrency": str,
+        "ComplianceSeverity": AssociationComplianceSeverityType,
+        "SyncCompliance": AssociationSyncComplianceType,
+        "ApplyOnlyAtCronInterval": bool,
+        "CalendarNames": Sequence[str],
+        "TargetLocations": Sequence[TargetLocationUnionTypeDef],
+        "ScheduleOffset": int,
+        "TargetMaps": Sequence[Mapping[str, Sequence[str]]],
+        "AlarmConfiguration": AlarmConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateAssociationRequestRequestTypeDef(
+    _RequiredUpdateAssociationRequestRequestTypeDef, _OptionalUpdateAssociationRequestRequestTypeDef
+):
+    pass
+
+
+GetPatchBaselineResultTypeDef = TypedDict(
+    "GetPatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "PatchGroups": List[str],
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePatchBaselineResultTypeDef = TypedDict(
+    "UpdatePatchBaselineResultTypeDef",
+    {
+        "BaselineId": str,
+        "Name": str,
+        "OperatingSystem": OperatingSystemType,
+        "GlobalFilters": PatchFilterGroupOutputTypeDef,
+        "ApprovalRules": PatchRuleGroupOutputTypeDef,
+        "ApprovedPatches": List[str],
+        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
+        "ApprovedPatchesEnableNonSecurity": bool,
+        "RejectedPatches": List[str],
+        "RejectedPatchesAction": PatchActionType,
+        "CreatedDate": datetime,
+        "ModifiedDate": datetime,
+        "Description": str,
+        "Sources": List[PatchSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BaselineOverrideTypeDef = TypedDict(
     "BaselineOverrideTypeDef",
     {
         "OperatingSystem": OperatingSystemType,
@@ -6770,49 +7355,30 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePatchBaselineRequestRequestTypeDef(
     _RequiredCreatePatchBaselineRequestRequestTypeDef,
     _OptionalCreatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-GetPatchBaselineResultTypeDef = TypedDict(
-    "GetPatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "PatchGroups": List[str],
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
+PatchRuleGroupUnionTypeDef = Union[PatchRuleGroupTypeDef, PatchRuleGroupOutputTypeDef]
 _RequiredUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePatchBaselineRequestRequestTypeDef",
     {
         "BaselineId": str,
     },
 )
 _OptionalUpdatePatchBaselineRequestRequestTypeDef = TypedDict(
@@ -6823,81 +7389,100 @@
         "ApprovalRules": PatchRuleGroupTypeDef,
         "ApprovedPatches": Sequence[str],
         "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
         "ApprovedPatchesEnableNonSecurity": bool,
         "RejectedPatches": Sequence[str],
         "RejectedPatchesAction": PatchActionType,
         "Description": str,
-        "Sources": Sequence[PatchSourceTypeDef],
+        "Sources": Sequence[PatchSourceUnionTypeDef],
         "Replace": bool,
     },
     total=False,
 )
 
+
 class UpdatePatchBaselineRequestRequestTypeDef(
     _RequiredUpdatePatchBaselineRequestRequestTypeDef,
     _OptionalUpdatePatchBaselineRequestRequestTypeDef,
 ):
     pass
 
-UpdatePatchBaselineResultTypeDef = TypedDict(
-    "UpdatePatchBaselineResultTypeDef",
-    {
-        "BaselineId": str,
-        "Name": str,
-        "OperatingSystem": OperatingSystemType,
-        "GlobalFilters": PatchFilterGroupTypeDef,
-        "ApprovalRules": PatchRuleGroupTypeDef,
-        "ApprovedPatches": List[str],
-        "ApprovedPatchesComplianceLevel": PatchComplianceLevelType,
-        "ApprovedPatchesEnableNonSecurity": bool,
-        "RejectedPatches": List[str],
-        "RejectedPatchesAction": PatchActionType,
-        "CreatedDate": datetime,
-        "ModifiedDate": datetime,
-        "Description": str,
-        "Sources": List[PatchSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListResourceDataSyncResultTypeDef = TypedDict(
     "ListResourceDataSyncResultTypeDef",
     {
         "ResourceDataSyncItems": List[ResourceDataSyncItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssociationBatchResultTypeDef = TypedDict(
     "CreateAssociationBatchResultTypeDef",
     {
         "Successful": List[AssociationDescriptionTypeDef],
         "Failed": List[FailedCreateAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAutomationExecutionsResultTypeDef = TypedDict(
     "DescribeAutomationExecutionsResultTypeDef",
     {
         "AutomationExecutionMetadataList": List[AutomationExecutionMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutomationExecutionResultTypeDef = TypedDict(
     "GetAutomationExecutionResultTypeDef",
     {
         "AutomationExecution": AutomationExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssociationBatchRequestRequestTypeDef = TypedDict(
+    "CreateAssociationBatchRequestRequestTypeDef",
+    {
+        "Entries": Sequence[CreateAssociationBatchRequestEntryUnionTypeDef],
+    },
+)
+
+_RequiredStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_RequiredStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "DocumentName": str,
+        "Runbooks": Sequence[RunbookUnionTypeDef],
     },
 )
+_OptionalStartChangeRequestExecutionRequestRequestTypeDef = TypedDict(
+    "_OptionalStartChangeRequestExecutionRequestRequestTypeDef",
+    {
+        "ScheduledTime": TimestampTypeDef,
+        "DocumentVersion": str,
+        "Parameters": Mapping[str, Sequence[str]],
+        "ChangeRequestName": str,
+        "ClientToken": str,
+        "AutoApprove": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ScheduledEndTime": TimestampTypeDef,
+        "ChangeDetails": str,
+    },
+    total=False,
+)
+
+
+class StartChangeRequestExecutionRequestRequestTypeDef(
+    _RequiredStartChangeRequestExecutionRequestRequestTypeDef,
+    _OptionalStartChangeRequestExecutionRequestRequestTypeDef,
+):
+    pass
+
 
 _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
         "SnapshotId": str,
     },
@@ -6906,12 +7491,13 @@
     "_OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef",
     {
         "BaselineOverride": BaselineOverrideTypeDef,
     },
     total=False,
 )
 
+
 class GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef(
     _RequiredGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
     _OptionalGetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 ):
     pass
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/waiter.py` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm/waiter.pyi` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/PKG-INFO` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ssm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ssm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ssm"></a>
 
 # types-aiobotocore-ssm
 
 [![PyPI - types-aiobotocore-ssm](https://img.shields.io/pypi/v/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm)](https://pepy.tech/project/types-aiobotocore-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [types-aiobotocore-ssm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm/).
 
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
@@ -639,306 +638,311 @@
 )
 
 
 def check_value(value: AssociationComplianceSeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ssm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ssm.type_defs import (
     AccountSharingInfoTypeDef,
     TagTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
-    AssociateOpsItemRelatedItemResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
-    AssociationStatusTypeDef,
-    TargetTypeDef,
+    AssociationStatusOutputTypeDef,
+    TargetOutputTypeDef,
     AssociationExecutionFilterTypeDef,
     OutputSourceTypeDef,
     AssociationExecutionTargetsFilterTypeDef,
     AssociationFilterTypeDef,
+    TimestampTypeDef,
     AttachmentContentTypeDef,
     AttachmentInformationTypeDef,
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
+    BlobTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CancelMaintenanceWindowExecutionResultTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
-    NotificationConfigTypeDef,
-    ComplianceExecutionSummaryTypeDef,
+    NotificationConfigOutputTypeDef,
+    ComplianceExecutionSummaryOutputTypeDef,
     ComplianceItemEntryTypeDef,
     ComplianceStringFilterTypeDef,
     SeveritySummaryTypeDef,
     RegistrationMetadataItemTypeDef,
-    CreateActivationResultTypeDef,
+    TargetTypeDef,
     DocumentRequiresTypeDef,
-    CreateMaintenanceWindowResultTypeDef,
     OpsItemDataValueTypeDef,
     OpsItemNotificationTypeDef,
     RelatedOpsItemTypeDef,
-    CreateOpsItemResponseTypeDef,
     MetadataValueTypeDef,
-    CreateOpsMetadataResultTypeDef,
-    CreatePatchBaselineResultTypeDef,
     DeleteActivationRequestRequestTypeDef,
     DeleteAssociationRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteInventoryRequestRequestTypeDef,
     DeleteMaintenanceWindowRequestRequestTypeDef,
-    DeleteMaintenanceWindowResultTypeDef,
     DeleteOpsMetadataRequestRequestTypeDef,
     DeleteParameterRequestRequestTypeDef,
     DeleteParametersRequestRequestTypeDef,
-    DeleteParametersResultTypeDef,
     DeletePatchBaselineRequestRequestTypeDef,
-    DeletePatchBaselineResultTypeDef,
     DeleteResourceDataSyncRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeregisterManagedInstanceRequestRequestTypeDef,
     DeregisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    DeregisterPatchBaselineForPatchGroupResultTypeDef,
     DeregisterTargetFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTargetFromMaintenanceWindowResultTypeDef,
     DeregisterTaskFromMaintenanceWindowRequestRequestTypeDef,
-    DeregisterTaskFromMaintenanceWindowResultTypeDef,
     DescribeActivationsFilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAssociationRequestRequestTypeDef,
     StepExecutionFilterTypeDef,
     PatchOrchestratorFilterTypeDef,
     PatchTypeDef,
     DescribeDocumentPermissionRequestRequestTypeDef,
     DescribeDocumentRequestRequestTypeDef,
-    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestRequestTypeDef,
     InstanceAssociationTypeDef,
-    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
     DescribeEffectivePatchesForPatchBaselineRequestRequestTypeDef,
-    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
     DescribeInstanceAssociationsStatusRequestRequestTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
     InstancePatchStateTypeDef,
-    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
     DescribeInstancePatchStatesRequestRequestTypeDef,
     PatchComplianceDataTypeDef,
-    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
     DescribeInventoryDeletionsRequestRequestTypeDef,
     MaintenanceWindowFilterTypeDef,
     MaintenanceWindowExecutionTaskInvocationIdentityTypeDef,
     MaintenanceWindowExecutionTypeDef,
     ScheduledWindowExecutionTypeDef,
     MaintenanceWindowIdentityForTargetTypeDef,
     MaintenanceWindowIdentityTypeDef,
     OpsItemFilterTypeDef,
     ParameterStringFilterTypeDef,
     ParametersFilterTypeDef,
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
-    DescribePatchGroupStateResultTypeDef,
-    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
-    DescribePatchPropertiesResultTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
-    GetCalendarStateResponseTypeDef,
     WaiterConfigTypeDef,
     GetCommandInvocationRequestRequestTypeDef,
     GetConnectionStatusRequestRequestTypeDef,
-    GetConnectionStatusResponseTypeDef,
     GetDefaultPatchBaselineRequestRequestTypeDef,
-    GetDefaultPatchBaselineResultTypeDef,
-    GetDeployablePatchSnapshotForInstanceResultTypeDef,
     GetDocumentRequestRequestTypeDef,
     InventoryFilterTypeDef,
     ResultAttributeTypeDef,
-    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionResultTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
-    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
-    MaintenanceWindowTaskParameterValueExpressionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
-    GetMaintenanceWindowResultTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
     LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
-    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
-    GetPatchBaselineForPatchGroupResultTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
-    LabelParameterVersionResultTypeDef,
-    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
     ListAssociationVersionsRequestRequestTypeDef,
     ListDocumentMetadataHistoryRequestRequestTypeDef,
-    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
     ListDocumentVersionsRequestRequestTypeDef,
-    ListInventoryEntriesResultTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
-    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
-    MaintenanceWindowLambdaParametersTypeDef,
+    MaintenanceWindowLambdaParametersOutputTypeDef,
+    NotificationConfigTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
     OpsItemIdentityTypeDef,
-    PaginatorConfigTypeDef,
     ParameterInlinePolicyTypeDef,
+    PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
-    PutInventoryResultTypeDef,
-    PutParameterResultTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
-    RegisterDefaultPatchBaselineResultTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
-    RegisterPatchBaselineForPatchGroupResultTypeDef,
-    RegisterTargetWithMaintenanceWindowResultTypeDef,
-    RegisterTaskWithMaintenanceWindowResultTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
-    ResponseMetadataTypeDef,
     ResumeSessionRequestRequestTypeDef,
-    ResumeSessionResponseTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
-    StartAutomationExecutionResultTypeDef,
-    StartChangeRequestExecutionResultTypeDef,
     StartSessionRequestRequestTypeDef,
-    StartSessionResponseTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UnlabelParameterVersionRequestRequestTypeDef,
-    UnlabelParameterVersionResultTypeDef,
     UpdateDocumentDefaultVersionRequestRequestTypeDef,
     UpdateMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowResultTypeDef,
     UpdateManagedInstanceRoleRequestRequestTypeDef,
-    UpdateOpsMetadataResultTypeDef,
     UpdateServiceSettingRequestRequestTypeDef,
-    DescribeDocumentPermissionResponseTypeDef,
     ActivationTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateMaintenanceWindowRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     PutParameterRequestRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
-    UpdateAssociationStatusRequestRequestTypeDef,
+    AssociateOpsItemRelatedItemResponseTypeDef,
+    CancelMaintenanceWindowExecutionResultTypeDef,
+    CreateActivationResultTypeDef,
+    CreateMaintenanceWindowResultTypeDef,
+    CreateOpsItemResponseTypeDef,
+    CreateOpsMetadataResultTypeDef,
+    CreatePatchBaselineResultTypeDef,
+    DeleteMaintenanceWindowResultTypeDef,
+    DeleteParametersResultTypeDef,
+    DeletePatchBaselineResultTypeDef,
+    DeregisterPatchBaselineForPatchGroupResultTypeDef,
+    DeregisterTargetFromMaintenanceWindowResultTypeDef,
+    DeregisterTaskFromMaintenanceWindowResultTypeDef,
+    DescribeDocumentPermissionResponseTypeDef,
+    DescribePatchGroupStateResultTypeDef,
+    DescribePatchPropertiesResultTypeDef,
+    GetCalendarStateResponseTypeDef,
+    GetConnectionStatusResponseTypeDef,
+    GetDefaultPatchBaselineResultTypeDef,
+    GetDeployablePatchSnapshotForInstanceResultTypeDef,
+    GetMaintenanceWindowExecutionResultTypeDef,
+    GetMaintenanceWindowExecutionTaskInvocationResultTypeDef,
+    GetMaintenanceWindowResultTypeDef,
+    GetPatchBaselineForPatchGroupResultTypeDef,
+    LabelParameterVersionResultTypeDef,
+    ListInventoryEntriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    PutInventoryResultTypeDef,
+    PutParameterResultTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    RegisterDefaultPatchBaselineResultTypeDef,
+    RegisterPatchBaselineForPatchGroupResultTypeDef,
+    RegisterTargetWithMaintenanceWindowResultTypeDef,
+    RegisterTaskWithMaintenanceWindowResultTypeDef,
+    ResumeSessionResponseTypeDef,
+    StartAutomationExecutionResultTypeDef,
+    StartChangeRequestExecutionResultTypeDef,
+    StartSessionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
+    UnlabelParameterVersionResultTypeDef,
+    UpdateMaintenanceWindowResultTypeDef,
+    UpdateOpsMetadataResultTypeDef,
     AssociationTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
-    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     MaintenanceWindowTargetTypeDef,
-    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetResultTypeDef,
-    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAssociationExecutionsRequestRequestTypeDef,
     AssociationExecutionTargetTypeDef,
-    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestRequestTypeDef,
-    ListAssociationsRequestListAssociationsPaginateTypeDef,
     ListAssociationsRequestRequestTypeDef,
+    AssociationStatusTypeDef,
+    ComplianceExecutionSummaryTypeDef,
     UpdateDocumentRequestRequestTypeDef,
-    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestRequestTypeDef,
+    MaintenanceWindowLambdaParametersTypeDef,
     GetCommandInvocationResultTypeDef,
-    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
     ListCommandInvocationsRequestRequestTypeDef,
-    ListCommandsRequestListCommandsPaginateTypeDef,
     ListCommandsRequestRequestTypeDef,
     CommandInvocationTypeDef,
-    MaintenanceWindowRunCommandParametersTypeDef,
+    MaintenanceWindowRunCommandParametersOutputTypeDef,
     ComplianceItemTypeDef,
-    PutComplianceItemsRequestRequestTypeDef,
-    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
     ListComplianceItemsRequestRequestTypeDef,
-    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
     ListComplianceSummariesRequestRequestTypeDef,
-    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
     ListResourceComplianceSummariesRequestRequestTypeDef,
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
+    TargetUnionTypeDef,
     CreateDocumentRequestRequestTypeDef,
     DocumentIdentifierTypeDef,
     GetDocumentResultTypeDef,
     OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
     OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
     GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
-    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeActivationsRequestRequestTypeDef,
+    DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
+    DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
+    DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
+    DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
+    DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
+    DescribeEffectivePatchesForPatchBaselineRequestDescribeEffectivePatchesForPatchBaselinePaginateTypeDef,
+    DescribeInstanceAssociationsStatusRequestDescribeInstanceAssociationsStatusPaginateTypeDef,
+    DescribeInstancePatchStatesRequestDescribeInstancePatchStatesPaginateTypeDef,
+    DescribeInventoryDeletionsRequestDescribeInventoryDeletionsPaginateTypeDef,
+    DescribePatchPropertiesRequestDescribePatchPropertiesPaginateTypeDef,
+    GetInventorySchemaRequestGetInventorySchemaPaginateTypeDef,
+    GetParameterHistoryRequestGetParameterHistoryPaginateTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    ListAssociationVersionsRequestListAssociationVersionsPaginateTypeDef,
+    ListAssociationsRequestListAssociationsPaginateTypeDef,
+    ListCommandInvocationsRequestListCommandInvocationsPaginateTypeDef,
+    ListCommandsRequestListCommandsPaginateTypeDef,
+    ListComplianceItemsRequestListComplianceItemsPaginateTypeDef,
+    ListComplianceSummariesRequestListComplianceSummariesPaginateTypeDef,
+    ListDocumentVersionsRequestListDocumentVersionsPaginateTypeDef,
+    ListResourceComplianceSummariesRequestListResourceComplianceSummariesPaginateTypeDef,
+    ListResourceDataSyncRequestListResourceDataSyncPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestDescribeAutomationStepExecutionsPaginateTypeDef,
     DescribeAutomationStepExecutionsRequestRequestTypeDef,
     DescribeAvailablePatchesRequestDescribeAvailablePatchesPaginateTypeDef,
     DescribeAvailablePatchesRequestRequestTypeDef,
     DescribeInstancePatchesRequestDescribeInstancePatchesPaginateTypeDef,
     DescribeInstancePatchesRequestRequestTypeDef,
-    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
-    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
     DescribePatchBaselinesRequestDescribePatchBaselinesPaginateTypeDef,
     DescribePatchBaselinesRequestRequestTypeDef,
     DescribePatchGroupsRequestDescribePatchGroupsPaginateTypeDef,
     DescribePatchGroupsRequestRequestTypeDef,
     DescribeAvailablePatchesResultTypeDef,
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef,
@@ -990,14 +994,15 @@
     GetInventoryRequestRequestTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
+    PatchSourceUnionTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
@@ -1007,39 +1012,56 @@
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
     ListOpsItemEventsRequestRequestTypeDef,
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
+    MaintenanceWindowRunCommandParametersTypeDef,
+    NotificationConfigUnionTypeDef,
+    MaintenanceWindowTaskParameterValueExpressionUnionTypeDef,
     OpsEntityTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
+    PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
+    ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
     MaintenanceWindowTaskTypeDef,
-    SendCommandRequestRequestTypeDef,
+    TargetLocationOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
     TargetLocationTypeDef,
     ListAssociationsResultTypeDef,
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
+    AssociationStatusUnionTypeDef,
+    UpdateAssociationStatusRequestRequestTypeDef,
+    ComplianceExecutionSummaryUnionTypeDef,
+    PutComplianceItemsRequestRequestTypeDef,
     ListCommandInvocationsResultTypeDef,
-    MaintenanceWindowTaskInvocationParametersTypeDef,
+    MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
+    DescribeMaintenanceWindowScheduleRequestDescribeMaintenanceWindowSchedulePaginateTypeDef,
+    DescribeMaintenanceWindowScheduleRequestRequestTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestDescribeMaintenanceWindowsForTargetPaginateTypeDef,
+    DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
+    RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
+    SendCommandRequestRequestTypeDef,
+    UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     ListDocumentsResultTypeDef,
     DescribeOpsItemsResponseTypeDef,
     GetOpsItemResponseTypeDef,
     DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
@@ -1049,74 +1071,85 @@
     InventoryAggregatorTypeDef,
     DescribeInstanceInformationResultTypeDef,
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
+    PatchRuleOutputTypeDef,
+    PatchFilterGroupUnionTypeDef,
     PatchRuleTypeDef,
-    ResourceDataSyncSourceTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
+    ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
     DescribeAssociationExecutionsResultTypeDef,
     ListCommandsResultTypeDef,
     SendCommandResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowTasksResultTypeDef,
     AssociationDescriptionTypeDef,
     AssociationVersionInfoTypeDef,
+    CreateAssociationBatchRequestEntryOutputTypeDef,
+    RunbookOutputTypeDef,
+    StepExecutionTypeDef,
     CreateAssociationBatchRequestEntryTypeDef,
-    CreateAssociationRequestRequestTypeDef,
     RunbookTypeDef,
-    StartAutomationExecutionRequestRequestTypeDef,
-    StepExecutionTypeDef,
-    UpdateAssociationRequestRequestTypeDef,
+    TargetLocationUnionTypeDef,
     GetMaintenanceWindowTaskResultTypeDef,
-    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
-    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
     UpdateMaintenanceWindowTaskResultTypeDef,
     ListComplianceSummariesResultTypeDef,
     ListResourceComplianceSummariesResultTypeDef,
     ListDocumentMetadataHistoryResponseTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
+    MaintenanceWindowTaskInvocationParametersUnionTypeDef,
+    RegisterTaskWithMaintenanceWindowRequestRequestTypeDef,
+    UpdateMaintenanceWindowTaskRequestRequestTypeDef,
+    PatchRuleGroupOutputTypeDef,
     PatchRuleGroupTypeDef,
+    ResourceDataSyncItemTypeDef,
     CreateResourceDataSyncRequestRequestTypeDef,
     UpdateResourceDataSyncRequestRequestTypeDef,
-    ResourceDataSyncItemTypeDef,
     CreateAssociationResultTypeDef,
     DescribeAssociationResultTypeDef,
     UpdateAssociationResultTypeDef,
     UpdateAssociationStatusResultTypeDef,
     ListAssociationVersionsResultTypeDef,
-    CreateAssociationBatchRequestRequestTypeDef,
     FailedCreateAssociationTypeDef,
     AutomationExecutionMetadataTypeDef,
-    StartChangeRequestExecutionRequestRequestTypeDef,
     AutomationExecutionTypeDef,
     DescribeAutomationStepExecutionsResultTypeDef,
+    CreateAssociationBatchRequestEntryUnionTypeDef,
+    RunbookUnionTypeDef,
+    CreateAssociationRequestRequestTypeDef,
+    StartAutomationExecutionRequestRequestTypeDef,
+    UpdateAssociationRequestRequestTypeDef,
+    GetPatchBaselineResultTypeDef,
+    UpdatePatchBaselineResultTypeDef,
     BaselineOverrideTypeDef,
     CreatePatchBaselineRequestRequestTypeDef,
-    GetPatchBaselineResultTypeDef,
+    PatchRuleGroupUnionTypeDef,
     UpdatePatchBaselineRequestRequestTypeDef,
-    UpdatePatchBaselineResultTypeDef,
     ListResourceDataSyncResultTypeDef,
     CreateAssociationBatchResultTypeDef,
     DescribeAutomationExecutionsResultTypeDef,
     GetAutomationExecutionResultTypeDef,
+    CreateAssociationBatchRequestRequestTypeDef,
+    StartChangeRequestExecutionRequestRequestTypeDef,
     GetDeployablePatchSnapshotForInstanceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSharingInfoTypeDef:
+def get_value() -> AccountSharingInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ssm-2.5.2/types_aiobotocore_ssm.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-2.5.2.post1/types_aiobotocore_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


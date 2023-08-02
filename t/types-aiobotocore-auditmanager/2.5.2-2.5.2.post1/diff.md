# Comparing `tmp/types-aiobotocore-auditmanager-2.5.2.tar.gz` & `tmp/types-aiobotocore-auditmanager-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-auditmanager-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-auditmanager-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-auditmanager-2.5.2.tar` & `types-aiobotocore-auditmanager-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.697734 types-aiobotocore-auditmanager-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-07-08 01:43:16.697734 types-aiobotocore-auditmanager-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.697734 types-aiobotocore-auditmanager-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.697734 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45840 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45770 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57845 2023-07-08 01:26:09.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57800 2023-07-08 01:26:08.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:07.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.697734 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-07-08 01:43:16.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-08 01:43:16.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:16.000000 types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45855 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45785 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58050 2023-08-02 14:33:35.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58005 2023-08-02 14:33:35.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/LICENSE` & `types-aiobotocore-auditmanager-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2/PKG-INFO` & `types-aiobotocore-auditmanager-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-auditmanager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AuditManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AuditManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore auditmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore auditmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-auditmanager"></a>
 
 # types-aiobotocore-auditmanager
 
 [![PyPI - types-aiobotocore-auditmanager](https://img.shields.io/pypi/v/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-auditmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-auditmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AuditManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [types-aiobotocore-auditmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/).
 
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
@@ -305,20 +304,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_auditmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_auditmanager.type_defs import (
     AWSAccountTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
     RoleTypeDef,
@@ -329,14 +328,15 @@
     FrameworkMetadataTypeDef,
     AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
@@ -347,84 +347,84 @@
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
-    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFileUploadUrlRequestRequestTypeDef,
-    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
-    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
+    DeregisterAccountResponseTypeDef,
+    GetAccountStatusResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    ListAssessmentFrameworksResponseTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ListAssessmentFrameworkShareRequestsResponseTypeDef,
+    ListAssessmentFrameworksResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterAccountResponseTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
@@ -442,14 +442,15 @@
     GetAssessmentReportUrlResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetServicesInScopeResponseTypeDef,
     ListNotificationsResponseTypeDef,
     AssessmentMetadataTypeDef,
     CreateAssessmentRequestRequestTypeDef,
+    ScopeUnionTypeDef,
     UpdateAssessmentRequestRequestTypeDef,
     ListAssessmentsResponseTypeDef,
     AssessmentControlSetTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     BatchCreateDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlResponseTypeDef,
     ListControlDomainInsightsByAssessmentResponseTypeDef,
@@ -479,15 +480,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_value() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/README.md` & `types-aiobotocore-auditmanager-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-auditmanager"></a>
 
 # types-aiobotocore-auditmanager
 
 [![PyPI - types-aiobotocore-auditmanager](https://img.shields.io/pypi/v/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-auditmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-auditmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AuditManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [types-aiobotocore-auditmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/).
 
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
@@ -272,20 +272,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_auditmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_auditmanager.type_defs import (
     AWSAccountTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
     RoleTypeDef,
@@ -296,14 +296,15 @@
     FrameworkMetadataTypeDef,
     AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
@@ -314,84 +315,84 @@
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
-    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFileUploadUrlRequestRequestTypeDef,
-    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
-    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
+    DeregisterAccountResponseTypeDef,
+    GetAccountStatusResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    ListAssessmentFrameworksResponseTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ListAssessmentFrameworkShareRequestsResponseTypeDef,
+    ListAssessmentFrameworksResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterAccountResponseTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
@@ -409,14 +410,15 @@
     GetAssessmentReportUrlResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetServicesInScopeResponseTypeDef,
     ListNotificationsResponseTypeDef,
     AssessmentMetadataTypeDef,
     CreateAssessmentRequestRequestTypeDef,
+    ScopeUnionTypeDef,
     UpdateAssessmentRequestRequestTypeDef,
     ListAssessmentsResponseTypeDef,
     AssessmentControlSetTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     BatchCreateDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlResponseTypeDef,
     ListControlDomainInsightsByAssessmentResponseTypeDef,
@@ -446,15 +448,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_value() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/setup.py` & `types-aiobotocore-auditmanager-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-auditmanager",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AuditManager 2.5.2 service generated with"
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
-    keywords="aiobotocore auditmanager type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore auditmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_auditmanager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/"
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/__main__.py` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AuditManager 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AuditManager 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/client.py` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
-    ScopeTypeDef,
+    ScopeUnionTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentResponseTypeDef,
@@ -221,15 +221,15 @@
         """
 
     async def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: ScopeTypeDef,
+        scope: ScopeUnionTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -741,15 +741,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#untag_resource)
         """
 
     async def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: ScopeTypeDef,
+        scope: ScopeUnionTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/client.pyi` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
-    ScopeTypeDef,
+    ScopeUnionTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentResponseTypeDef,
@@ -209,15 +209,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#close)
         """
     async def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: ScopeTypeDef,
+        scope: ScopeUnionTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -681,15 +681,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#untag_resource)
         """
     async def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: ScopeTypeDef,
+        scope: ScopeUnionTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/literals.py` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/literals.pyi` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/type_defs.py` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_auditmanager.type_defs import AWSAccountTypeDef
 
-    data: AWSAccountTypeDef = {...}
+    data: AWSAccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountStatusType,
     ActionEnumType,
     AssessmentReportStatusType,
     AssessmentStatusType,
     ControlResponseType,
@@ -63,14 +63,15 @@
     "FrameworkMetadataTypeDef",
     "AssessmentReportsDestinationTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
@@ -81,84 +82,84 @@
     "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
-    "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
-    "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
     "URLTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetChangeLogsRequestRequestTypeDef",
     "GetControlRequestRequestTypeDef",
     "GetDelegationsRequestRequestTypeDef",
     "GetEvidenceByEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
-    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     "GetEvidenceRequestRequestTypeDef",
     "GetInsightsByAssessmentRequestRequestTypeDef",
     "InsightsByAssessmentTypeDef",
     "InsightsTypeDef",
-    "GetOrganizationAdminAccountResponseTypeDef",
     "ServiceMetadataTypeDef",
     "GetSettingsRequestRequestTypeDef",
     "ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef",
     "ListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     "ListAssessmentFrameworksRequestRequestTypeDef",
     "ListAssessmentReportsRequestRequestTypeDef",
     "ListAssessmentsRequestRequestTypeDef",
     "ListControlDomainInsightsByAssessmentRequestRequestTypeDef",
     "ListControlDomainInsightsRequestRequestTypeDef",
     "ListControlInsightsByControlDomainRequestRequestTypeDef",
     "ListControlsRequestRequestTypeDef",
     "ListKeywordsForDataSourceRequestRequestTypeDef",
-    "ListKeywordsForDataSourceResponseTypeDef",
     "ListNotificationsRequestRequestTypeDef",
     "NotificationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegisterAccountRequestRequestTypeDef",
-    "RegisterAccountResponseTypeDef",
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAssessmentFrameworkShareRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    "CreateAssessmentReportResponseTypeDef",
+    "DeregisterAccountResponseTypeDef",
+    "GetAccountStatusResponseTypeDef",
+    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
-    "ListAssessmentFrameworksResponseTypeDef",
+    "GetOrganizationAdminAccountResponseTypeDef",
     "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    "ListAssessmentFrameworksResponseTypeDef",
+    "ListAssessmentReportsResponseTypeDef",
+    "ListKeywordsForDataSourceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterAccountResponseTypeDef",
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     "StartAssessmentFrameworkShareResponseTypeDef",
     "UpdateAssessmentFrameworkShareResponseTypeDef",
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    "ListAssessmentReportsResponseTypeDef",
-    "CreateAssessmentReportResponseTypeDef",
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     "BatchCreateDelegationByAssessmentRequestRequestTypeDef",
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
@@ -176,14 +177,15 @@
     "GetAssessmentReportUrlResponseTypeDef",
     "GetInsightsByAssessmentResponseTypeDef",
     "GetInsightsResponseTypeDef",
     "GetServicesInScopeResponseTypeDef",
     "ListNotificationsResponseTypeDef",
     "AssessmentMetadataTypeDef",
     "CreateAssessmentRequestRequestTypeDef",
+    "ScopeUnionTypeDef",
     "UpdateAssessmentRequestRequestTypeDef",
     "ListAssessmentsResponseTypeDef",
     "AssessmentControlSetTypeDef",
     "UpdateAssessmentControlResponseTypeDef",
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
@@ -409,14 +411,25 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
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
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
         "roleArn": str,
         "roleType": RoleTypeType,
@@ -592,22 +605,14 @@
 DeleteControlRequestRequestTypeDef = TypedDict(
     "DeleteControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
-DeregisterAccountResponseTypeDef = TypedDict(
-    "DeregisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
@@ -645,22 +650,14 @@
         "arn": str,
         "value": str,
         "complianceCheck": str,
     },
     total=False,
 )
 
-GetAccountStatusResponseTypeDef = TypedDict(
-    "GetAccountStatusResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "GetAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
     },
 )
 
@@ -756,23 +753,14 @@
 GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
     {
         "fileName": str,
     },
 )
 
-GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
-    "GetEvidenceFileUploadUrlResponseTypeDef",
-    {
-        "evidenceFileName": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEvidenceFolderRequestRequestTypeDef = TypedDict(
     "GetEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
     },
@@ -866,23 +854,14 @@
         "assessmentControlsCountByNoncompliantEvidence": int,
         "totalAssessmentControlsCount": int,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
-GetOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "GetOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
         "category": str,
@@ -1082,23 +1061,14 @@
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
 
-ListKeywordsForDataSourceResponseTypeDef = TypedDict(
-    "ListKeywordsForDataSourceResponseTypeDef",
-    {
-        "keywords": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListNotificationsRequestRequestTypeDef = TypedDict(
     "ListNotificationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1122,66 +1092,30 @@
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
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "kmsKey": str,
         "delegatedAdminAccount": str,
     },
     total=False,
 )
 
-RegisterAccountResponseTypeDef = TypedDict(
-    "RegisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
 )
 
-RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "frameworkId": str,
         "destinationAccount": str,
         "destinationRegion": str,
     },
@@ -1273,24 +1207,21 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
-ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
     {
-        "signatureValid": bool,
-        "signatureAlgorithm": str,
-        "signatureDateTime": str,
-        "signatureKeyId": str,
-        "validationErrors": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "awsAccounts": List[AWSAccountTypeDef],
+        "awsServices": List[AWSServiceTypeDef],
     },
+    total=False,
 )
 
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
@@ -1325,106 +1256,186 @@
         "evidenceSources": List[str],
         "evidenceCount": int,
         "assessmentReportEvidenceCount": int,
     },
     total=False,
 )
 
+BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssessmentReportResponseTypeDef = TypedDict(
+    "CreateAssessmentReportResponseTypeDef",
+    {
+        "assessmentReport": AssessmentReportTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterAccountResponseTypeDef = TypedDict(
+    "DeregisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountStatusResponseTypeDef = TypedDict(
+    "GetAccountStatusResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlResponseTypeDef",
+    {
+        "evidenceFileName": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceFolderResponseTypeDef",
     {
         "evidenceFolder": AssessmentEvidenceFolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentControlResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "GetOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    {
+        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentFrameworksResponseTypeDef = TypedDict(
     "ListAssessmentFrameworksResponseTypeDef",
     {
         "frameworkMetadataList": List[AssessmentFrameworkMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+ListAssessmentReportsResponseTypeDef = TypedDict(
+    "ListAssessmentReportsResponseTypeDef",
     {
-        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "assessmentReports": List[AssessmentReportMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "StartAssessmentFrameworkShareResponseTypeDef",
+ListKeywordsForDataSourceResponseTypeDef = TypedDict(
+    "ListKeywordsForDataSourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "keywords": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "UpdateAssessmentFrameworkShareResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+RegisterAccountResponseTypeDef = TypedDict(
+    "RegisterAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentReportsResponseTypeDef = TypedDict(
-    "ListAssessmentReportsResponseTypeDef",
+StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "StartAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReports": List[AssessmentReportMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssessmentReportResponseTypeDef = TypedDict(
-    "CreateAssessmentReportResponseTypeDef",
+UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "UpdateAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReport": AssessmentReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    {
+        "signatureValid": bool,
+        "signatureAlgorithm": str,
+        "signatureDateTime": str,
+        "signatureKeyId": str,
+        "validationErrors": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
         "createDelegationRequest": CreateDelegationRequestTypeDef,
@@ -1442,15 +1453,15 @@
     },
 )
 
 BatchDeleteDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     {
         "errors": List[BatchDeleteDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
         "manualEvidence": ManualEvidenceTypeDef,
@@ -1471,15 +1482,15 @@
 )
 
 GetChangeLogsResponseTypeDef = TypedDict(
     "GetChangeLogsResponseTypeDef",
     {
         "changeLogs": List[ChangeLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlDomainInsightsTypeDef = TypedDict(
     "ControlDomainInsightsTypeDef",
     {
         "name": str,
@@ -1545,15 +1556,15 @@
 )
 
 ListControlsResponseTypeDef = TypedDict(
     "ListControlsResponseTypeDef",
     {
         "controlMetadataList": List[ControlMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
@@ -1599,15 +1610,15 @@
 
 
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "snsTopic": str,
@@ -1658,61 +1669,61 @@
     total=False,
 )
 
 GetAssessmentReportUrlResponseTypeDef = TypedDict(
     "GetAssessmentReportUrlResponseTypeDef",
     {
         "preSignedUrl": URLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsByAssessmentResponseTypeDef = TypedDict(
     "GetInsightsByAssessmentResponseTypeDef",
     {
         "insights": InsightsByAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "insights": InsightsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServicesInScopeResponseTypeDef = TypedDict(
     "GetServicesInScopeResponseTypeDef",
     {
         "serviceMetadata": List[ServiceMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsResponseTypeDef = TypedDict(
     "ListNotificationsResponseTypeDef",
     {
         "notifications": List[NotificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentMetadataTypeDef = TypedDict(
     "AssessmentMetadataTypeDef",
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
         "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "scope": ScopeTypeDef,
+        "scope": ScopeOutputTypeDef,
         "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
@@ -1739,14 +1750,15 @@
 
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
 
+ScopeUnionTypeDef = Union[ScopeTypeDef, ScopeOutputTypeDef]
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
@@ -1769,15 +1781,15 @@
 
 
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
@@ -1792,68 +1804,68 @@
     total=False,
 )
 
 UpdateAssessmentControlResponseTypeDef = TypedDict(
     "UpdateAssessmentControlResponseTypeDef",
     {
         "control": AssessmentControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     {
         "delegations": List[DelegationTypeDef],
         "errors": List[BatchCreateDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlResponseTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     {
         "errors": List[BatchImportEvidenceToAssessmentControlErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsByAssessmentResponseTypeDef = TypedDict(
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsResponseTypeDef = TypedDict(
     "ListControlDomainInsightsResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListAssessmentControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsByAssessment": List[ControlInsightsMetadataByAssessmentItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsMetadata": List[ControlInsightsMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlTypeDef = TypedDict(
     "ControlTypeDef",
     {
         "arn": str,
@@ -1977,40 +1989,40 @@
     pass
 
 
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsResponseTypeDef = TypedDict(
     "UpdateSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceByEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceByEvidenceFolderResponseTypeDef",
     {
         "evidence": List[EvidenceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceResponseTypeDef = TypedDict(
     "GetEvidenceResponseTypeDef",
     {
         "evidence": EvidenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentFrameworkTypeDef = TypedDict(
     "AssessmentFrameworkTypeDef",
     {
         "id": str,
@@ -2021,15 +2033,15 @@
     total=False,
 )
 
 UpdateAssessmentControlSetStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusResponseTypeDef",
     {
         "controlSet": AssessmentControlSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlSetTypeDef = TypedDict(
     "ControlSetTypeDef",
     {
         "id": str,
@@ -2039,31 +2051,31 @@
     total=False,
 )
 
 CreateControlResponseTypeDef = TypedDict(
     "CreateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlResponseTypeDef = TypedDict(
     "GetControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateControlResponseTypeDef = TypedDict(
     "UpdateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
@@ -2096,59 +2108,59 @@
     total=False,
 )
 
 CreateAssessmentResponseTypeDef = TypedDict(
     "CreateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
         "userRole": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentStatusResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssessmentFrameworkResponseTypeDef = TypedDict(
     "CreateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentFrameworkResponseTypeDef = TypedDict(
     "GetAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentFrameworkResponseTypeDef = TypedDict(
     "UpdateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager/type_defs.pyi` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_auditmanager.type_defs import AWSAccountTypeDef
 
-    data: AWSAccountTypeDef = {...}
+    data: AWSAccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountStatusType,
     ActionEnumType,
     AssessmentReportStatusType,
     AssessmentStatusType,
     ControlResponseType,
@@ -62,14 +62,15 @@
     "FrameworkMetadataTypeDef",
     "AssessmentReportsDestinationTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
@@ -80,84 +81,84 @@
     "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
-    "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
-    "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
     "URLTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetChangeLogsRequestRequestTypeDef",
     "GetControlRequestRequestTypeDef",
     "GetDelegationsRequestRequestTypeDef",
     "GetEvidenceByEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
-    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     "GetEvidenceRequestRequestTypeDef",
     "GetInsightsByAssessmentRequestRequestTypeDef",
     "InsightsByAssessmentTypeDef",
     "InsightsTypeDef",
-    "GetOrganizationAdminAccountResponseTypeDef",
     "ServiceMetadataTypeDef",
     "GetSettingsRequestRequestTypeDef",
     "ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef",
     "ListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     "ListAssessmentFrameworksRequestRequestTypeDef",
     "ListAssessmentReportsRequestRequestTypeDef",
     "ListAssessmentsRequestRequestTypeDef",
     "ListControlDomainInsightsByAssessmentRequestRequestTypeDef",
     "ListControlDomainInsightsRequestRequestTypeDef",
     "ListControlInsightsByControlDomainRequestRequestTypeDef",
     "ListControlsRequestRequestTypeDef",
     "ListKeywordsForDataSourceRequestRequestTypeDef",
-    "ListKeywordsForDataSourceResponseTypeDef",
     "ListNotificationsRequestRequestTypeDef",
     "NotificationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegisterAccountRequestRequestTypeDef",
-    "RegisterAccountResponseTypeDef",
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAssessmentFrameworkShareRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    "CreateAssessmentReportResponseTypeDef",
+    "DeregisterAccountResponseTypeDef",
+    "GetAccountStatusResponseTypeDef",
+    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
-    "ListAssessmentFrameworksResponseTypeDef",
+    "GetOrganizationAdminAccountResponseTypeDef",
     "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    "ListAssessmentFrameworksResponseTypeDef",
+    "ListAssessmentReportsResponseTypeDef",
+    "ListKeywordsForDataSourceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterAccountResponseTypeDef",
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     "StartAssessmentFrameworkShareResponseTypeDef",
     "UpdateAssessmentFrameworkShareResponseTypeDef",
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    "ListAssessmentReportsResponseTypeDef",
-    "CreateAssessmentReportResponseTypeDef",
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     "BatchCreateDelegationByAssessmentRequestRequestTypeDef",
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
@@ -175,14 +176,15 @@
     "GetAssessmentReportUrlResponseTypeDef",
     "GetInsightsByAssessmentResponseTypeDef",
     "GetInsightsResponseTypeDef",
     "GetServicesInScopeResponseTypeDef",
     "ListNotificationsResponseTypeDef",
     "AssessmentMetadataTypeDef",
     "CreateAssessmentRequestRequestTypeDef",
+    "ScopeUnionTypeDef",
     "UpdateAssessmentRequestRequestTypeDef",
     "ListAssessmentsResponseTypeDef",
     "AssessmentControlSetTypeDef",
     "UpdateAssessmentControlResponseTypeDef",
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
@@ -408,14 +410,25 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
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
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
         "roleArn": str,
         "roleType": RoleTypeType,
@@ -589,22 +602,14 @@
 DeleteControlRequestRequestTypeDef = TypedDict(
     "DeleteControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
-DeregisterAccountResponseTypeDef = TypedDict(
-    "DeregisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
@@ -642,22 +647,14 @@
         "arn": str,
         "value": str,
         "complianceCheck": str,
     },
     total=False,
 )
 
-GetAccountStatusResponseTypeDef = TypedDict(
-    "GetAccountStatusResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "GetAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
     },
 )
 
@@ -749,23 +746,14 @@
 GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
     {
         "fileName": str,
     },
 )
 
-GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
-    "GetEvidenceFileUploadUrlResponseTypeDef",
-    {
-        "evidenceFileName": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEvidenceFolderRequestRequestTypeDef = TypedDict(
     "GetEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
     },
@@ -855,23 +843,14 @@
         "assessmentControlsCountByNoncompliantEvidence": int,
         "totalAssessmentControlsCount": int,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
-GetOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "GetOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
         "category": str,
@@ -1057,23 +1036,14 @@
 
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
-ListKeywordsForDataSourceResponseTypeDef = TypedDict(
-    "ListKeywordsForDataSourceResponseTypeDef",
-    {
-        "keywords": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListNotificationsRequestRequestTypeDef = TypedDict(
     "ListNotificationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1097,66 +1067,30 @@
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
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "kmsKey": str,
         "delegatedAdminAccount": str,
     },
     total=False,
 )
 
-RegisterAccountResponseTypeDef = TypedDict(
-    "RegisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
 )
 
-RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "frameworkId": str,
         "destinationAccount": str,
         "destinationRegion": str,
     },
@@ -1244,24 +1178,21 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
-ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
     {
-        "signatureValid": bool,
-        "signatureAlgorithm": str,
-        "signatureDateTime": str,
-        "signatureKeyId": str,
-        "validationErrors": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "awsAccounts": List[AWSAccountTypeDef],
+        "awsServices": List[AWSServiceTypeDef],
     },
+    total=False,
 )
 
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
@@ -1296,106 +1227,186 @@
         "evidenceSources": List[str],
         "evidenceCount": int,
         "assessmentReportEvidenceCount": int,
     },
     total=False,
 )
 
+BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssessmentReportResponseTypeDef = TypedDict(
+    "CreateAssessmentReportResponseTypeDef",
+    {
+        "assessmentReport": AssessmentReportTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterAccountResponseTypeDef = TypedDict(
+    "DeregisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountStatusResponseTypeDef = TypedDict(
+    "GetAccountStatusResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlResponseTypeDef",
+    {
+        "evidenceFileName": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceFolderResponseTypeDef",
     {
         "evidenceFolder": AssessmentEvidenceFolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentControlResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "GetOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    {
+        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentFrameworksResponseTypeDef = TypedDict(
     "ListAssessmentFrameworksResponseTypeDef",
     {
         "frameworkMetadataList": List[AssessmentFrameworkMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+ListAssessmentReportsResponseTypeDef = TypedDict(
+    "ListAssessmentReportsResponseTypeDef",
     {
-        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "assessmentReports": List[AssessmentReportMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "StartAssessmentFrameworkShareResponseTypeDef",
+ListKeywordsForDataSourceResponseTypeDef = TypedDict(
+    "ListKeywordsForDataSourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "keywords": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "UpdateAssessmentFrameworkShareResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+RegisterAccountResponseTypeDef = TypedDict(
+    "RegisterAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentReportsResponseTypeDef = TypedDict(
-    "ListAssessmentReportsResponseTypeDef",
+StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "StartAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReports": List[AssessmentReportMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssessmentReportResponseTypeDef = TypedDict(
-    "CreateAssessmentReportResponseTypeDef",
+UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "UpdateAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReport": AssessmentReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    {
+        "signatureValid": bool,
+        "signatureAlgorithm": str,
+        "signatureDateTime": str,
+        "signatureKeyId": str,
+        "validationErrors": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
         "createDelegationRequest": CreateDelegationRequestTypeDef,
@@ -1413,15 +1424,15 @@
     },
 )
 
 BatchDeleteDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     {
         "errors": List[BatchDeleteDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
         "manualEvidence": ManualEvidenceTypeDef,
@@ -1442,15 +1453,15 @@
 )
 
 GetChangeLogsResponseTypeDef = TypedDict(
     "GetChangeLogsResponseTypeDef",
     {
         "changeLogs": List[ChangeLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlDomainInsightsTypeDef = TypedDict(
     "ControlDomainInsightsTypeDef",
     {
         "name": str,
@@ -1516,15 +1527,15 @@
 )
 
 ListControlsResponseTypeDef = TypedDict(
     "ListControlsResponseTypeDef",
     {
         "controlMetadataList": List[ControlMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
@@ -1566,15 +1577,15 @@
     pass
 
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "snsTopic": str,
@@ -1625,61 +1636,61 @@
     total=False,
 )
 
 GetAssessmentReportUrlResponseTypeDef = TypedDict(
     "GetAssessmentReportUrlResponseTypeDef",
     {
         "preSignedUrl": URLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsByAssessmentResponseTypeDef = TypedDict(
     "GetInsightsByAssessmentResponseTypeDef",
     {
         "insights": InsightsByAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "insights": InsightsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServicesInScopeResponseTypeDef = TypedDict(
     "GetServicesInScopeResponseTypeDef",
     {
         "serviceMetadata": List[ServiceMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsResponseTypeDef = TypedDict(
     "ListNotificationsResponseTypeDef",
     {
         "notifications": List[NotificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentMetadataTypeDef = TypedDict(
     "AssessmentMetadataTypeDef",
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
         "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "scope": ScopeTypeDef,
+        "scope": ScopeOutputTypeDef,
         "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
@@ -1704,14 +1715,15 @@
 )
 
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
+ScopeUnionTypeDef = Union[ScopeTypeDef, ScopeOutputTypeDef]
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
@@ -1732,15 +1744,15 @@
     pass
 
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
@@ -1755,68 +1767,68 @@
     total=False,
 )
 
 UpdateAssessmentControlResponseTypeDef = TypedDict(
     "UpdateAssessmentControlResponseTypeDef",
     {
         "control": AssessmentControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     {
         "delegations": List[DelegationTypeDef],
         "errors": List[BatchCreateDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlResponseTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     {
         "errors": List[BatchImportEvidenceToAssessmentControlErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsByAssessmentResponseTypeDef = TypedDict(
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsResponseTypeDef = TypedDict(
     "ListControlDomainInsightsResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListAssessmentControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsByAssessment": List[ControlInsightsMetadataByAssessmentItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsMetadata": List[ControlInsightsMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlTypeDef = TypedDict(
     "ControlTypeDef",
     {
         "arn": str,
@@ -1932,40 +1944,40 @@
 ):
     pass
 
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsResponseTypeDef = TypedDict(
     "UpdateSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceByEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceByEvidenceFolderResponseTypeDef",
     {
         "evidence": List[EvidenceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceResponseTypeDef = TypedDict(
     "GetEvidenceResponseTypeDef",
     {
         "evidence": EvidenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentFrameworkTypeDef = TypedDict(
     "AssessmentFrameworkTypeDef",
     {
         "id": str,
@@ -1976,15 +1988,15 @@
     total=False,
 )
 
 UpdateAssessmentControlSetStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusResponseTypeDef",
     {
         "controlSet": AssessmentControlSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlSetTypeDef = TypedDict(
     "ControlSetTypeDef",
     {
         "id": str,
@@ -1994,31 +2006,31 @@
     total=False,
 )
 
 CreateControlResponseTypeDef = TypedDict(
     "CreateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlResponseTypeDef = TypedDict(
     "GetControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateControlResponseTypeDef = TypedDict(
     "UpdateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
@@ -2051,59 +2063,59 @@
     total=False,
 )
 
 CreateAssessmentResponseTypeDef = TypedDict(
     "CreateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
         "userRole": RoleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentStatusResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssessmentFrameworkResponseTypeDef = TypedDict(
     "CreateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentFrameworkResponseTypeDef = TypedDict(
     "GetAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentFrameworkResponseTypeDef = TypedDict(
     "UpdateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/PKG-INFO` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-auditmanager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AuditManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AuditManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore auditmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore auditmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-auditmanager"></a>
 
 # types-aiobotocore-auditmanager
 
 [![PyPI - types-aiobotocore-auditmanager](https://img.shields.io/pypi/v/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-auditmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-auditmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-auditmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-auditmanager)](https://pepy.tech/project/types-aiobotocore-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AuditManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [types-aiobotocore-auditmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/).
 
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
@@ -305,20 +304,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_auditmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_auditmanager.type_defs import (
     AWSAccountTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
     RoleTypeDef,
@@ -329,14 +328,15 @@
     FrameworkMetadataTypeDef,
     AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
@@ -347,84 +347,84 @@
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
-    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFileUploadUrlRequestRequestTypeDef,
-    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
-    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
+    DeregisterAccountResponseTypeDef,
+    GetAccountStatusResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    ListAssessmentFrameworksResponseTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ListAssessmentFrameworkShareRequestsResponseTypeDef,
+    ListAssessmentFrameworksResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterAccountResponseTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
@@ -442,14 +442,15 @@
     GetAssessmentReportUrlResponseTypeDef,
     GetInsightsByAssessmentResponseTypeDef,
     GetInsightsResponseTypeDef,
     GetServicesInScopeResponseTypeDef,
     ListNotificationsResponseTypeDef,
     AssessmentMetadataTypeDef,
     CreateAssessmentRequestRequestTypeDef,
+    ScopeUnionTypeDef,
     UpdateAssessmentRequestRequestTypeDef,
     ListAssessmentsResponseTypeDef,
     AssessmentControlSetTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     BatchCreateDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlResponseTypeDef,
     ListControlDomainInsightsByAssessmentResponseTypeDef,
@@ -479,15 +480,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_value() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-auditmanager-2.5.2/types_aiobotocore_auditmanager.egg-info/SOURCES.txt` & `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


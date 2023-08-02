# Comparing `tmp/types-aiobotocore-ssm-contacts-2.5.2.tar.gz` & `tmp/types-aiobotocore-ssm-contacts-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ssm-contacts-2.5.2.tar", last modified: Sat Jul  8 01:44:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-ssm-contacts-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:03 2023, max compression
```

## Comparing `types-aiobotocore-ssm-contacts-2.5.2.tar` & `types-aiobotocore-ssm-contacts-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.042934 types-aiobotocore-ssm-contacts-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-08 01:44:22.042934 types-aiobotocore-ssm-contacts-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:22.042934 types-aiobotocore-ssm-contacts-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.042934 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34382 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34323 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39525 2023-07-08 01:41:33.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39450 2023-07-08 01:41:32.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:31.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.042934 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-07-08 01:44:21.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:44:21.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:21.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:21.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:21.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:44:21.000000 types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.949449 types-aiobotocore-ssm-contacts-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-08-02 14:53:03.945449 types-aiobotocore-ssm-contacts-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:03.949449 types-aiobotocore-ssm-contacts-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.945449 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34358 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34299 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40767 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-08-02 14:50:10.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:09.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.945449 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:53:03.000000 types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/LICENSE` & `types-aiobotocore-ssm-contacts-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/PKG-INFO` & `types-aiobotocore-ssm-contacts-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-contacts
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ssm-contacts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ssm-contacts type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ssm-contacts"></a>
 
 # types-aiobotocore-ssm-contacts
 
 [![PyPI - types-aiobotocore-ssm-contacts](https://img.shields.io/pypi/v/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-contacts?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-contacts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSMContacts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [types-aiobotocore-ssm-contacts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/).
 
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
@@ -360,127 +359,133 @@
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ssm_contacts.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
-    CreateContactChannelResultTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateContactResultTypeDef,
-    CreateRotationOverrideRequestRequestTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
+    TimestampTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
-    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
-    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
-    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
-    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
-    PreviewOverrideTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    ListRotationShiftsRequestRequestTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutContactPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
-    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
-    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
     TargetTypeDef,
-    ListContactsResultTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
+    CreateContactChannelResultTypeDef,
+    CreateContactResultTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
+    DescribeEngagementResultTypeDef,
+    DescribePageResultTypeDef,
+    GetContactChannelResultTypeDef,
+    GetContactPolicyResultTypeDef,
+    GetRotationOverrideResultTypeDef,
+    ListContactsResultTypeDef,
+    StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateRotationOverrideRequestRequestTypeDef,
+    ListRotationOverridesRequestRequestTypeDef,
+    ListRotationShiftsRequestRequestTypeDef,
+    PreviewOverrideTypeDef,
+    TimeRangeTypeDef,
     ListEngagementsResultTypeDef,
-    ListEngagementsRequestListEngagementsPaginateTypeDef,
-    ListEngagementsRequestRequestTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
+    StageOutputTypeDef,
     StageTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
+    ListEngagementsRequestListEngagementsPaginateTypeDef,
+    ListEngagementsRequestRequestTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
-    CreateRotationRequestRequestTypeDef,
     GetRotationResultTypeDef,
+    RotationTypeDef,
+    CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
-    RotationTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     UpdateRotationRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResultTypeDef,
+    CreateContactRequestRequestTypeDef,
+    PlanUnionTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
-def get_structure() -> AcceptPageRequestRequestTypeDef:
+def get_value() -> AcceptPageRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/README.md` & `types-aiobotocore-ssm-contacts-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ssm-contacts"></a>
 
 # types-aiobotocore-ssm-contacts
 
 [![PyPI - types-aiobotocore-ssm-contacts](https://img.shields.io/pypi/v/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-contacts?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-contacts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSMContacts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [types-aiobotocore-ssm-contacts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/).
 
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
@@ -327,127 +327,133 @@
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ssm_contacts.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
-    CreateContactChannelResultTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateContactResultTypeDef,
-    CreateRotationOverrideRequestRequestTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
+    TimestampTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
-    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
-    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
-    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
-    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
-    PreviewOverrideTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    ListRotationShiftsRequestRequestTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutContactPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
-    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
-    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
     TargetTypeDef,
-    ListContactsResultTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
+    CreateContactChannelResultTypeDef,
+    CreateContactResultTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
+    DescribeEngagementResultTypeDef,
+    DescribePageResultTypeDef,
+    GetContactChannelResultTypeDef,
+    GetContactPolicyResultTypeDef,
+    GetRotationOverrideResultTypeDef,
+    ListContactsResultTypeDef,
+    StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateRotationOverrideRequestRequestTypeDef,
+    ListRotationOverridesRequestRequestTypeDef,
+    ListRotationShiftsRequestRequestTypeDef,
+    PreviewOverrideTypeDef,
+    TimeRangeTypeDef,
     ListEngagementsResultTypeDef,
-    ListEngagementsRequestListEngagementsPaginateTypeDef,
-    ListEngagementsRequestRequestTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
+    StageOutputTypeDef,
     StageTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
+    ListEngagementsRequestListEngagementsPaginateTypeDef,
+    ListEngagementsRequestRequestTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
-    CreateRotationRequestRequestTypeDef,
     GetRotationResultTypeDef,
+    RotationTypeDef,
+    CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
-    RotationTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     UpdateRotationRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResultTypeDef,
+    CreateContactRequestRequestTypeDef,
+    PlanUnionTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
-def get_structure() -> AcceptPageRequestRequestTypeDef:
+def get_value() -> AcceptPageRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/setup.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ssm-contacts",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with"
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
-    keywords="aiobotocore ssm-contacts type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ssm-contacts type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ssm_contacts": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/"
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/__init__.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/__init__.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/__main__.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSMContacts 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SSMContacts 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/client.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("ssm-contacts") as client:
         client: SSMContactsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import AcceptCodeValidationType, AcceptTypeType, ChannelTypeType, ContactTypeType
 from .paginator import (
     ListContactChannelsPaginator,
@@ -56,20 +55,21 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    PlanTypeDef,
+    PlanUnionTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -158,15 +158,15 @@
         """
 
     async def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: PlanTypeDef,
+        Plan: PlanUnionTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
@@ -196,16 +196,16 @@
 
     async def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation)
@@ -213,16 +213,16 @@
         """
 
     async def create_rotation_override(
         self,
         *,
         RotationId: str,
         NewContactIds: Sequence[str],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         IdempotencyToken: str = ...
     ) -> CreateRotationOverrideResultTypeDef:
         """
         Creates an override for a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation_override)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation_override)
@@ -425,20 +425,20 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_pages_by_engagement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_pages_by_engagement)
         """
 
     async def list_preview_rotation_shifts(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
         Returns a list of shifts based on rotation configuration parameters.
 
@@ -446,32 +446,32 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_preview_rotation_shifts)
         """
 
     async def list_rotation_overrides(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationOverridesResultTypeDef:
         """
         Retrieves a list of overrides currently specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_overrides)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_rotation_overrides)
         """
 
     async def list_rotation_shifts(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationShiftsResultTypeDef:
         """
         Returns a list of shifts generated by an existing rotation in the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_shifts)
@@ -553,15 +553,15 @@
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#untag_resource)
         """
 
     async def update_contact(
-        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanTypeDef = ...
+        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact)
         """
@@ -580,17 +580,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact_channel)
         """
 
     async def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
         ContactIds: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_rotation)
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/client.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("ssm-contacts") as client:
         client: SSMContactsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import AcceptCodeValidationType, AcceptTypeType, ChannelTypeType, ContactTypeType
 from .paginator import (
     ListContactChannelsPaginator,
@@ -56,20 +55,21 @@
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     ListTagsForResourceResultTypeDef,
-    PlanTypeDef,
+    PlanUnionTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     StartEngagementResultTypeDef,
     TagTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -149,15 +149,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#close)
         """
     async def create_contact(
         self,
         *,
         Alias: str,
         Type: ContactTypeType,
-        Plan: PlanTypeDef,
+        Plan: PlanUnionTypeDef,
         DisplayName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateContactResultTypeDef:
         """
         Contacts are either the contacts that Incident Manager engages during an
         incident or the escalation plans that Incident Manager uses to engage contacts
@@ -185,32 +185,32 @@
         """
     async def create_rotation(
         self,
         *,
         Name: str,
         ContactIds: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        StartTime: TimestampTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> CreateRotationResultTypeDef:
         """
         Creates a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation)
         """
     async def create_rotation_override(
         self,
         *,
         RotationId: str,
         NewContactIds: Sequence[str],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         IdempotencyToken: str = ...
     ) -> CreateRotationOverrideResultTypeDef:
         """
         Creates an override for a rotation in an on-call schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.create_rotation_override)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#create_rotation_override)
@@ -392,51 +392,51 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_pages_by_engagement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_pages_by_engagement)
         """
     async def list_preview_rotation_shifts(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListPreviewRotationShiftsResultTypeDef:
         """
         Returns a list of shifts based on rotation configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_preview_rotation_shifts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_preview_rotation_shifts)
         """
     async def list_rotation_overrides(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationOverridesResultTypeDef:
         """
         Retrieves a list of overrides currently specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_overrides)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#list_rotation_overrides)
         """
     async def list_rotation_shifts(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListRotationShiftsResultTypeDef:
         """
         Returns a list of shifts generated by an existing rotation in the system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.list_rotation_shifts)
@@ -509,15 +509,15 @@
         """
         Removes tags from the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#untag_resource)
         """
     async def update_contact(
-        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanTypeDef = ...
+        self, *, ContactId: str, DisplayName: str = ..., Plan: PlanUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the contact or escalation plan specified.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact)
         """
@@ -534,17 +534,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_contact_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_contact_channel)
         """
     async def update_rotation(
         self,
         *,
         RotationId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
         ContactIds: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
         TimeZoneId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the information specified for an on-call rotation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client.update_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/client/#update_rotation)
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/literals.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/literals.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/paginator.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         list_pages_by_engagement_paginator: ListPagesByEngagementPaginator = client.get_paginator("list_pages_by_engagement")
         list_preview_rotation_shifts_paginator: ListPreviewRotationShiftsPaginator = client.get_paginator("list_preview_rotation_shifts")
         list_rotation_overrides_paginator: ListRotationOverridesPaginator = client.get_paginator("list_rotation_overrides")
         list_rotation_shifts_paginator: ListRotationShiftsPaginator = client.get_paginator("list_rotation_shifts")
         list_rotations_paginator: ListRotationsPaginator = client.get_paginator("list_rotations")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ContactTypeType
 from .type_defs import (
     ListContactChannelsResultTypeDef,
@@ -57,16 +56,17 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
     "ListEngagementsPaginator",
     "ListPageReceiptsPaginator",
@@ -75,208 +75,195 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
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
 class ListContactChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactchannelspaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContactChannelsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactchannelspaginator)
         """
 
-
 class ListContactsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactspaginator)
         """
 
-
 class ListEngagementsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listengagementspaginator)
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listengagementspaginator)
         """
 
-
 class ListPageReceiptsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagereceiptspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPageReceiptsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagereceiptspaginator)
         """
 
-
 class ListPageResolutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpageresolutionspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPageResolutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpageresolutionspaginator)
         """
 
-
 class ListPagesByContactPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbycontactpaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPagesByContactResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbycontactpaginator)
         """
 
-
 class ListPagesByEngagementPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbyengagementpaginator)
     """
 
     def paginate(
-        self, *, EngagementId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EngagementId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPagesByEngagementResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbyengagementpaginator)
         """
 
-
 class ListPreviewRotationShiftsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
-
 class ListRotationOverridesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
-
 class ListRotationShiftsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
-
 class ListRotationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationspaginator)
     """
 
     def paginate(
-        self, *, RotationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RotationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRotationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/paginator.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         list_pages_by_engagement_paginator: ListPagesByEngagementPaginator = client.get_paginator("list_pages_by_engagement")
         list_preview_rotation_shifts_paginator: ListPreviewRotationShiftsPaginator = client.get_paginator("list_preview_rotation_shifts")
         list_rotation_overrides_paginator: ListRotationOverridesPaginator = client.get_paginator("list_rotation_overrides")
         list_rotation_shifts_paginator: ListRotationShiftsPaginator = client.get_paginator("list_rotation_shifts")
         list_rotations_paginator: ListRotationsPaginator = client.get_paginator("list_rotations")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ContactTypeType
 from .type_defs import (
     ListContactChannelsResultTypeDef,
@@ -57,16 +56,17 @@
     ListPagesByEngagementResultTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationOverridesResultTypeDef,
     ListRotationShiftsResultTypeDef,
     ListRotationsResultTypeDef,
     PaginatorConfigTypeDef,
     PreviewOverrideTypeDef,
-    RecurrenceSettingsTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     TimeRangeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListContactChannelsPaginator",
     "ListContactsPaginator",
     "ListEngagementsPaginator",
     "ListPageReceiptsPaginator",
@@ -75,195 +75,208 @@
     "ListPagesByEngagementPaginator",
     "ListPreviewRotationShiftsPaginator",
     "ListRotationOverridesPaginator",
     "ListRotationShiftsPaginator",
     "ListRotationsPaginator",
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
 class ListContactChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactchannelspaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContactChannelsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContactChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactchannelspaginator)
         """
 
+
 class ListContactsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactspaginator)
     """
 
     def paginate(
         self,
         *,
         AliasPrefix: str = ...,
         Type: ContactTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListContactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListContacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listcontactspaginator)
         """
 
+
 class ListEngagementsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listengagementspaginator)
     """
 
     def paginate(
         self,
         *,
         IncidentId: str = ...,
         TimeRangeValue: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEngagementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListEngagements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listengagementspaginator)
         """
 
+
 class ListPageReceiptsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagereceiptspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPageReceiptsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageReceipts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagereceiptspaginator)
         """
 
+
 class ListPageResolutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpageresolutionspaginator)
     """
 
     def paginate(
-        self, *, PageId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PageId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPageResolutionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPageResolutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpageresolutionspaginator)
         """
 
+
 class ListPagesByContactPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbycontactpaginator)
     """
 
     def paginate(
-        self, *, ContactId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ContactId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPagesByContactResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByContact.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbycontactpaginator)
         """
 
+
 class ListPagesByEngagementPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbyengagementpaginator)
     """
 
     def paginate(
-        self, *, EngagementId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EngagementId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPagesByEngagementResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPagesByEngagement.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpagesbyengagementpaginator)
         """
 
+
 class ListPreviewRotationShiftsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
-        EndTime: Union[datetime, str],
+        EndTime: TimestampTypeDef,
         Members: Sequence[str],
         TimeZoneId: str,
-        Recurrence: RecurrenceSettingsTypeDef,
-        RotationStartTime: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
+        Recurrence: RecurrenceSettingsUnionTypeDef,
+        RotationStartTime: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
         Overrides: Sequence[PreviewOverrideTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPreviewRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListPreviewRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listpreviewrotationshiftspaginator)
         """
 
+
 class ListRotationOverridesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationoverridespaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRotationOverridesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationOverrides.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationoverridespaginator)
         """
 
+
 class ListRotationShiftsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationshiftspaginator)
     """
 
     def paginate(
         self,
         *,
         RotationId: str,
-        EndTime: Union[datetime, str],
-        StartTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        EndTime: TimestampTypeDef,
+        StartTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRotationShiftsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotationShifts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationshiftspaginator)
         """
 
+
 class ListRotationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationspaginator)
     """
 
     def paginate(
-        self, *, RotationNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RotationNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRotationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Paginator.ListRotations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/paginators/#listrotationspaginator)
         """
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/type_defs.py` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ssm_contacts.type_defs import AcceptPageRequestRequestTypeDef
 
-    data: AcceptPageRequestRequestTypeDef = {...}
+    data: AcceptPageRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -36,105 +36,111 @@
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
     "HandOffTimeTypeDef",
-    "CreateContactChannelResultTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateContactResultTypeDef",
-    "CreateRotationOverrideRequestRequestTypeDef",
-    "CreateRotationOverrideResultTypeDef",
-    "CreateRotationResultTypeDef",
+    "TimestampTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
-    "DescribeEngagementResultTypeDef",
     "DescribePageRequestRequestTypeDef",
-    "DescribePageResultTypeDef",
     "EngagementTypeDef",
     "GetContactChannelRequestRequestTypeDef",
     "GetContactPolicyRequestRequestTypeDef",
-    "GetContactPolicyResultTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
-    "GetRotationOverrideResultTypeDef",
     "GetRotationRequestRequestTypeDef",
-    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
-    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
-    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
-    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
-    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
-    "PreviewOverrideTypeDef",
-    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
-    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    "ListRotationShiftsRequestRequestTypeDef",
-    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
-    "StartEngagementResultTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
-    "GetContactChannelResultTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
     "TargetTypeDef",
-    "ListContactsResultTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
+    "CreateContactChannelResultTypeDef",
+    "CreateContactResultTypeDef",
+    "CreateRotationOverrideResultTypeDef",
+    "CreateRotationResultTypeDef",
+    "DescribeEngagementResultTypeDef",
+    "DescribePageResultTypeDef",
+    "GetContactChannelResultTypeDef",
+    "GetContactPolicyResultTypeDef",
+    "GetRotationOverrideResultTypeDef",
+    "ListContactsResultTypeDef",
+    "StartEngagementResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateRotationOverrideRequestRequestTypeDef",
+    "ListRotationOverridesRequestRequestTypeDef",
+    "ListRotationShiftsRequestRequestTypeDef",
+    "PreviewOverrideTypeDef",
+    "TimeRangeTypeDef",
     "ListEngagementsResultTypeDef",
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
-    "ListEngagementsRequestRequestTypeDef",
+    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
+    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
+    "StageOutputTypeDef",
     "StageTypeDef",
+    "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    "ListEngagementsRequestRequestTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
+    "PlanOutputTypeDef",
     "PlanTypeDef",
-    "CreateRotationRequestRequestTypeDef",
     "GetRotationResultTypeDef",
+    "RotationTypeDef",
+    "CreateRotationRequestRequestTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
-    "RotationTypeDef",
+    "RecurrenceSettingsUnionTypeDef",
     "UpdateRotationRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "GetContactResultTypeDef",
+    "CreateContactRequestRequestTypeDef",
+    "PlanUnionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -243,80 +249,35 @@
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
 
-CreateContactChannelResultTypeDef = TypedDict(
-    "CreateContactChannelResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ContactChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateContactResultTypeDef = TypedDict(
-    "CreateContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "NewContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-
-class CreateRotationOverrideRequestRequestTypeDef(
-    _RequiredCreateRotationOverrideRequestRequestTypeDef,
-    _OptionalCreateRotationOverrideRequestRequestTypeDef,
-):
-    pass
-
-
-CreateRotationOverrideResultTypeDef = TypedDict(
-    "CreateRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRotationResultTypeDef = TypedDict(
-    "CreateRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -352,57 +313,21 @@
 DescribeEngagementRequestRequestTypeDef = TypedDict(
     "DescribeEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 
-DescribeEngagementResultTypeDef = TypedDict(
-    "DescribeEngagementResultTypeDef",
-    {
-        "ContactArn": str,
-        "EngagementArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "StartTime": datetime,
-        "StopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePageRequestRequestTypeDef = TypedDict(
     "DescribePageRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 
-DescribePageResultTypeDef = TypedDict(
-    "DescribePageResultTypeDef",
-    {
-        "PageArn": str,
-        "EngagementArn": str,
-        "ContactArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "SentTime": datetime,
-        "ReadTime": datetime,
-        "DeliveryTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngagementTypeDef = TypedDict(
     "_RequiredEngagementTypeDef",
     {
         "EngagementArn": str,
         "ContactArn": str,
         "Sender": str,
     },
@@ -432,23 +357,14 @@
 GetContactPolicyRequestRequestTypeDef = TypedDict(
     "GetContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
     },
 )
 
-GetContactPolicyResultTypeDef = TypedDict(
-    "GetContactPolicyResultTypeDef",
-    {
-        "ContactArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 
@@ -456,56 +372,31 @@
     "GetRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "RotationOverrideId": str,
     },
 )
 
-GetRotationOverrideResultTypeDef = TypedDict(
-    "GetRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "RotationArn": str,
-        "NewContactIds": List[str],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRotationRequestRequestTypeDef = TypedDict(
     "GetRotationRequestRequestTypeDef",
     {
         "RotationId": str,
     },
 )
 
-_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
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
-class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
-    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListContactChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactChannelsRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListContactChannelsRequestRequestTypeDef = TypedDict(
@@ -521,66 +412,25 @@
 class ListContactChannelsRequestRequestTypeDef(
     _RequiredListContactChannelsRequestRequestTypeDef,
     _OptionalListContactChannelsRequestRequestTypeDef,
 ):
     pass
 
 
-ListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "ListContactsRequestListContactsPaginateTypeDef",
-    {
-        "AliasPrefix": str,
-        "Type": ContactTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContactsRequestRequestTypeDef = TypedDict(
     "ListContactsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
-    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -616,36 +466,14 @@
 )
 
 
 class ReceiptTypeDef(_RequiredReceiptTypeDef, _OptionalReceiptTypeDef):
     pass
 
 
-_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
-    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPageResolutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageResolutionsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageResolutionsRequestRequestTypeDef = TypedDict(
@@ -682,36 +510,14 @@
 
 class ResolutionContactTypeDef(
     _RequiredResolutionContactTypeDef, _OptionalResolutionContactTypeDef
 ):
     pass
 
 
-_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
-    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPagesByContactRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListPagesByContactRequestRequestTypeDef = TypedDict(
@@ -752,36 +558,14 @@
 )
 
 
 class PageTypeDef(_RequiredPageTypeDef, _OptionalPageTypeDef):
     pass
 
 
-_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "EngagementId": str,
-    },
-)
-_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
-    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPagesByEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalListPagesByEngagementRequestRequestTypeDef = TypedDict(
@@ -797,142 +581,25 @@
 class ListPagesByEngagementRequestRequestTypeDef(
     _RequiredListPagesByEngagementRequestRequestTypeDef,
     _OptionalListPagesByEngagementRequestRequestTypeDef,
 ):
     pass
 
 
-PreviewOverrideTypeDef = TypedDict(
-    "PreviewOverrideTypeDef",
-    {
-        "NewMembers": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
-    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListRotationOverridesRequestRequestTypeDef(
-    _RequiredListRotationOverridesRequestRequestTypeDef,
-    _OptionalListRotationOverridesRequestRequestTypeDef,
-):
-    pass
-
-
 RotationOverrideTypeDef = TypedDict(
     "RotationOverrideTypeDef",
     {
         "RotationOverrideId": str,
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
-_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
-    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListRotationShiftsRequestRequestTypeDef(
-    _RequiredListRotationShiftsRequestRequestTypeDef,
-    _OptionalListRotationShiftsRequestRequestTypeDef,
-):
-    pass
-
-
-ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
-    "ListRotationsRequestListRotationsPaginateTypeDef",
-    {
-        "RotationNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -942,43 +609,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
         "Policy": str,
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
 ShiftDetailsTypeDef = TypedDict(
     "ShiftDetailsTypeDef",
     {
         "OverriddenContactIds": List[str],
     },
 )
 
@@ -1012,22 +658,14 @@
 
 class StartEngagementRequestRequestTypeDef(
     _RequiredStartEngagementRequestRequestTypeDef, _OptionalStartEngagementRequestRequestTypeDef
 ):
     pass
 
 
-StartEngagementResultTypeDef = TypedDict(
-    "StartEngagementResultTypeDef",
-    {
-        "EngagementArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredStopEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalStopEngagementRequestRequestTypeDef = TypedDict(
@@ -1098,27 +736,14 @@
 class CreateContactChannelRequestRequestTypeDef(
     _RequiredCreateContactChannelRequestRequestTypeDef,
     _OptionalCreateContactChannelRequestRequestTypeDef,
 ):
     pass
 
 
-GetContactChannelResultTypeDef = TypedDict(
-    "GetContactChannelResultTypeDef",
-    {
-        "ContactArn": str,
-        "ContactChannelArn": str,
-        "Name": str,
-        "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
-        "ActivationStatus": ActivationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalUpdateContactChannelRequestRequestTypeDef = TypedDict(
@@ -1143,23 +768,14 @@
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
-ListContactsResultTypeDef = TypedDict(
-    "ListContactsResultTypeDef",
-    {
-        "NextToken": str,
-        "Contacts": List[ContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
         "End": HandOffTimeTypeDef,
     },
     total=False,
@@ -1177,102 +793,472 @@
     "WeeklySettingTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "HandOffTime": HandOffTimeTypeDef,
     },
 )
 
+CreateContactChannelResultTypeDef = TypedDict(
+    "CreateContactChannelResultTypeDef",
+    {
+        "ContactChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContactResultTypeDef = TypedDict(
+    "CreateContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationOverrideResultTypeDef = TypedDict(
+    "CreateRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationResultTypeDef = TypedDict(
+    "CreateRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEngagementResultTypeDef = TypedDict(
+    "DescribeEngagementResultTypeDef",
+    {
+        "ContactArn": str,
+        "EngagementArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "StartTime": datetime,
+        "StopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePageResultTypeDef = TypedDict(
+    "DescribePageResultTypeDef",
+    {
+        "PageArn": str,
+        "EngagementArn": str,
+        "ContactArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "SentTime": datetime,
+        "ReadTime": datetime,
+        "DeliveryTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactChannelResultTypeDef = TypedDict(
+    "GetContactChannelResultTypeDef",
+    {
+        "ContactArn": str,
+        "ContactChannelArn": str,
+        "Name": str,
+        "Type": ChannelTypeType,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
+        "ActivationStatus": ActivationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactPolicyResultTypeDef = TypedDict(
+    "GetContactPolicyResultTypeDef",
+    {
+        "ContactArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRotationOverrideResultTypeDef = TypedDict(
+    "GetRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "RotationArn": str,
+        "NewContactIds": List[str],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContactsResultTypeDef = TypedDict(
+    "ListContactsResultTypeDef",
+    {
+        "NextToken": str,
+        "Contacts": List[ContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartEngagementResultTypeDef = TypedDict(
+    "StartEngagementResultTypeDef",
+    {
+        "EngagementArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "NewContactIds": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+
+class CreateRotationOverrideRequestRequestTypeDef(
+    _RequiredCreateRotationOverrideRequestRequestTypeDef,
+    _OptionalCreateRotationOverrideRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListRotationOverridesRequestRequestTypeDef(
+    _RequiredListRotationOverridesRequestRequestTypeDef,
+    _OptionalListRotationOverridesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListRotationShiftsRequestRequestTypeDef(
+    _RequiredListRotationShiftsRequestRequestTypeDef,
+    _OptionalListRotationShiftsRequestRequestTypeDef,
+):
+    pass
+
+
+PreviewOverrideTypeDef = TypedDict(
+    "PreviewOverrideTypeDef",
+    {
+        "NewMembers": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
     {
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ContactId": str,
+    },
+)
+_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListEngagementsRequestRequestTypeDef = TypedDict(
-    "ListEngagementsRequestRequestTypeDef",
+
+class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
+    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
+):
+    pass
+
+
+ListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "ListContactsRequestListContactsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
+        "AliasPrefix": str,
+        "Type": ContactTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
+    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
+    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
+    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "EngagementId": str,
+    },
+)
+_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
+    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
+    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
+    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+):
+    pass
+
+
+ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
+    "ListRotationsRequestListRotationsPaginateTypeDef",
+    {
+        "RotationNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPageResolutionsResultTypeDef = TypedDict(
     "ListPageResolutionsResultTypeDef",
     {
         "NextToken": str,
         "PageResolutions": List[ResolutionContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByContactResultTypeDef = TypedDict(
     "ListPagesByContactResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByEngagementResultTypeDef = TypedDict(
     "ListPagesByEngagementResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationOverridesResultTypeDef = TypedDict(
     "ListRotationOverridesResultTypeDef",
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
@@ -1295,26 +1281,59 @@
 
 
 ListContactChannelsResultTypeDef = TypedDict(
     "ListContactChannelsResultTypeDef",
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StageOutputTypeDef = TypedDict(
+    "StageOutputTypeDef",
+    {
+        "DurationInMinutes": int,
+        "Targets": List[TargetTypeDef],
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
         "Targets": Sequence[TargetTypeDef],
     },
 )
 
+_RequiredRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_RequiredRecurrenceSettingsOutputTypeDef",
+    {
+        "NumberOfOnCalls": int,
+        "RecurrenceMultiplier": int,
+    },
+)
+_OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_OptionalRecurrenceSettingsOutputTypeDef",
+    {
+        "MonthlySettings": List[MonthlySettingTypeDef],
+        "WeeklySettings": List[WeeklySettingTypeDef],
+        "DailySettings": List[HandOffTimeTypeDef],
+        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeTypeDef]],
+    },
+    total=False,
+)
+
+
+class RecurrenceSettingsOutputTypeDef(
+    _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
+):
+    pass
+
+
 _RequiredRecurrenceSettingsTypeDef = TypedDict(
     "_RequiredRecurrenceSettingsTypeDef",
     {
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
@@ -1332,96 +1351,149 @@
 
 class RecurrenceSettingsTypeDef(
     _RequiredRecurrenceSettingsTypeDef, _OptionalRecurrenceSettingsTypeDef
 ):
     pass
 
 
+ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    {
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEngagementsRequestRequestTypeDef = TypedDict(
+    "ListEngagementsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+    },
+    total=False,
+)
+
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationShiftsResultTypeDef = TypedDict(
     "ListRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PlanOutputTypeDef = TypedDict(
+    "PlanOutputTypeDef",
+    {
+        "Stages": List[StageOutputTypeDef],
+        "RotationIds": List[str],
+    },
+    total=False,
+)
+
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
         "RotationIds": Sequence[str],
     },
     total=False,
 )
 
+GetRotationResultTypeDef = TypedDict(
+    "GetRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRotationTypeDef = TypedDict(
+    "_RequiredRotationTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+    },
+)
+_OptionalRotationTypeDef = TypedDict(
+    "_OptionalRotationTypeDef",
+    {
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
+    pass
+
+
 _RequiredCreateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationRequestRequestTypeDef",
     {
         "Name": str,
         "ContactIds": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalCreateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRotationRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "IdempotencyToken": str,
     },
     total=False,
 )
 
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
 
-GetRotationResultTypeDef = TypedDict(
-    "GetRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
     _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
@@ -1429,25 +1501,25 @@
 ):
     pass
 
 
 _RequiredListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
@@ -1455,61 +1527,51 @@
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredRotationTypeDef = TypedDict(
-    "_RequiredRotationTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-    },
-)
-_OptionalRotationTypeDef = TypedDict(
-    "_OptionalRotationTypeDef",
-    {
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
-    pass
-
-
+RecurrenceSettingsUnionTypeDef = Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef]
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalUpdateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRotationRequestRequestTypeDef",
     {
         "ContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "TimeZoneId": str,
     },
     total=False,
 )
 
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
 ):
     pass
 
 
+GetContactResultTypeDef = TypedDict(
+    "GetContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "Alias": str,
+        "DisplayName": str,
+        "Type": ContactTypeType,
+        "Plan": PlanOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateContactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactRequestRequestTypeDef",
     {
         "Alias": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
     },
@@ -1527,26 +1589,15 @@
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
 
-GetContactResultTypeDef = TypedDict(
-    "GetContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "Alias": str,
-        "DisplayName": str,
-        "Type": ContactTypeType,
-        "Plan": PlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+PlanUnionTypeDef = Union[PlanTypeDef, PlanOutputTypeDef]
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
@@ -1566,10 +1617,10 @@
 
 
 ListRotationsResultTypeDef = TypedDict(
     "ListRotationsResultTypeDef",
     {
         "NextToken": str,
         "Rotations": List[RotationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts/type_defs.pyi` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ssm_contacts.type_defs import AcceptPageRequestRequestTypeDef
 
-    data: AcceptPageRequestRequestTypeDef = {...}
+    data: AcceptPageRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -35,105 +35,111 @@
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
     "ChannelTargetInfoTypeDef",
     "ContactChannelAddressTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
     "HandOffTimeTypeDef",
-    "CreateContactChannelResultTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "CreateContactResultTypeDef",
-    "CreateRotationOverrideRequestRequestTypeDef",
-    "CreateRotationOverrideResultTypeDef",
-    "CreateRotationResultTypeDef",
+    "TimestampTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteRotationOverrideRequestRequestTypeDef",
     "DeleteRotationRequestRequestTypeDef",
     "DescribeEngagementRequestRequestTypeDef",
-    "DescribeEngagementResultTypeDef",
     "DescribePageRequestRequestTypeDef",
-    "DescribePageResultTypeDef",
     "EngagementTypeDef",
     "GetContactChannelRequestRequestTypeDef",
     "GetContactPolicyRequestRequestTypeDef",
-    "GetContactPolicyResultTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetRotationOverrideRequestRequestTypeDef",
-    "GetRotationOverrideResultTypeDef",
     "GetRotationRequestRequestTypeDef",
-    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListContactChannelsRequestRequestTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "TimeRangeTypeDef",
-    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageReceiptsRequestRequestTypeDef",
     "ReceiptTypeDef",
-    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPageResolutionsRequestRequestTypeDef",
     "ResolutionContactTypeDef",
-    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
     "ListPagesByContactRequestRequestTypeDef",
     "PageTypeDef",
-    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
     "ListPagesByEngagementRequestRequestTypeDef",
-    "PreviewOverrideTypeDef",
-    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
-    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    "ListRotationShiftsRequestRequestTypeDef",
-    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
-    "StartEngagementResultTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
-    "GetContactChannelResultTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
     "TargetTypeDef",
-    "ListContactsResultTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
+    "CreateContactChannelResultTypeDef",
+    "CreateContactResultTypeDef",
+    "CreateRotationOverrideResultTypeDef",
+    "CreateRotationResultTypeDef",
+    "DescribeEngagementResultTypeDef",
+    "DescribePageResultTypeDef",
+    "GetContactChannelResultTypeDef",
+    "GetContactPolicyResultTypeDef",
+    "GetRotationOverrideResultTypeDef",
+    "ListContactsResultTypeDef",
+    "StartEngagementResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateRotationOverrideRequestRequestTypeDef",
+    "ListRotationOverridesRequestRequestTypeDef",
+    "ListRotationShiftsRequestRequestTypeDef",
+    "PreviewOverrideTypeDef",
+    "TimeRangeTypeDef",
     "ListEngagementsResultTypeDef",
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
-    "ListEngagementsRequestRequestTypeDef",
+    "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
+    "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    "ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    "ListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    "ListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    "ListRotationsRequestListRotationsPaginateTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
+    "StageOutputTypeDef",
     "StageTypeDef",
+    "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    "ListEngagementsRequestRequestTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
     "ListRotationShiftsResultTypeDef",
+    "PlanOutputTypeDef",
     "PlanTypeDef",
-    "CreateRotationRequestRequestTypeDef",
     "GetRotationResultTypeDef",
+    "RotationTypeDef",
+    "CreateRotationRequestRequestTypeDef",
     "ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     "ListPreviewRotationShiftsRequestRequestTypeDef",
-    "RotationTypeDef",
+    "RecurrenceSettingsUnionTypeDef",
     "UpdateRotationRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "GetContactResultTypeDef",
+    "CreateContactRequestRequestTypeDef",
+    "PlanUnionTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "ListRotationsResultTypeDef",
 )
 
 _RequiredAcceptPageRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptPageRequestRequestTypeDef",
     {
@@ -234,78 +240,35 @@
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
 
-CreateContactChannelResultTypeDef = TypedDict(
-    "CreateContactChannelResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ContactChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-CreateContactResultTypeDef = TypedDict(
-    "CreateContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "NewContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
-    {
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-class CreateRotationOverrideRequestRequestTypeDef(
-    _RequiredCreateRotationOverrideRequestRequestTypeDef,
-    _OptionalCreateRotationOverrideRequestRequestTypeDef,
-):
-    pass
-
-CreateRotationOverrideResultTypeDef = TypedDict(
-    "CreateRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRotationResultTypeDef = TypedDict(
-    "CreateRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DeactivateContactChannelRequestRequestTypeDef = TypedDict(
     "DeactivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 
@@ -341,57 +304,21 @@
 DescribeEngagementRequestRequestTypeDef = TypedDict(
     "DescribeEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 
-DescribeEngagementResultTypeDef = TypedDict(
-    "DescribeEngagementResultTypeDef",
-    {
-        "ContactArn": str,
-        "EngagementArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "StartTime": datetime,
-        "StopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePageRequestRequestTypeDef = TypedDict(
     "DescribePageRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 
-DescribePageResultTypeDef = TypedDict(
-    "DescribePageResultTypeDef",
-    {
-        "PageArn": str,
-        "EngagementArn": str,
-        "ContactArn": str,
-        "Sender": str,
-        "Subject": str,
-        "Content": str,
-        "PublicSubject": str,
-        "PublicContent": str,
-        "IncidentId": str,
-        "SentTime": datetime,
-        "ReadTime": datetime,
-        "DeliveryTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngagementTypeDef = TypedDict(
     "_RequiredEngagementTypeDef",
     {
         "EngagementArn": str,
         "ContactArn": str,
         "Sender": str,
     },
@@ -419,23 +346,14 @@
 GetContactPolicyRequestRequestTypeDef = TypedDict(
     "GetContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
     },
 )
 
-GetContactPolicyResultTypeDef = TypedDict(
-    "GetContactPolicyResultTypeDef",
-    {
-        "ContactArn": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 
@@ -443,54 +361,31 @@
     "GetRotationOverrideRequestRequestTypeDef",
     {
         "RotationId": str,
         "RotationOverrideId": str,
     },
 )
 
-GetRotationOverrideResultTypeDef = TypedDict(
-    "GetRotationOverrideResultTypeDef",
-    {
-        "RotationOverrideId": str,
-        "RotationArn": str,
-        "NewContactIds": List[str],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRotationRequestRequestTypeDef = TypedDict(
     "GetRotationRequestRequestTypeDef",
     {
         "RotationId": str,
     },
 )
 
-_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
-    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
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
 
-class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
-    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
-    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
-):
-    pass
-
 _RequiredListContactChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactChannelsRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListContactChannelsRequestRequestTypeDef = TypedDict(
@@ -504,64 +399,25 @@
 
 class ListContactChannelsRequestRequestTypeDef(
     _RequiredListContactChannelsRequestRequestTypeDef,
     _OptionalListContactChannelsRequestRequestTypeDef,
 ):
     pass
 
-ListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "ListContactsRequestListContactsPaginateTypeDef",
-    {
-        "AliasPrefix": str,
-        "Type": ContactTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListContactsRequestRequestTypeDef = TypedDict(
     "ListContactsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "AliasPrefix": str,
         "Type": ContactTypeType,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
-    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
-    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPageReceiptsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageReceiptsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageReceiptsRequestRequestTypeDef = TypedDict(
@@ -593,34 +449,14 @@
     },
     total=False,
 )
 
 class ReceiptTypeDef(_RequiredReceiptTypeDef, _OptionalReceiptTypeDef):
     pass
 
-_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PageId": str,
-    },
-)
-_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
-    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPageResolutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPageResolutionsRequestRequestTypeDef",
     {
         "PageId": str,
     },
 )
 _OptionalListPageResolutionsRequestRequestTypeDef = TypedDict(
@@ -653,34 +489,14 @@
 )
 
 class ResolutionContactTypeDef(
     _RequiredResolutionContactTypeDef, _OptionalResolutionContactTypeDef
 ):
     pass
 
-_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "ContactId": str,
-    },
-)
-_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
-    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
-    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
-):
-    pass
-
 _RequiredListPagesByContactRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalListPagesByContactRequestRequestTypeDef = TypedDict(
@@ -717,34 +533,14 @@
     },
     total=False,
 )
 
 class PageTypeDef(_RequiredPageTypeDef, _OptionalPageTypeDef):
     pass
 
-_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "EngagementId": str,
-    },
-)
-_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
-    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
-    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
-):
-    pass
-
 _RequiredListPagesByEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredListPagesByEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalListPagesByEngagementRequestRequestTypeDef = TypedDict(
@@ -758,134 +554,25 @@
 
 class ListPagesByEngagementRequestRequestTypeDef(
     _RequiredListPagesByEngagementRequestRequestTypeDef,
     _OptionalListPagesByEngagementRequestRequestTypeDef,
 ):
     pass
 
-PreviewOverrideTypeDef = TypedDict(
-    "PreviewOverrideTypeDef",
-    {
-        "NewMembers": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
-    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-):
-    pass
-
-_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationOverridesRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationOverridesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListRotationOverridesRequestRequestTypeDef(
-    _RequiredListRotationOverridesRequestRequestTypeDef,
-    _OptionalListRotationOverridesRequestRequestTypeDef,
-):
-    pass
-
 RotationOverrideTypeDef = TypedDict(
     "RotationOverrideTypeDef",
     {
         "RotationOverrideId": str,
         "NewContactIds": List[str],
         "StartTime": datetime,
         "EndTime": datetime,
         "CreateTime": datetime,
     },
 )
 
-_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
-    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-):
-    pass
-
-_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_RequiredListRotationShiftsRequestRequestTypeDef",
-    {
-        "RotationId": str,
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
-    "_OptionalListRotationShiftsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListRotationShiftsRequestRequestTypeDef(
-    _RequiredListRotationShiftsRequestRequestTypeDef,
-    _OptionalListRotationShiftsRequestRequestTypeDef,
-):
-    pass
-
-ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
-    "ListRotationsRequestListRotationsPaginateTypeDef",
-    {
-        "RotationNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRotationsRequestRequestTypeDef = TypedDict(
     "ListRotationsRequestRequestTypeDef",
     {
         "RotationNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -895,43 +582,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
         "Policy": str,
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
 ShiftDetailsTypeDef = TypedDict(
     "ShiftDetailsTypeDef",
     {
         "OverriddenContactIds": List[str],
     },
 )
 
@@ -963,22 +629,14 @@
 )
 
 class StartEngagementRequestRequestTypeDef(
     _RequiredStartEngagementRequestRequestTypeDef, _OptionalStartEngagementRequestRequestTypeDef
 ):
     pass
 
-StartEngagementResultTypeDef = TypedDict(
-    "StartEngagementResultTypeDef",
-    {
-        "EngagementArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopEngagementRequestRequestTypeDef = TypedDict(
     "_RequiredStopEngagementRequestRequestTypeDef",
     {
         "EngagementId": str,
     },
 )
 _OptionalStopEngagementRequestRequestTypeDef = TypedDict(
@@ -1043,27 +701,14 @@
 
 class CreateContactChannelRequestRequestTypeDef(
     _RequiredCreateContactChannelRequestRequestTypeDef,
     _OptionalCreateContactChannelRequestRequestTypeDef,
 ):
     pass
 
-GetContactChannelResultTypeDef = TypedDict(
-    "GetContactChannelResultTypeDef",
-    {
-        "ContactArn": str,
-        "ContactChannelArn": str,
-        "Name": str,
-        "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressTypeDef,
-        "ActivationStatus": ActivationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalUpdateContactChannelRequestRequestTypeDef = TypedDict(
@@ -1086,23 +731,14 @@
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
-ListContactsResultTypeDef = TypedDict(
-    "ListContactsResultTypeDef",
-    {
-        "NextToken": str,
-        "Contacts": List[ContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
         "End": HandOffTimeTypeDef,
     },
     total=False,
@@ -1120,102 +756,452 @@
     "WeeklySettingTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "HandOffTime": HandOffTimeTypeDef,
     },
 )
 
+CreateContactChannelResultTypeDef = TypedDict(
+    "CreateContactChannelResultTypeDef",
+    {
+        "ContactChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContactResultTypeDef = TypedDict(
+    "CreateContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationOverrideResultTypeDef = TypedDict(
+    "CreateRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRotationResultTypeDef = TypedDict(
+    "CreateRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEngagementResultTypeDef = TypedDict(
+    "DescribeEngagementResultTypeDef",
+    {
+        "ContactArn": str,
+        "EngagementArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "StartTime": datetime,
+        "StopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePageResultTypeDef = TypedDict(
+    "DescribePageResultTypeDef",
+    {
+        "PageArn": str,
+        "EngagementArn": str,
+        "ContactArn": str,
+        "Sender": str,
+        "Subject": str,
+        "Content": str,
+        "PublicSubject": str,
+        "PublicContent": str,
+        "IncidentId": str,
+        "SentTime": datetime,
+        "ReadTime": datetime,
+        "DeliveryTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactChannelResultTypeDef = TypedDict(
+    "GetContactChannelResultTypeDef",
+    {
+        "ContactArn": str,
+        "ContactChannelArn": str,
+        "Name": str,
+        "Type": ChannelTypeType,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
+        "ActivationStatus": ActivationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactPolicyResultTypeDef = TypedDict(
+    "GetContactPolicyResultTypeDef",
+    {
+        "ContactArn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRotationOverrideResultTypeDef = TypedDict(
+    "GetRotationOverrideResultTypeDef",
+    {
+        "RotationOverrideId": str,
+        "RotationArn": str,
+        "NewContactIds": List[str],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContactsResultTypeDef = TypedDict(
+    "ListContactsResultTypeDef",
+    {
+        "NextToken": str,
+        "Contacts": List[ContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartEngagementResultTypeDef = TypedDict(
+    "StartEngagementResultTypeDef",
+    {
+        "EngagementArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "NewContactIds": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateRotationOverrideRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRotationOverrideRequestRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+class CreateRotationOverrideRequestRequestTypeDef(
+    _RequiredCreateRotationOverrideRequestRequestTypeDef,
+    _OptionalCreateRotationOverrideRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationOverridesRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListRotationOverridesRequestRequestTypeDef(
+    _RequiredListRotationOverridesRequestRequestTypeDef,
+    _OptionalListRotationOverridesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestRequestTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationShiftsRequestRequestTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListRotationShiftsRequestRequestTypeDef(
+    _RequiredListRotationShiftsRequestRequestTypeDef,
+    _OptionalListRotationShiftsRequestRequestTypeDef,
+):
+    pass
+
+PreviewOverrideTypeDef = TypedDict(
+    "PreviewOverrideTypeDef",
+    {
+        "NewMembers": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 ListEngagementsResultTypeDef = TypedDict(
     "ListEngagementsResultTypeDef",
     {
         "NextToken": str,
         "Engagements": List[EngagementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
-    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef",
     {
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ContactId": str,
+    },
+)
+_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef = TypedDict(
+    "_OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListEngagementsRequestRequestTypeDef = TypedDict(
-    "ListEngagementsRequestRequestTypeDef",
+class ListContactChannelsRequestListContactChannelsPaginateTypeDef(
+    _RequiredListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    _OptionalListContactChannelsRequestListContactChannelsPaginateTypeDef,
+):
+    pass
+
+ListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "ListContactsRequestListContactsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "IncidentId": str,
-        "TimeRangeValue": TimeRangeTypeDef,
+        "AliasPrefix": str,
+        "Type": ContactTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef = TypedDict(
+    "_OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPageReceiptsRequestListPageReceiptsPaginateTypeDef(
+    _RequiredListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    _OptionalListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PageId": str,
+    },
+)
+_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPageResolutionsRequestListPageResolutionsPaginateTypeDef(
+    _RequiredListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    _OptionalListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "ContactId": str,
+    },
+)
+_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPagesByContactRequestListPagesByContactPaginateTypeDef(
+    _RequiredListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    _OptionalListPagesByContactRequestListPagesByContactPaginateTypeDef,
+):
+    pass
+
+_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "EngagementId": str,
+    },
+)
+_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef = TypedDict(
+    "_OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef(
+    _RequiredListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    _OptionalListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+):
+    pass
+
+_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "RotationId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef = TypedDict(
+    "_OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRotationOverridesRequestListRotationOverridesPaginateTypeDef(
+    _RequiredListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    _OptionalListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+):
+    pass
+
+_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "RotationId": str,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef = TypedDict(
+    "_OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRotationShiftsRequestListRotationShiftsPaginateTypeDef(
+    _RequiredListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    _OptionalListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+):
+    pass
+
+ListRotationsRequestListRotationsPaginateTypeDef = TypedDict(
+    "ListRotationsRequestListRotationsPaginateTypeDef",
+    {
+        "RotationNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPageReceiptsResultTypeDef = TypedDict(
     "ListPageReceiptsResultTypeDef",
     {
         "NextToken": str,
         "Receipts": List[ReceiptTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPageResolutionsResultTypeDef = TypedDict(
     "ListPageResolutionsResultTypeDef",
     {
         "NextToken": str,
         "PageResolutions": List[ResolutionContactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByContactResultTypeDef = TypedDict(
     "ListPagesByContactResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPagesByEngagementResultTypeDef = TypedDict(
     "ListPagesByEngagementResultTypeDef",
     {
         "NextToken": str,
         "Pages": List[PageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationOverridesResultTypeDef = TypedDict(
     "ListRotationOverridesResultTypeDef",
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
@@ -1236,26 +1222,57 @@
     pass
 
 ListContactChannelsResultTypeDef = TypedDict(
     "ListContactChannelsResultTypeDef",
     {
         "NextToken": str,
         "ContactChannels": List[ContactChannelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StageOutputTypeDef = TypedDict(
+    "StageOutputTypeDef",
+    {
+        "DurationInMinutes": int,
+        "Targets": List[TargetTypeDef],
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
         "Targets": Sequence[TargetTypeDef],
     },
 )
 
+_RequiredRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_RequiredRecurrenceSettingsOutputTypeDef",
+    {
+        "NumberOfOnCalls": int,
+        "RecurrenceMultiplier": int,
+    },
+)
+_OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
+    "_OptionalRecurrenceSettingsOutputTypeDef",
+    {
+        "MonthlySettings": List[MonthlySettingTypeDef],
+        "WeeklySettings": List[WeeklySettingTypeDef],
+        "DailySettings": List[HandOffTimeTypeDef],
+        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeTypeDef]],
+    },
+    total=False,
+)
+
+class RecurrenceSettingsOutputTypeDef(
+    _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
+):
+    pass
+
 _RequiredRecurrenceSettingsTypeDef = TypedDict(
     "_RequiredRecurrenceSettingsTypeDef",
     {
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
@@ -1271,174 +1288,217 @@
 )
 
 class RecurrenceSettingsTypeDef(
     _RequiredRecurrenceSettingsTypeDef, _OptionalRecurrenceSettingsTypeDef
 ):
     pass
 
+ListEngagementsRequestListEngagementsPaginateTypeDef = TypedDict(
+    "ListEngagementsRequestListEngagementsPaginateTypeDef",
+    {
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEngagementsRequestRequestTypeDef = TypedDict(
+    "ListEngagementsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "IncidentId": str,
+        "TimeRangeValue": TimeRangeTypeDef,
+    },
+    total=False,
+)
+
 ListPreviewRotationShiftsResultTypeDef = TypedDict(
     "ListPreviewRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRotationShiftsResultTypeDef = TypedDict(
     "ListRotationShiftsResultTypeDef",
     {
         "RotationShifts": List[RotationShiftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PlanOutputTypeDef = TypedDict(
+    "PlanOutputTypeDef",
+    {
+        "Stages": List[StageOutputTypeDef],
+        "RotationIds": List[str],
+    },
+    total=False,
+)
+
 PlanTypeDef = TypedDict(
     "PlanTypeDef",
     {
         "Stages": Sequence[StageTypeDef],
         "RotationIds": Sequence[str],
     },
     total=False,
 )
 
+GetRotationResultTypeDef = TypedDict(
+    "GetRotationResultTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRotationTypeDef = TypedDict(
+    "_RequiredRotationTypeDef",
+    {
+        "RotationArn": str,
+        "Name": str,
+    },
+)
+_OptionalRotationTypeDef = TypedDict(
+    "_OptionalRotationTypeDef",
+    {
+        "ContactIds": List[str],
+        "StartTime": datetime,
+        "TimeZoneId": str,
+        "Recurrence": RecurrenceSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
+    pass
+
 _RequiredCreateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRotationRequestRequestTypeDef",
     {
         "Name": str,
         "ContactIds": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalCreateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRotationRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "Tags": Sequence[TagTypeDef],
         "IdempotencyToken": str,
     },
     total=False,
 )
 
 class CreateRotationRequestRequestTypeDef(
     _RequiredCreateRotationRequestRequestTypeDef, _OptionalCreateRotationRequestRequestTypeDef
 ):
     pass
 
-GetRotationResultTypeDef = TypedDict(
-    "GetRotationResultTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef(
     _RequiredListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     _OptionalListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
 ):
     pass
 
 _RequiredListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_RequiredListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "EndTime": Union[datetime, str],
+        "EndTime": TimestampTypeDef,
         "Members": Sequence[str],
         "TimeZoneId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalListPreviewRotationShiftsRequestRequestTypeDef = TypedDict(
     "_OptionalListPreviewRotationShiftsRequestRequestTypeDef",
     {
-        "RotationStartTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
+        "RotationStartTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
         "Overrides": Sequence[PreviewOverrideTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class ListPreviewRotationShiftsRequestRequestTypeDef(
     _RequiredListPreviewRotationShiftsRequestRequestTypeDef,
     _OptionalListPreviewRotationShiftsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredRotationTypeDef = TypedDict(
-    "_RequiredRotationTypeDef",
-    {
-        "RotationArn": str,
-        "Name": str,
-    },
-)
-_OptionalRotationTypeDef = TypedDict(
-    "_OptionalRotationTypeDef",
-    {
-        "ContactIds": List[str],
-        "StartTime": datetime,
-        "TimeZoneId": str,
-        "Recurrence": RecurrenceSettingsTypeDef,
-    },
-    total=False,
-)
-
-class RotationTypeDef(_RequiredRotationTypeDef, _OptionalRotationTypeDef):
-    pass
-
+RecurrenceSettingsUnionTypeDef = Union[RecurrenceSettingsTypeDef, RecurrenceSettingsOutputTypeDef]
 _RequiredUpdateRotationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRotationRequestRequestTypeDef",
     {
         "RotationId": str,
         "Recurrence": RecurrenceSettingsTypeDef,
     },
 )
 _OptionalUpdateRotationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRotationRequestRequestTypeDef",
     {
         "ContactIds": Sequence[str],
-        "StartTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
         "TimeZoneId": str,
     },
     total=False,
 )
 
 class UpdateRotationRequestRequestTypeDef(
     _RequiredUpdateRotationRequestRequestTypeDef, _OptionalUpdateRotationRequestRequestTypeDef
 ):
     pass
 
+GetContactResultTypeDef = TypedDict(
+    "GetContactResultTypeDef",
+    {
+        "ContactArn": str,
+        "Alias": str,
+        "DisplayName": str,
+        "Type": ContactTypeType,
+        "Plan": PlanOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateContactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContactRequestRequestTypeDef",
     {
         "Alias": str,
         "Type": ContactTypeType,
         "Plan": PlanTypeDef,
     },
@@ -1454,26 +1514,15 @@
 )
 
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
-GetContactResultTypeDef = TypedDict(
-    "GetContactResultTypeDef",
-    {
-        "ContactArn": str,
-        "Alias": str,
-        "DisplayName": str,
-        "Type": ContactTypeType,
-        "Plan": PlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+PlanUnionTypeDef = Union[PlanTypeDef, PlanOutputTypeDef]
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactId": str,
     },
 )
 _OptionalUpdateContactRequestRequestTypeDef = TypedDict(
@@ -1491,10 +1540,10 @@
     pass
 
 ListRotationsResultTypeDef = TypedDict(
     "ListRotationsResultTypeDef",
     {
         "NextToken": str,
         "Rotations": List[RotationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ssm-contacts
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSMContacts 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ssm-contacts type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ssm-contacts type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ssm-contacts"></a>
 
 # types-aiobotocore-ssm-contacts
 
 [![PyPI - types-aiobotocore-ssm-contacts](https://img.shields.io/pypi/v/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ssm-contacts.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ssm-contacts?color=blue)](https://pypistats.org/packages/types-aiobotocore-ssm-contacts)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ssm-contacts)](https://pepy.tech/project/types-aiobotocore-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSMContacts 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [types-aiobotocore-ssm-contacts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ssm_contacts/).
 
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
@@ -360,127 +359,133 @@
 )
 
 
 def check_value(value: AcceptCodeValidationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ssm_contacts.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
     ChannelTargetInfoTypeDef,
     ContactChannelAddressTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
     HandOffTimeTypeDef,
-    CreateContactChannelResultTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    CreateContactResultTypeDef,
-    CreateRotationOverrideRequestRequestTypeDef,
-    CreateRotationOverrideResultTypeDef,
-    CreateRotationResultTypeDef,
+    TimestampTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteRotationOverrideRequestRequestTypeDef,
     DeleteRotationRequestRequestTypeDef,
     DescribeEngagementRequestRequestTypeDef,
-    DescribeEngagementResultTypeDef,
     DescribePageRequestRequestTypeDef,
-    DescribePageResultTypeDef,
     EngagementTypeDef,
     GetContactChannelRequestRequestTypeDef,
     GetContactPolicyRequestRequestTypeDef,
-    GetContactPolicyResultTypeDef,
     GetContactRequestRequestTypeDef,
     GetRotationOverrideRequestRequestTypeDef,
-    GetRotationOverrideResultTypeDef,
     GetRotationRequestRequestTypeDef,
-    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContactChannelsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
-    TimeRangeTypeDef,
-    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageReceiptsRequestRequestTypeDef,
     ReceiptTypeDef,
-    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPageResolutionsRequestRequestTypeDef,
     ResolutionContactTypeDef,
-    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
     ListPagesByContactRequestRequestTypeDef,
     PageTypeDef,
-    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
     ListPagesByEngagementRequestRequestTypeDef,
-    PreviewOverrideTypeDef,
-    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
-    ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
-    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
-    ListRotationShiftsRequestRequestTypeDef,
-    ListRotationsRequestListRotationsPaginateTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutContactPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
-    StartEngagementResultTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
-    GetContactChannelResultTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
     TargetTypeDef,
-    ListContactsResultTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
+    CreateContactChannelResultTypeDef,
+    CreateContactResultTypeDef,
+    CreateRotationOverrideResultTypeDef,
+    CreateRotationResultTypeDef,
+    DescribeEngagementResultTypeDef,
+    DescribePageResultTypeDef,
+    GetContactChannelResultTypeDef,
+    GetContactPolicyResultTypeDef,
+    GetRotationOverrideResultTypeDef,
+    ListContactsResultTypeDef,
+    StartEngagementResultTypeDef,
     ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateRotationOverrideRequestRequestTypeDef,
+    ListRotationOverridesRequestRequestTypeDef,
+    ListRotationShiftsRequestRequestTypeDef,
+    PreviewOverrideTypeDef,
+    TimeRangeTypeDef,
     ListEngagementsResultTypeDef,
-    ListEngagementsRequestListEngagementsPaginateTypeDef,
-    ListEngagementsRequestRequestTypeDef,
+    ListContactChannelsRequestListContactChannelsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
+    ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
+    ListPagesByContactRequestListPagesByContactPaginateTypeDef,
+    ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef,
+    ListRotationOverridesRequestListRotationOverridesPaginateTypeDef,
+    ListRotationShiftsRequestListRotationShiftsPaginateTypeDef,
+    ListRotationsRequestListRotationsPaginateTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
+    StageOutputTypeDef,
     StageTypeDef,
+    RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
+    ListEngagementsRequestListEngagementsPaginateTypeDef,
+    ListEngagementsRequestRequestTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
     ListRotationShiftsResultTypeDef,
+    PlanOutputTypeDef,
     PlanTypeDef,
-    CreateRotationRequestRequestTypeDef,
     GetRotationResultTypeDef,
+    RotationTypeDef,
+    CreateRotationRequestRequestTypeDef,
     ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef,
     ListPreviewRotationShiftsRequestRequestTypeDef,
-    RotationTypeDef,
+    RecurrenceSettingsUnionTypeDef,
     UpdateRotationRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResultTypeDef,
+    CreateContactRequestRequestTypeDef,
+    PlanUnionTypeDef,
     UpdateContactRequestRequestTypeDef,
     ListRotationsResultTypeDef,
 )
 
 
-def get_structure() -> AcceptPageRequestRequestTypeDef:
+def get_value() -> AcceptPageRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ssm-contacts-2.5.2/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt` & `types-aiobotocore-ssm-contacts-2.5.2.post1/types_aiobotocore_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*


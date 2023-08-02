# Comparing `tmp/types-aiobotocore-sesv2-2.5.2.tar.gz` & `tmp/types-aiobotocore-sesv2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sesv2-2.5.2.tar", last modified: Sat Jul  8 01:44:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-sesv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
```

## Comparing `types-aiobotocore-sesv2-2.5.2.tar` & `types-aiobotocore-sesv2-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.758902 types-aiobotocore-sesv2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-07-08 01:44:19.758902 types-aiobotocore-sesv2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:19.758902 types-aiobotocore-sesv2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.758902 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59902 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59807 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69255 2023-07-08 01:41:05.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69185 2023-07-08 01:41:04.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:03.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.758902 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-07-08 01:44:19.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-08 01:44:19.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:19.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:44:19.000000 types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.537456 types-aiobotocore-sesv2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-08-02 14:53:01.533456 types-aiobotocore-sesv2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.537456 types-aiobotocore-sesv2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.529456 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59893 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59798 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-08-02 14:49:43.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71044 2023-08-02 14:49:44.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70974 2023-08-02 14:49:44.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:42.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.533456 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:53:01.000000 types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sesv2-2.5.2/LICENSE` & `types-aiobotocore-sesv2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sesv2-2.5.2/PKG-INFO` & `types-aiobotocore-sesv2-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sesv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SESV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SESV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sesv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sesv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sesv2"></a>
 
 # types-aiobotocore-sesv2
 
 [![PyPI - types-aiobotocore-sesv2](https://img.shields.io/pypi/v/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sesv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-sesv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sesv2)](https://pepy.tech/project/types-aiobotocore-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SESV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [types-aiobotocore-sesv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/).
 
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
@@ -312,52 +311,51 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sesv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sesv2.type_defs import (
     ReviewDetailsTypeDef,
-    BatchGetMetricDataQueryTypeDef,
+    TimestampTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
+    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
     TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
-    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DashboardAttributesTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
@@ -369,64 +367,59 @@
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SuppressionOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    ListSuppressedDestinationsRequestRequestTypeDef,
     SuppressedDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountDetailsRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
@@ -435,36 +428,47 @@
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
-    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    BatchGetMetricDataRequestRequestTypeDef,
+    BatchGetMetricDataQueryTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListSuppressedDestinationsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     BatchGetMetricDataResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    CreateImportJobResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
     CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
     UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
@@ -484,58 +488,63 @@
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    SuppressionOptionsUnionTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
+    BatchGetMetricDataRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
     CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ReviewDetailsTypeDef:
+def get_value() -> ReviewDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sesv2-2.5.2/README.md` & `types-aiobotocore-sesv2-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sesv2"></a>
 
 # types-aiobotocore-sesv2
 
 [![PyPI - types-aiobotocore-sesv2](https://img.shields.io/pypi/v/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sesv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-sesv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sesv2)](https://pepy.tech/project/types-aiobotocore-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SESV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [types-aiobotocore-sesv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/).
 
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
@@ -279,52 +279,51 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sesv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sesv2.type_defs import (
     ReviewDetailsTypeDef,
-    BatchGetMetricDataQueryTypeDef,
+    TimestampTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
+    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
     TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
-    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DashboardAttributesTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
@@ -336,64 +335,59 @@
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SuppressionOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    ListSuppressedDestinationsRequestRequestTypeDef,
     SuppressedDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountDetailsRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
@@ -402,36 +396,47 @@
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
-    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    BatchGetMetricDataRequestRequestTypeDef,
+    BatchGetMetricDataQueryTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListSuppressedDestinationsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     BatchGetMetricDataResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    CreateImportJobResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
     CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
     UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
@@ -451,58 +456,63 @@
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    SuppressionOptionsUnionTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
+    BatchGetMetricDataRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
     CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ReviewDetailsTypeDef:
+def get_value() -> ReviewDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sesv2-2.5.2/setup.py` & `types-aiobotocore-sesv2-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sesv2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SESV2 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore sesv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sesv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sesv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/"
```

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/__main__.py` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SESV2 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SESV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/client.py` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_sesv2.client import SESV2Client
 
     session = get_session()
     async with session.create_client("sesv2") as client:
         client: SESV2Client
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BehaviorOnMxFailureType,
     ContactLanguageType,
@@ -38,15 +37,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -80,22 +79,23 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsTypeDef,
+    SuppressionOptionsUnionTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
+    TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
 )
 
@@ -172,18 +172,18 @@
 
     async def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsTypeDef = ...,
+        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set)
@@ -555,15 +555,15 @@
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_deliverability_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#get_domain_deliverability_campaign)
         """
 
     async def get_domain_statistics_report(
-        self, *, Domain: str, StartDate: Union[datetime, str], EndDate: Union[datetime, str]
+        self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_statistics_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#get_domain_statistics_report)
@@ -686,16 +686,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_deliverability_test_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_deliverability_test_reports)
         """
 
     async def list_domain_deliverability_campaigns(
         self,
         *,
-        StartDate: Union[datetime, str],
-        EndDate: Union[datetime, str],
+        StartDate: TimestampTypeDef,
+        EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time range.
@@ -755,16 +755,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_recommendations)
         """
 
     async def list_suppressed_destinations(
         self,
         *,
         Reasons: Sequence[SuppressionListReasonType] = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListSuppressedDestinationsResponseTypeDef:
         """
         Retrieves a list of email addresses that are on the suppression list for your
         account.
 
@@ -939,15 +939,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
 
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/client.pyi` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_sesv2.client import SESV2Client
 
     session = get_session()
     async with session.create_client("sesv2") as client:
         client: SESV2Client
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BehaviorOnMxFailureType,
     ContactLanguageType,
@@ -38,15 +37,15 @@
     BulkEmailEntryTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateImportJobResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
     DkimSigningAttributesTypeDef,
-    DomainDeliverabilityTrackingOptionTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     EmailContentTypeDef,
     EmailTemplateContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
@@ -80,22 +79,23 @@
     ListImportJobsResponseTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
     PutEmailIdentityDkimSigningAttributesResponseTypeDef,
-    ReputationOptionsTypeDef,
+    ReputationOptionsUnionTypeDef,
     SendBulkEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
-    SuppressionOptionsTypeDef,
+    SuppressionOptionsUnionTypeDef,
     TagTypeDef,
     TestRenderEmailTemplateResponseTypeDef,
+    TimestampTypeDef,
     TopicPreferenceTypeDef,
     TopicTypeDef,
     TrackingOptionsTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
 )
 
@@ -165,18 +165,18 @@
         """
     async def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsTypeDef = ...,
+        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SuppressionOptions: SuppressionOptionsTypeDef = ...,
+        SuppressionOptions: SuppressionOptionsUnionTypeDef = ...,
         VdmOptions: VdmOptionsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#create_configuration_set)
@@ -513,15 +513,15 @@
         """
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_deliverability_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#get_domain_deliverability_campaign)
         """
     async def get_domain_statistics_report(
-        self, *, Domain: str, StartDate: Union[datetime, str], EndDate: Union[datetime, str]
+        self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.get_domain_statistics_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#get_domain_statistics_report)
@@ -632,16 +632,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_deliverability_test_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_deliverability_test_reports)
         """
     async def list_domain_deliverability_campaigns(
         self,
         *,
-        StartDate: Union[datetime, str],
-        EndDate: Union[datetime, str],
+        StartDate: TimestampTypeDef,
+        EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListDomainDeliverabilityCampaignsResponseTypeDef:
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time range.
@@ -696,16 +696,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#list_recommendations)
         """
     async def list_suppressed_destinations(
         self,
         *,
         Reasons: Sequence[SuppressionListReasonType] = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         PageSize: int = ...
     ) -> ListSuppressedDestinationsResponseTypeDef:
         """
         Retrieves a list of email addresses that are on the suppression list for your
         account.
 
@@ -864,15 +864,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_dedicated_ip_warmup_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_dedicated_ip_warmup_attributes)
         """
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/client/#put_deliverability_dashboard_option)
         """
```

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/literals.py` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/literals.pyi` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/type_defs.py` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sesv2.type_defs import ReviewDetailsTypeDef
 
-    data: ReviewDetailsTypeDef = {...}
+    data: ReviewDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -58,45 +58,43 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ReviewDetailsTypeDef",
-    "BatchGetMetricDataQueryTypeDef",
+    "TimestampTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
+    "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
     "TopicPreferenceTypeDef",
     "DeliveryOptionsTypeDef",
-    "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
-    "CreateImportJobResponseTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DashboardAttributesTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
@@ -108,64 +106,59 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "RawMessageTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SuppressionOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
-    "GetEmailIdentityPoliciesResponseTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
     "GuardianAttributesTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "ListSuppressedDestinationsRequestRequestTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -174,36 +167,47 @@
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
-    "ResponseMetadataTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
-    "TestRenderEmailTemplateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
-    "BatchGetMetricDataRequestRequestTypeDef",
+    "BatchGetMetricDataQueryTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "BatchGetMetricDataResponseTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    "CreateImportJobResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
@@ -223,50 +227,55 @@
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
+    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
+    "BatchGetMetricDataRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -274,39 +283,15 @@
     {
         "Status": ReviewStatusType,
         "CaseId": str,
     },
     total=False,
 )
 
-_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_RequiredBatchGetMetricDataQueryTypeDef",
-    {
-        "Id": str,
-        "Namespace": Literal["VDM"],
-        "Metric": MetricType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_OptionalBatchGetMetricDataQueryTypeDef",
-    {
-        "Dimensions": Mapping[MetricDimensionNameType, str],
-    },
-    total=False,
-)
-
-
-class BatchGetMetricDataQueryTypeDef(
-    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 MetricDataErrorTypeDef = TypedDict(
     "MetricDataErrorTypeDef",
     {
         "Id": str,
         "Code": QueryErrorCodeType,
         "Message": str,
     },
@@ -319,43 +304,53 @@
         "Id": str,
         "Timestamps": List[datetime],
         "Values": List[int],
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
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
-
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
-
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateName": str,
         "TemplateArn": str,
         "TemplateData": str,
     },
@@ -429,23 +424,14 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-ReputationOptionsTypeDef = TypedDict(
-    "ReputationOptionsTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": Union[datetime, str],
-    },
-    total=False,
-)
-
 SendingOptionsTypeDef = TypedDict(
     "SendingOptionsTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -485,40 +471,29 @@
     "_OptionalTopicTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class TopicTypeDef(_RequiredTopicTypeDef, _OptionalTopicTypeDef):
     pass
 
-
 CreateCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
 )
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateEmailIdentityPolicyRequestRequestTypeDef = TypedDict(
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -562,22 +537,14 @@
     "ImportDataSourceTypeDef",
     {
         "S3Url": str,
         "DataFormat": DataFormatType,
     },
 )
 
-CreateImportJobResponseTypeDef = TypedDict(
-    "CreateImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomVerificationEmailTemplateMetadataTypeDef = TypedDict(
     "CustomVerificationEmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -645,19 +612,17 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
-
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
-
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -757,28 +722,30 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
-InboxPlacementTrackingOptionTypeDef = TypedDict(
-    "InboxPlacementTrackingOptionTypeDef",
+InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionOutputTypeDef",
     {
         "Global": bool,
         "TrackedIsps": List[str],
     },
     total=False,
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
+InboxPlacementTrackingOptionTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Global": bool,
+        "TrackedIsps": Sequence[str],
     },
+    total=False,
 )
 
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
@@ -853,14 +820,31 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+ReputationOptionsOutputTypeDef = TypedDict(
+    "ReputationOptionsOutputTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": datetime,
+    },
+    total=False,
+)
+
+SuppressionOptionsOutputTypeDef = TypedDict(
+    "SuppressionOptionsOutputTypeDef",
+    {
+        "SuppressedReasons": List[SuppressionListReasonType],
+    },
+    total=False,
+)
+
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
@@ -875,27 +859,14 @@
 GetCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
-GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "FromEmailAddress": str,
-        "TemplateSubject": str,
-        "TemplateContent": str,
-        "SuccessRedirectionURL": str,
-        "FailureRedirectionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 
@@ -938,38 +909,21 @@
 GetDomainDeliverabilityCampaignRequestRequestTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     {
         "CampaignId": str,
     },
 )
 
-GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
-GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -1042,23 +996,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListContactListsRequestRequestTypeDef = TypedDict(
     "ListContactListsRequestRequestTypeDef",
     {
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
@@ -1087,57 +1032,23 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListDedicatedIpPoolsResponseTypeDef = TypedDict(
-    "ListDedicatedIpPoolsResponseTypeDef",
-    {
-        "DedicatedIpPools": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "SubscribedDomain": str,
-    },
-)
-_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
-
-class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
-    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-):
-    pass
-
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1172,21 +1083,19 @@
     "_OptionalListManagementOptionsTypeDef",
     {
         "TopicName": str,
     },
     total=False,
 )
 
-
 class ListManagementOptionsTypeDef(
     _RequiredListManagementOptionsTypeDef, _OptionalListManagementOptionsTypeDef
 ):
     pass
 
-
 ListRecommendationsRequestRequestTypeDef = TypedDict(
     "ListRecommendationsRequestRequestTypeDef",
     {
         "Filter": Mapping[ListRecommendationsFilterKeyType, str],
         "NextToken": str,
         "PageSize": int,
     },
@@ -1203,26 +1112,14 @@
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Impact": RecommendationImpactType,
     },
     total=False,
 )
 
-ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
-    "ListSuppressedDestinationsRequestRequestTypeDef",
-    {
-        "Reasons": Sequence[SuppressionListReasonType],
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
 SuppressedDestinationSummaryTypeDef = TypedDict(
     "SuppressedDestinationSummaryTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
         "LastUpdateTime": datetime,
     },
@@ -1257,21 +1154,19 @@
         "ContactLanguage": ContactLanguageType,
         "AdditionalContactEmailAddresses": Sequence[str],
         "ProductionAccessEnabled": bool,
     },
     total=False,
 )
 
-
 class PutAccountDetailsRequestRequestTypeDef(
     _RequiredPutAccountDetailsRequestRequestTypeDef, _OptionalPutAccountDetailsRequestRequestTypeDef
 ):
     pass
 
-
 PutAccountSendingAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountSendingAttributesRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -1295,110 +1190,100 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "SuppressedReasons": Sequence[SuppressionListReasonType],
     },
     total=False,
 )
 
-
 class PutConfigurationSetSuppressionOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -1429,75 +1314,60 @@
     "_OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-
-PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    {
-        "DkimStatus": DkimStatusType,
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -1505,22 +1375,20 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
-
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 PutSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "PutSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
     },
 )
@@ -1529,25 +1397,14 @@
     "ReplacementTemplateTypeDef",
     {
         "ReplacementTemplateData": str,
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
 _RequiredSendCustomVerificationEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "TemplateName": str,
     },
 )
@@ -1555,38 +1412,20 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
-
-SendCustomVerificationEmailResponseTypeDef = TypedDict(
-    "SendCustomVerificationEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1596,22 +1435,14 @@
     "TestRenderEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderEmailTemplateResponseTypeDef = TypedDict(
-    "TestRenderEmailTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1646,35 +1477,200 @@
         "UseCaseDescription": str,
         "AdditionalContactEmailAddresses": List[str],
         "ReviewDetails": ReviewDetailsTypeDef,
     },
     total=False,
 )
 
-BatchGetMetricDataRequestRequestTypeDef = TypedDict(
-    "BatchGetMetricDataRequestRequestTypeDef",
+_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_RequiredBatchGetMetricDataQueryTypeDef",
     {
-        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+        "Id": str,
+        "Namespace": Literal["VDM"],
+        "Metric": MetricType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_OptionalBatchGetMetricDataQueryTypeDef",
+    {
+        "Dimensions": Mapping[MetricDimensionNameType, str],
+    },
+    total=False,
+)
+
+class BatchGetMetricDataQueryTypeDef(
+    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
+):
+    pass
+
+GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+
+_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "SubscribedDomain": str,
+    },
+)
+_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
+    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+):
+    pass
+
+ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    {
+        "Reasons": Sequence[SuppressionListReasonType],
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": int,
     },
+    total=False,
+)
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImportJobResponseTypeDef = TypedDict(
+    "CreateImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "FromEmailAddress": str,
+        "TemplateSubject": str,
+        "TemplateContent": str,
+        "SuccessRedirectionURL": str,
+        "FailureRedirectionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDedicatedIpPoolsResponseTypeDef = TypedDict(
+    "ListDedicatedIpPoolsResponseTypeDef",
+    {
+        "DedicatedIpPools": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    {
+        "DkimStatus": DkimStatusType,
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderEmailTemplateResponseTypeDef = TypedDict(
+    "TestRenderEmailTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBlacklistReportsResponseTypeDef = TypedDict(
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
     },
 )
 
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
@@ -1691,15 +1687,22 @@
     total=False,
 )
 
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1707,15 +1710,15 @@
 )
 
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
@@ -1740,33 +1743,31 @@
         "TopicPreferences": Sequence[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
     },
     total=False,
 )
 
-
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
-
 GetContactResponseTypeDef = TypedDict(
     "GetContactResponseTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
         "TopicPreferences": List[TopicPreferenceTypeDef],
         "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1779,21 +1780,19 @@
         "TopicPreferences": Sequence[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
     },
     total=False,
 )
 
-
 class UpdateContactRequestRequestTypeDef(
     _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 _OptionalCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
@@ -1801,27 +1800,25 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ScalingMode": ScalingModeType,
     },
     total=False,
 )
 
-
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1841,31 +1838,29 @@
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateContactListRequestRequestTypeDef(
     _RequiredCreateContactListRequestRequestTypeDef, _OptionalCreateContactListRequestRequestTypeDef
 ):
     pass
 
-
 GetContactListResponseTypeDef = TypedDict(
     "GetContactListResponseTypeDef",
     {
         "ContactListName": str,
         "Topics": List[TopicTypeDef],
         "Description": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1876,21 +1871,19 @@
     {
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateContactListRequestRequestTypeDef(
     _RequiredUpdateContactListRequestRequestTypeDef, _OptionalUpdateContactListRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
@@ -1899,22 +1892,20 @@
         "Tags": Sequence[TagTypeDef],
         "DkimSigningAttributes": DkimSigningAttributesTypeDef,
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "SigningAttributesOrigin": DkimSigningAttributesOriginType,
     },
 )
@@ -1922,29 +1913,27 @@
     "_OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "SigningAttributes": DkimSigningAttributesTypeDef,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1953,15 +1942,15 @@
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1970,15 +1959,15 @@
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1998,80 +1987,91 @@
     total=False,
 )
 
 GetDedicatedIpPoolResponseTypeDef = TypedDict(
     "GetDedicatedIpPoolResponseTypeDef",
     {
         "DedicatedIpPool": DedicatedIpPoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpResponseTypeDef = TypedDict(
     "GetDedicatedIpResponseTypeDef",
     {
         "DedicatedIp": DedicatedIpTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
+    {
+        "Domain": str,
+        "SubscriptionStartDate": datetime,
+        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
+    },
+    total=False,
+)
+
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": datetime,
+        "SubscriptionStartDate": TimestampTypeDef,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2085,15 +2085,15 @@
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
         "Tags": List[TagTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
@@ -2104,34 +2104,32 @@
     {
         "DashboardAttributes": DashboardAttributesTypeDef,
         "GuardianAttributes": GuardianAttributesTypeDef,
     },
     total=False,
 )
 
-
 class VdmAttributesTypeDef(_RequiredVdmAttributesTypeDef, _OptionalVdmAttributesTypeDef):
     pass
 
-
 VdmOptionsTypeDef = TypedDict(
     "VdmOptionsTypeDef",
     {
         "DashboardOptions": DashboardOptionsTypeDef,
         "GuardianOptions": GuardianOptionsTypeDef,
     },
     total=False,
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
@@ -2150,24 +2148,24 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplacementEmailContentTypeDef = TypedDict(
     "ReplacementEmailContentTypeDef",
     {
         "ReplacementTemplate": ReplacementTemplateTypeDef,
@@ -2187,142 +2185,127 @@
     "_OptionalSuppressedDestinationTypeDef",
     {
         "Attributes": SuppressedDestinationAttributesTypeDef,
     },
     total=False,
 )
 
-
 class SuppressedDestinationTypeDef(
     _RequiredSuppressedDestinationTypeDef, _OptionalSuppressedDestinationTypeDef
 ):
     pass
 
+BatchGetMetricDataRequestRequestTypeDef = TypedDict(
+    "BatchGetMetricDataRequestRequestTypeDef",
+    {
+        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+    },
+)
 
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
-
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
-
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
         "VdmAttributes": VdmAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
@@ -2345,34 +2328,32 @@
         "Tags": Sequence[TagTypeDef],
         "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsTypeDef,
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -2382,22 +2363,20 @@
     "_OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
-
 class PutConfigurationSetVdmOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 CreateImportJobRequestRequestTypeDef = TypedDict(
     "CreateImportJobRequestRequestTypeDef",
     {
         "ImportDestination": ImportDestinationTypeDef,
         "ImportDataSource": ImportDataSourceTypeDef,
     },
 )
@@ -2410,15 +2389,15 @@
         "ImportDataSource": ImportDataSourceTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
@@ -2443,21 +2422,19 @@
         "Filter": ListContactsFilterTypeDef,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBulkEmailEntryTypeDef = TypedDict(
     "_RequiredBulkEmailEntryTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailEntryTypeDef = TypedDict(
@@ -2465,37 +2442,43 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementEmailContent": ReplacementEmailContentTypeDef,
     },
     total=False,
 )
 
-
 class BulkEmailEntryTypeDef(_RequiredBulkEmailEntryTypeDef, _OptionalBulkEmailEntryTypeDef):
     pass
 
-
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    {
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2506,28 +2489,40 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DashboardEnabled": bool,
     },
 )
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+    },
+    total=False,
+)
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
 
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendBulkEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
@@ -2544,21 +2539,19 @@
         "FeedbackForwardingEmailAddressIdentityArn": str,
         "DefaultEmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendBulkEmailRequestRequestTypeDef(
     _RequiredSendBulkEmailRequestRequestTypeDef, _OptionalSendBulkEmailRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -2567,22 +2560,20 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Content": EmailContentTypeDef,
     },
 )
 _OptionalSendEmailRequestRequestTypeDef = TypedDict(
@@ -2597,12 +2588,11 @@
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "ListManagementOptions": ListManagementOptionsTypeDef,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2/type_defs.pyi` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sesv2.type_defs import ReviewDetailsTypeDef
 
-    data: ReviewDetailsTypeDef = {...}
+    data: ReviewDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -58,44 +58,44 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ReviewDetailsTypeDef",
-    "BatchGetMetricDataQueryTypeDef",
+    "TimestampTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
+    "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
     "TopicPreferenceTypeDef",
     "DeliveryOptionsTypeDef",
-    "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
-    "CreateImportJobResponseTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DashboardAttributesTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
@@ -107,64 +107,59 @@
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "RawMessageTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SuppressionOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
-    "GetEmailIdentityPoliciesResponseTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
     "GuardianAttributesTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "RecommendationTypeDef",
-    "ListSuppressedDestinationsRequestRequestTypeDef",
     "SuppressedDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountDetailsRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutAccountSuppressionAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -173,36 +168,47 @@
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
-    "ResponseMetadataTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
-    "TestRenderEmailTemplateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
-    "BatchGetMetricDataRequestRequestTypeDef",
+    "BatchGetMetricDataQueryTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "BatchGetMetricDataResponseTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    "CreateImportJobResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
     "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
     "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
@@ -222,50 +228,55 @@
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "ListEmailTemplatesResponseTypeDef",
+    "SuppressionOptionsUnionTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "VdmAttributesTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
+    "BatchGetMetricDataRequestRequestTypeDef",
+    "ReputationOptionsUnionTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "DomainDeliverabilityTrackingOptionUnionTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
     "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -273,37 +284,15 @@
     {
         "Status": ReviewStatusType,
         "CaseId": str,
     },
     total=False,
 )
 
-_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_RequiredBatchGetMetricDataQueryTypeDef",
-    {
-        "Id": str,
-        "Namespace": Literal["VDM"],
-        "Metric": MetricType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
-    "_OptionalBatchGetMetricDataQueryTypeDef",
-    {
-        "Dimensions": Mapping[MetricDimensionNameType, str],
-    },
-    total=False,
-)
-
-class BatchGetMetricDataQueryTypeDef(
-    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 MetricDataErrorTypeDef = TypedDict(
     "MetricDataErrorTypeDef",
     {
         "Id": str,
         "Code": QueryErrorCodeType,
         "Message": str,
     },
@@ -316,41 +305,55 @@
         "Id": str,
         "Timestamps": List[datetime],
         "Values": List[int],
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
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
+
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
+
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateName": str,
         "TemplateArn": str,
         "TemplateData": str,
     },
@@ -424,23 +427,14 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-ReputationOptionsTypeDef = TypedDict(
-    "ReputationOptionsTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": Union[datetime, str],
-    },
-    total=False,
-)
-
 SendingOptionsTypeDef = TypedDict(
     "SendingOptionsTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -480,38 +474,31 @@
     "_OptionalTopicTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class TopicTypeDef(_RequiredTopicTypeDef, _OptionalTopicTypeDef):
     pass
 
+
 CreateCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
 )
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateEmailIdentityPolicyRequestRequestTypeDef = TypedDict(
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -555,22 +542,14 @@
     "ImportDataSourceTypeDef",
     {
         "S3Url": str,
         "DataFormat": DataFormatType,
     },
 )
 
-CreateImportJobResponseTypeDef = TypedDict(
-    "CreateImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomVerificationEmailTemplateMetadataTypeDef = TypedDict(
     "CustomVerificationEmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -638,17 +617,19 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
+
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
+
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -748,28 +729,30 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
-InboxPlacementTrackingOptionTypeDef = TypedDict(
-    "InboxPlacementTrackingOptionTypeDef",
+InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionOutputTypeDef",
     {
         "Global": bool,
         "TrackedIsps": List[str],
     },
     total=False,
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
+InboxPlacementTrackingOptionTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Global": bool,
+        "TrackedIsps": Sequence[str],
     },
+    total=False,
 )
 
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
@@ -844,14 +827,31 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+ReputationOptionsOutputTypeDef = TypedDict(
+    "ReputationOptionsOutputTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": datetime,
+    },
+    total=False,
+)
+
+SuppressionOptionsOutputTypeDef = TypedDict(
+    "SuppressionOptionsOutputTypeDef",
+    {
+        "SuppressedReasons": List[SuppressionListReasonType],
+    },
+    total=False,
+)
+
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
@@ -866,27 +866,14 @@
 GetCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
-GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "FromEmailAddress": str,
-        "TemplateSubject": str,
-        "TemplateContent": str,
-        "SuccessRedirectionURL": str,
-        "FailureRedirectionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 
@@ -929,38 +916,21 @@
 GetDomainDeliverabilityCampaignRequestRequestTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     {
         "CampaignId": str,
     },
 )
 
-GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-    },
-)
-
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
-GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -1033,23 +1003,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListContactListsRequestRequestTypeDef = TypedDict(
     "ListContactListsRequestRequestTypeDef",
     {
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
@@ -1078,55 +1039,23 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListDedicatedIpPoolsResponseTypeDef = TypedDict(
-    "ListDedicatedIpPoolsResponseTypeDef",
-    {
-        "DedicatedIpPools": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "SubscribedDomain": str,
-    },
-)
-_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
-class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
-    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-):
-    pass
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1161,19 +1090,21 @@
     "_OptionalListManagementOptionsTypeDef",
     {
         "TopicName": str,
     },
     total=False,
 )
 
+
 class ListManagementOptionsTypeDef(
     _RequiredListManagementOptionsTypeDef, _OptionalListManagementOptionsTypeDef
 ):
     pass
 
+
 ListRecommendationsRequestRequestTypeDef = TypedDict(
     "ListRecommendationsRequestRequestTypeDef",
     {
         "Filter": Mapping[ListRecommendationsFilterKeyType, str],
         "NextToken": str,
         "PageSize": int,
     },
@@ -1190,26 +1121,14 @@
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Impact": RecommendationImpactType,
     },
     total=False,
 )
 
-ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
-    "ListSuppressedDestinationsRequestRequestTypeDef",
-    {
-        "Reasons": Sequence[SuppressionListReasonType],
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
 SuppressedDestinationSummaryTypeDef = TypedDict(
     "SuppressedDestinationSummaryTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
         "LastUpdateTime": datetime,
     },
@@ -1244,19 +1163,21 @@
         "ContactLanguage": ContactLanguageType,
         "AdditionalContactEmailAddresses": Sequence[str],
         "ProductionAccessEnabled": bool,
     },
     total=False,
 )
 
+
 class PutAccountDetailsRequestRequestTypeDef(
     _RequiredPutAccountDetailsRequestRequestTypeDef, _OptionalPutAccountDetailsRequestRequestTypeDef
 ):
     pass
 
+
 PutAccountSendingAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountSendingAttributesRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
@@ -1280,100 +1201,110 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     {
         "SuppressedReasons": Sequence[SuppressionListReasonType],
     },
     total=False,
 )
 
+
 class PutConfigurationSetSuppressionOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -1404,48 +1335,43 @@
     "_OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    {
-        "DkimStatus": DkimStatusType,
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
@@ -1453,20 +1379,22 @@
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -1474,20 +1402,22 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
+
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 PutSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "PutSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "Reason": SuppressionListReasonType,
     },
 )
@@ -1496,25 +1426,14 @@
     "ReplacementTemplateTypeDef",
     {
         "ReplacementTemplateData": str,
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
 _RequiredSendCustomVerificationEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "TemplateName": str,
     },
 )
@@ -1522,35 +1441,21 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
-SendCustomVerificationEmailResponseTypeDef = TypedDict(
-    "SendCustomVerificationEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
@@ -1561,22 +1466,14 @@
     "TestRenderEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderEmailTemplateResponseTypeDef = TypedDict(
-    "TestRenderEmailTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1611,35 +1508,204 @@
         "UseCaseDescription": str,
         "AdditionalContactEmailAddresses": List[str],
         "ReviewDetails": ReviewDetailsTypeDef,
     },
     total=False,
 )
 
-BatchGetMetricDataRequestRequestTypeDef = TypedDict(
-    "BatchGetMetricDataRequestRequestTypeDef",
+_RequiredBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_RequiredBatchGetMetricDataQueryTypeDef",
     {
-        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
+        "Id": str,
+        "Namespace": Literal["VDM"],
+        "Metric": MetricType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
     },
 )
+_OptionalBatchGetMetricDataQueryTypeDef = TypedDict(
+    "_OptionalBatchGetMetricDataQueryTypeDef",
+    {
+        "Dimensions": Mapping[MetricDimensionNameType, str],
+    },
+    total=False,
+)
+
+
+class BatchGetMetricDataQueryTypeDef(
+    _RequiredBatchGetMetricDataQueryTypeDef, _OptionalBatchGetMetricDataQueryTypeDef
+):
+    pass
+
+
+GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+
+_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "SubscribedDomain": str,
+    },
+)
+_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+
+class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
+    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+):
+    pass
+
+
+ListSuppressedDestinationsRequestRequestTypeDef = TypedDict(
+    "ListSuppressedDestinationsRequestRequestTypeDef",
+    {
+        "Reasons": Sequence[SuppressionListReasonType],
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
+)
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImportJobResponseTypeDef = TypedDict(
+    "CreateImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "FromEmailAddress": str,
+        "TemplateSubject": str,
+        "TemplateContent": str,
+        "SuccessRedirectionURL": str,
+        "FailureRedirectionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDedicatedIpPoolsResponseTypeDef = TypedDict(
+    "ListDedicatedIpPoolsResponseTypeDef",
+    {
+        "DedicatedIpPools": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    {
+        "DkimStatus": DkimStatusType,
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderEmailTemplateResponseTypeDef = TypedDict(
+    "TestRenderEmailTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBlacklistReportsResponseTypeDef = TypedDict(
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
     },
 )
 
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
@@ -1656,15 +1722,22 @@
     total=False,
 )
 
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1672,15 +1745,15 @@
 )
 
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
@@ -1705,31 +1778,33 @@
         "TopicPreferences": Sequence[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
     },
     total=False,
 )
 
+
 class CreateContactRequestRequestTypeDef(
     _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
 ):
     pass
 
+
 GetContactResponseTypeDef = TypedDict(
     "GetContactResponseTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
         "TopicPreferences": List[TopicPreferenceTypeDef],
         "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1742,19 +1817,21 @@
         "TopicPreferences": Sequence[TopicPreferenceTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
     },
     total=False,
 )
 
+
 class UpdateContactRequestRequestTypeDef(
     _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 _OptionalCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
@@ -1762,25 +1839,27 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ScalingMode": ScalingModeType,
     },
     total=False,
 )
 
+
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1800,29 +1879,31 @@
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateContactListRequestRequestTypeDef(
     _RequiredCreateContactListRequestRequestTypeDef, _OptionalCreateContactListRequestRequestTypeDef
 ):
     pass
 
+
 GetContactListResponseTypeDef = TypedDict(
     "GetContactListResponseTypeDef",
     {
         "ContactListName": str,
         "Topics": List[TopicTypeDef],
         "Description": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
@@ -1833,19 +1914,21 @@
     {
         "Topics": Sequence[TopicTypeDef],
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateContactListRequestRequestTypeDef(
     _RequiredUpdateContactListRequestRequestTypeDef, _OptionalUpdateContactListRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
@@ -1854,20 +1937,22 @@
         "Tags": Sequence[TagTypeDef],
         "DkimSigningAttributes": DkimSigningAttributesTypeDef,
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "SigningAttributesOrigin": DkimSigningAttributesOriginType,
     },
 )
@@ -1875,27 +1960,29 @@
     "_OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     {
         "SigningAttributes": DkimSigningAttributesTypeDef,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1904,15 +1991,15 @@
 )
 
 GetEmailTemplateResponseTypeDef = TypedDict(
     "GetEmailTemplateResponseTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
@@ -1921,15 +2008,15 @@
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1949,80 +2036,91 @@
     total=False,
 )
 
 GetDedicatedIpPoolResponseTypeDef = TypedDict(
     "GetDedicatedIpPoolResponseTypeDef",
     {
         "DedicatedIpPool": DedicatedIpPoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpResponseTypeDef = TypedDict(
     "GetDedicatedIpResponseTypeDef",
     {
         "DedicatedIp": DedicatedIpTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
+    {
+        "Domain": str,
+        "SubscriptionStartDate": datetime,
+        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
+    },
+    total=False,
+)
+
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": datetime,
+        "SubscriptionStartDate": TimestampTypeDef,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SuppressionOptionsUnionTypeDef = Union[SuppressionOptionsTypeDef, SuppressionOptionsOutputTypeDef]
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -2036,15 +2134,15 @@
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
         "Tags": List[TagTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
@@ -2055,32 +2153,34 @@
     {
         "DashboardAttributes": DashboardAttributesTypeDef,
         "GuardianAttributes": GuardianAttributesTypeDef,
     },
     total=False,
 )
 
+
 class VdmAttributesTypeDef(_RequiredVdmAttributesTypeDef, _OptionalVdmAttributesTypeDef):
     pass
 
+
 VdmOptionsTypeDef = TypedDict(
     "VdmOptionsTypeDef",
     {
         "DashboardOptions": DashboardOptionsTypeDef,
         "GuardianOptions": GuardianOptionsTypeDef,
     },
     total=False,
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
@@ -2099,24 +2199,24 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplacementEmailContentTypeDef = TypedDict(
     "ReplacementEmailContentTypeDef",
     {
         "ReplacementTemplate": ReplacementTemplateTypeDef,
@@ -2136,136 +2236,131 @@
     "_OptionalSuppressedDestinationTypeDef",
     {
         "Attributes": SuppressedDestinationAttributesTypeDef,
     },
     total=False,
 )
 
+
 class SuppressedDestinationTypeDef(
     _RequiredSuppressedDestinationTypeDef, _OptionalSuppressedDestinationTypeDef
 ):
     pass
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+
+BatchGetMetricDataRequestRequestTypeDef = TypedDict(
+    "BatchGetMetricDataRequestRequestTypeDef",
     {
-        "Subject": ContentTypeDef,
-        "Body": BodyTypeDef,
+        "Queries": Sequence[BatchGetMetricDataQueryTypeDef],
     },
 )
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
+ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
+        "Subject": ContentTypeDef,
+        "Body": BodyTypeDef,
     },
-    total=False,
 )
 
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
+
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
+
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
+
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
+DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
+    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
+]
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
         "VdmAttributes": VdmAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
@@ -2288,32 +2383,34 @@
         "Tags": Sequence[TagTypeDef],
         "SuppressionOptions": SuppressionOptionsTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsTypeDef,
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
         "VdmOptions": VdmOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -2323,20 +2420,22 @@
     "_OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "VdmOptions": VdmOptionsTypeDef,
     },
     total=False,
 )
 
+
 class PutConfigurationSetVdmOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 CreateImportJobRequestRequestTypeDef = TypedDict(
     "CreateImportJobRequestRequestTypeDef",
     {
         "ImportDestination": ImportDestinationTypeDef,
         "ImportDataSource": ImportDataSourceTypeDef,
     },
 )
@@ -2349,15 +2448,15 @@
         "ImportDataSource": ImportDataSourceTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
@@ -2382,19 +2481,21 @@
         "Filter": ListContactsFilterTypeDef,
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBulkEmailEntryTypeDef = TypedDict(
     "_RequiredBulkEmailEntryTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailEntryTypeDef = TypedDict(
@@ -2402,35 +2503,45 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementEmailContent": ReplacementEmailContentTypeDef,
     },
     total=False,
 )
 
+
 class BulkEmailEntryTypeDef(_RequiredBulkEmailEntryTypeDef, _OptionalBulkEmailEntryTypeDef):
     pass
 
+
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    {
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2441,28 +2552,42 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DashboardEnabled": bool,
     },
 )
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
 
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendBulkEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
@@ -2479,19 +2604,21 @@
         "FeedbackForwardingEmailAddressIdentityArn": str,
         "DefaultEmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendBulkEmailRequestRequestTypeDef(
     _RequiredSendBulkEmailRequestRequestTypeDef, _OptionalSendBulkEmailRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -2500,20 +2627,22 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Content": EmailContentTypeDef,
     },
 )
 _OptionalSendEmailRequestRequestTypeDef = TypedDict(
@@ -2528,11 +2657,12 @@
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "ListManagementOptions": ListManagementOptionsTypeDef,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/PKG-INFO` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sesv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SESV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SESV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sesv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sesv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sesv2"></a>
 
 # types-aiobotocore-sesv2
 
 [![PyPI - types-aiobotocore-sesv2](https://img.shields.io/pypi/v/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sesv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sesv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sesv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-sesv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sesv2)](https://pepy.tech/project/types-aiobotocore-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SESV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [types-aiobotocore-sesv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sesv2/).
 
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
@@ -312,52 +311,51 @@
 )
 
 
 def check_value(value: BehaviorOnMxFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sesv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sesv2.type_defs import (
     ReviewDetailsTypeDef,
-    BatchGetMetricDataQueryTypeDef,
+    TimestampTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
+    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
     TopicPreferenceTypeDef,
     DeliveryOptionsTypeDef,
-    ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
-    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DashboardAttributesTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
@@ -369,64 +367,59 @@
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
-    RawMessageTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SuppressionOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
-    GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
     GuardianAttributesTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
-    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     RecommendationTypeDef,
-    ListSuppressedDestinationsRequestRequestTypeDef,
     SuppressedDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountDetailsRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutAccountSuppressionAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
@@ -435,36 +428,47 @@
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
-    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    BatchGetMetricDataRequestRequestTypeDef,
+    BatchGetMetricDataQueryTypeDef,
+    GetDomainStatisticsReportRequestRequestTypeDef,
+    ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    ListSuppressedDestinationsRequestRequestTypeDef,
+    ReputationOptionsTypeDef,
     BatchGetMetricDataResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    CreateImportJobResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
     CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
     UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
@@ -484,58 +488,63 @@
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    SuppressionOptionsUnionTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     VdmAttributesTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
+    BatchGetMetricDataRequestRequestTypeDef,
+    ReputationOptionsUnionTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
-    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    DomainDeliverabilityTrackingOptionUnionTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
     CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
+    PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ReviewDetailsTypeDef:
+def get_value() -> ReviewDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sesv2-2.5.2/types_aiobotocore_sesv2.egg-info/SOURCES.txt` & `types-aiobotocore-sesv2-2.5.2.post1/types_aiobotocore_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


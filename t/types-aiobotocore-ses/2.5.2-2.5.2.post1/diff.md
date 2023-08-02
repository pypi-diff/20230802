# Comparing `tmp/types-aiobotocore-ses-2.5.2.tar.gz` & `tmp/types-aiobotocore-ses-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ses-2.5.2.tar", last modified: Sat Jul  8 01:44:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-ses-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
```

## Comparing `types-aiobotocore-ses-2.5.2.tar` & `types-aiobotocore-ses-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.446899 types-aiobotocore-ses-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-07-08 01:44:19.446899 types-aiobotocore-ses-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:19.446899 types-aiobotocore-ses-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:00.000000 types-aiobotocore-ses-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.438899 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52059 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51973 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47999 2023-07-08 01:41:02.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47936 2023-07-08 01:41:02.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-08 01:41:01.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:19.446899 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-07-08 01:44:19.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:44:19.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:19.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:19.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:19.000000 types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.109457 types-aiobotocore-ses-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-02 14:53:01.101457 types-aiobotocore-ses-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.109457 types-aiobotocore-ses-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.101457 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52089 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52003 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49787 2023-08-02 14:49:42.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.101457 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ses-2.5.2/LICENSE` & `types-aiobotocore-ses-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/PKG-INFO` & `types-aiobotocore-ses-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ses
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ses type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ses type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ses"></a>
 
 # types-aiobotocore-ses
 
 [![PyPI - types-aiobotocore-ses](https://img.shields.io/pypi/v/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ses?color=blue)](https://pypistats.org/packages/types-aiobotocore-ses)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ses)](https://pepy.tech/project/types-aiobotocore-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SES 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [types-aiobotocore-ses docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/).
 
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
@@ -364,24 +363,25 @@
 )
 
 
 def check_value(value: BehaviorOnMXFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ses.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ses.type_defs import (
     AddHeaderActionTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -400,138 +400,144 @@
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
-    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
     LambdaActionTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
-    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
-    RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
-    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
-    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesResponseTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
+    GetSendQuotaResponseTypeDef,
+    GetTemplateResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListCustomVerificationEmailTemplatesResponseTypeDef,
+    ListIdentitiesResponseTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
-    MessageDsnTypeDef,
-    RecipientDsnFieldsTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    SendBounceResponseTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
+    TestRenderTemplateResponseTypeDef,
+    VerifyDomainDkimResponseTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
-    SendRawEmailRequestRequestTypeDef,
+    MessageDsnTypeDef,
+    RecipientDsnFieldsTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
+    SendRawEmailRequestRequestTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
+    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
+    EventDestinationUnionTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
-    CreateReceiptRuleRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
+    CreateReceiptRuleRequestRequestTypeDef,
+    ReceiptRuleUnionTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_value() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ses-2.5.2/README.md` & `types-aiobotocore-ses-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ses"></a>
 
 # types-aiobotocore-ses
 
 [![PyPI - types-aiobotocore-ses](https://img.shields.io/pypi/v/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ses?color=blue)](https://pypistats.org/packages/types-aiobotocore-ses)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ses)](https://pepy.tech/project/types-aiobotocore-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SES 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [types-aiobotocore-ses docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
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
@@ -331,24 +331,25 @@
 )
 
 
 def check_value(value: BehaviorOnMXFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ses.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ses.type_defs import (
     AddHeaderActionTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -367,138 +368,144 @@
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
-    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
     LambdaActionTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
-    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
-    RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
-    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
-    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesResponseTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
+    GetSendQuotaResponseTypeDef,
+    GetTemplateResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListCustomVerificationEmailTemplatesResponseTypeDef,
+    ListIdentitiesResponseTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
-    MessageDsnTypeDef,
-    RecipientDsnFieldsTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    SendBounceResponseTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
+    TestRenderTemplateResponseTypeDef,
+    VerifyDomainDkimResponseTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
-    SendRawEmailRequestRequestTypeDef,
+    MessageDsnTypeDef,
+    RecipientDsnFieldsTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
+    SendRawEmailRequestRequestTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
+    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
+    EventDestinationUnionTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
-    CreateReceiptRuleRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
+    CreateReceiptRuleRequestRequestTypeDef,
+    ReceiptRuleUnionTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_value() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ses-2.5.2/setup.py` & `types-aiobotocore-ses-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ses",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore ses type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ses type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ses": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/__init__.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/__init__.pyi` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/__main__.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SES 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SES 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/client.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventDestinationTypeDef,
+    EventDestinationUnionTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
@@ -64,15 +64,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
-    ReceiptRuleTypeDef,
+    ReceiptRuleUnionTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TemplateTypeDef,
@@ -188,15 +188,15 @@
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set)
         """
 
     async def create_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set_event_destination)
         """
@@ -234,15 +234,15 @@
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_filter)
         """
 
     async def create_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef, After: str = ...
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef, After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_rule)
         """
@@ -840,15 +840,15 @@
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_account_sending_enabled)
         """
 
     async def update_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_configuration_set_event_destination)
         """
@@ -900,15 +900,15 @@
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_custom_verification_email_template)
         """
 
     async def update_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_receipt_rule)
         """
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/client.pyi` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventDestinationTypeDef,
+    EventDestinationUnionTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
@@ -64,15 +64,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
-    ReceiptRuleTypeDef,
+    ReceiptRuleUnionTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TemplateTypeDef,
@@ -179,15 +179,15 @@
         """
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set)
         """
     async def create_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set_event_destination)
         """
@@ -221,15 +221,15 @@
         """
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_filter)
         """
     async def create_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef, After: str = ...
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef, After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_rule)
         """
@@ -772,15 +772,15 @@
         Enables or disables email sending across your entire Amazon SES account in the
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_account_sending_enabled)
         """
     async def update_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_configuration_set_event_destination)
         """
@@ -827,15 +827,15 @@
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_custom_verification_email_template)
         """
     async def update_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_receipt_rule)
         """
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/literals.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/literals.pyi` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/paginator.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,30 +65,30 @@
 class ListConfigurationSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listconfigurationsetspaginator)
         """
 
 
 class ListCustomVerificationEmailTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listcustomverificationemailtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listcustomverificationemailtemplatespaginator)
         """
 
 
@@ -98,43 +98,43 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listidentitiespaginator)
         """
 
 
 class ListReceiptRuleSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listreceiptrulesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReceiptRuleSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listreceiptrulesetspaginator)
         """
 
 
 class ListTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listtemplatespaginator)
         """
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/paginator.pyi` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,29 +62,29 @@
 class ListConfigurationSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listconfigurationsetspaginator)
         """
 
 class ListCustomVerificationEmailTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listcustomverificationemailtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listcustomverificationemailtemplatespaginator)
         """
 
 class ListIdentitiesPaginator(AioPaginator):
@@ -93,41 +93,41 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listidentitiespaginator)
         """
 
 class ListReceiptRuleSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listreceiptrulesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReceiptRuleSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listreceiptrulesetspaginator)
         """
 
 class ListTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/paginators/#listtemplatespaginator)
         """
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/type_defs.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ses.type_defs import AddHeaderActionTypeDef
 
-    data: AddHeaderActionTypeDef = {...}
+    data: AddHeaderActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -43,14 +43,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddHeaderActionTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
@@ -69,144 +70,151 @@
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
-    "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     "IdentityMailFromDomainAttributesTypeDef",
     "GetIdentityNotificationAttributesRequestRequestTypeDef",
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
-    "GetIdentityPoliciesResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
-    "GetSendQuotaResponseTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LambdaActionTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
-    "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
-    "ListIdentityPoliciesResponseTypeDef",
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    "PaginatorConfigTypeDef",
+    "TimestampTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
-    "RawMessageTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendBounceResponseTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "SendRawEmailResponseTypeDef",
-    "SendTemplatedEmailResponseTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
     "SetIdentityMailFromDomainRequestRequestTypeDef",
     "SetIdentityNotificationTopicRequestRequestTypeDef",
     "SetReceiptRulePositionRequestRequestTypeDef",
     "TestRenderTemplateRequestRequestTypeDef",
-    "TestRenderTemplateResponseTypeDef",
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
-    "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
-    "VerifyDomainIdentityResponseTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
-    "SendBulkTemplatedEmailResponseTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSendingEnabledResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetIdentityPoliciesResponseTypeDef",
+    "GetSendQuotaResponseTypeDef",
+    "GetTemplateResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    "ListIdentitiesResponseTypeDef",
+    "ListIdentityPoliciesResponseTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
-    "MessageDsnTypeDef",
-    "RecipientDsnFieldsTypeDef",
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    "SendBounceResponseTypeDef",
+    "SendBulkTemplatedEmailResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "SendRawEmailResponseTypeDef",
+    "SendTemplatedEmailResponseTypeDef",
+    "TestRenderTemplateResponseTypeDef",
+    "VerifyDomainDkimResponseTypeDef",
+    "VerifyDomainIdentityResponseTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
-    "SendRawEmailRequestRequestTypeDef",
+    "MessageDsnTypeDef",
+    "RecipientDsnFieldsTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
+    "SendRawEmailRequestRequestTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
+    "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
+    "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "EventDestinationUnionTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
-    "CreateReceiptRuleRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
+    "CreateReceiptRuleRequestRequestTypeDef",
+    "ReceiptRuleUnionTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
@@ -449,14 +457,25 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
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
 _RequiredDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -496,21 +515,14 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
         "DeliveryStreamARN": str,
     },
 )
@@ -526,42 +538,21 @@
     "ExtensionFieldTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-GetAccountSendingEnabledResponseTypeDef = TypedDict(
-    "GetAccountSendingEnabledResponseTypeDef",
-    {
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 GetIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -640,22 +631,14 @@
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
 
-GetIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
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
@@ -685,24 +668,14 @@
 
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
 
-GetSendQuotaResponseTypeDef = TypedDict(
-    "GetSendQuotaResponseTypeDef",
-    {
-        "Max24HourSend": float,
-        "MaxSendRate": float,
-        "SentLast24Hours": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -734,115 +707,67 @@
 )
 
 
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
 
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
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
 
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomVerificationEmailTemplatesRequestRequestTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    {
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIdentitiesRequestRequestTypeDef = TypedDict(
     "ListIdentitiesRequestRequestTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListIdentitiesResponseTypeDef = TypedDict(
-    "ListIdentitiesResponseTypeDef",
-    {
-        "Identities": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "ListIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
     },
 )
 
-ListIdentityPoliciesResponseTypeDef = TypedDict(
-    "ListIdentityPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReceiptRuleSetsRequestRequestTypeDef = TypedDict(
     "ListReceiptRuleSetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
@@ -853,48 +778,24 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    {
-        "VerifiedEmailAddresses": List[str],
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
+TimestampTypeDef = Union[datetime, str]
 PutIdentityPolicyRequestRequestTypeDef = TypedDict(
     "PutIdentityPolicyRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyName": str,
         "Policy": str,
     },
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -981,33 +882,14 @@
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleNames": Sequence[str],
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
-SendBounceResponseTypeDef = TypedDict(
-    "SendBounceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1023,46 +905,14 @@
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
-
-SendRawEmailResponseTypeDef = TypedDict(
-    "SendRawEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendTemplatedEmailResponseTypeDef = TypedDict(
-    "SendTemplatedEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -1165,22 +1015,14 @@
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderTemplateResponseTypeDef = TypedDict(
-    "TestRenderTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSendingEnabledRequestRequestTypeDef = TypedDict(
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1230,68 +1072,51 @@
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainDkimResponseTypeDef = TypedDict(
-    "VerifyDomainDkimResponseTypeDef",
-    {
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyDomainIdentityRequestRequestTypeDef = TypedDict(
     "VerifyDomainIdentityRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainIdentityResponseTypeDef = TypedDict(
-    "VerifyDomainIdentityResponseTypeDef",
-    {
-        "VerificationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyEmailAddressRequestRequestTypeDef = TypedDict(
     "VerifyEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
 VerifyEmailIdentityRequestRequestTypeDef = TypedDict(
     "VerifyEmailIdentityRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
-SendBulkTemplatedEmailResponseTypeDef = TypedDict(
-    "SendBulkTemplatedEmailResponseTypeDef",
-    {
-        "Status": List[BulkEmailDestinationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredBulkEmailDestinationTypeDef = TypedDict(
     "_RequiredBulkEmailDestinationTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailDestinationTypeDef = TypedDict(
@@ -1337,37 +1162,35 @@
 class SendTemplatedEmailRequestRequestTypeDef(
     _RequiredSendTemplatedEmailRequestRequestTypeDef,
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
 
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
+    },
+)
+
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
     },
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[ConfigurationSetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
     },
 )
@@ -1383,38 +1206,21 @@
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    {
-        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
@@ -1429,90 +1235,213 @@
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSendingEnabledResponseTypeDef = TypedDict(
+    "GetAccountSendingEnabledResponseTypeDef",
+    {
+        "Enabled": bool,
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
+GetIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSendQuotaResponseTypeDef = TypedDict(
+    "GetSendQuotaResponseTypeDef",
+    {
+        "Max24HourSend": float,
+        "MaxSendRate": float,
+        "SentLast24Hours": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[ConfigurationSetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    {
+        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentitiesResponseTypeDef = TypedDict(
+    "ListIdentitiesResponseTypeDef",
+    {
+        "Identities": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoliciesResponseTypeDef = TypedDict(
+    "ListIdentityPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListReceiptRuleSetsResponseTypeDef = TypedDict(
     "ListReceiptRuleSetsResponseTypeDef",
     {
         "RuleSets": List[ReceiptRuleSetMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMessageDsnTypeDef = TypedDict(
-    "_RequiredMessageDsnTypeDef",
+ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
+    "ListVerifiedEmailAddressesResponseTypeDef",
     {
-        "ReportingMta": str,
+        "VerifiedEmailAddresses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalMessageDsnTypeDef = TypedDict(
-    "_OptionalMessageDsnTypeDef",
+
+SendBounceResponseTypeDef = TypedDict(
+    "SendBounceResponseTypeDef",
     {
-        "ArrivalDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+SendBulkTemplatedEmailResponseTypeDef = TypedDict(
+    "SendBulkTemplatedEmailResponseTypeDef",
+    {
+        "Status": List[BulkEmailDestinationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
-    pass
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredRecipientDsnFieldsTypeDef = TypedDict(
-    "_RequiredRecipientDsnFieldsTypeDef",
+SendRawEmailResponseTypeDef = TypedDict(
+    "SendRawEmailResponseTypeDef",
     {
-        "Action": DsnActionType,
-        "Status": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRecipientDsnFieldsTypeDef = TypedDict(
-    "_OptionalRecipientDsnFieldsTypeDef",
+
+SendTemplatedEmailResponseTypeDef = TypedDict(
+    "SendTemplatedEmailResponseTypeDef",
     {
-        "FinalRecipient": str,
-        "RemoteMta": str,
-        "DiagnosticCode": str,
-        "LastAttemptDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+TestRenderTemplateResponseTypeDef = TypedDict(
+    "TestRenderTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class RecipientDsnFieldsTypeDef(
-    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
-):
-    pass
+VerifyDomainDkimResponseTypeDef = TypedDict(
+    "VerifyDomainDkimResponseTypeDef",
+    {
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+VerifyDomainIdentityResponseTypeDef = TypedDict(
+    "VerifyDomainIdentityResponseTypeDef",
+    {
+        "VerificationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityMailFromDomainAttributesResponseTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     {
         "MailFromDomainAttributes": Dict[str, IdentityMailFromDomainAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityNotificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityNotificationAttributesResponseTypeDef",
     {
         "NotificationAttributes": Dict[str, IdentityNotificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = TypedDict(
     "_RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "Identities": Sequence[str],
@@ -1534,58 +1463,118 @@
     pass
 
 
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSendStatisticsResponseTypeDef = TypedDict(
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    {
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_RequiredSendRawEmailRequestRequestTypeDef",
+_RequiredMessageDsnTypeDef = TypedDict(
+    "_RequiredMessageDsnTypeDef",
     {
-        "RawMessage": RawMessageTypeDef,
+        "ReportingMta": str,
     },
 )
-_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_OptionalSendRawEmailRequestRequestTypeDef",
+_OptionalMessageDsnTypeDef = TypedDict(
+    "_OptionalMessageDsnTypeDef",
     {
-        "Source": str,
-        "Destinations": Sequence[str],
-        "FromArn": str,
-        "SourceArn": str,
-        "ReturnPathArn": str,
-        "Tags": Sequence[MessageTagTypeDef],
-        "ConfigurationSetName": str,
+        "ArrivalDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
 
-class SendRawEmailRequestRequestTypeDef(
-    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
+    pass
+
+
+_RequiredRecipientDsnFieldsTypeDef = TypedDict(
+    "_RequiredRecipientDsnFieldsTypeDef",
+    {
+        "Action": DsnActionType,
+        "Status": str,
+    },
+)
+_OptionalRecipientDsnFieldsTypeDef = TypedDict(
+    "_OptionalRecipientDsnFieldsTypeDef",
+    {
+        "FinalRecipient": str,
+        "RemoteMta": str,
+        "DiagnosticCode": str,
+        "LastAttemptDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+    },
+    total=False,
+)
+
+
+class RecipientDsnFieldsTypeDef(
+    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
 
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
@@ -1604,14 +1593,41 @@
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
 
+_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_RequiredSendRawEmailRequestRequestTypeDef",
+    {
+        "RawMessage": RawMessageTypeDef,
+    },
+)
+_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_OptionalSendRawEmailRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Destinations": Sequence[str],
+        "FromArn": str,
+        "SourceArn": str,
+        "ReturnPathArn": str,
+        "Tags": Sequence[MessageTagTypeDef],
+        "ConfigurationSetName": str,
+    },
+    total=False,
+)
+
+
+class SendRawEmailRequestRequestTypeDef(
+    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+):
+    pass
+
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -1643,14 +1659,39 @@
 class SendBulkTemplatedEmailRequestRequestTypeDef(
     _RequiredSendBulkTemplatedEmailRequestRequestTypeDef,
     _OptionalSendBulkTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredEventDestinationOutputTypeDef = TypedDict(
+    "_RequiredEventDestinationOutputTypeDef",
+    {
+        "Name": str,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationOutputTypeDef = TypedDict(
+    "_OptionalEventDestinationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "SNSDestination": SNSDestinationTypeDef,
+    },
+    total=False,
+)
+
+
+class EventDestinationOutputTypeDef(
+    _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
+):
+    pass
+
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
 )
@@ -1689,14 +1730,39 @@
 
 class BouncedRecipientInfoTypeDef(
     _RequiredBouncedRecipientInfoTypeDef, _OptionalBouncedRecipientInfoTypeDef
 ):
     pass
 
 
+_RequiredReceiptRuleOutputTypeDef = TypedDict(
+    "_RequiredReceiptRuleOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalReceiptRuleOutputTypeDef = TypedDict(
+    "_OptionalReceiptRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+        "TlsPolicy": TlsPolicyType,
+        "Recipients": List[str],
+        "Actions": List[ReceiptActionTypeDef],
+        "ScanEnabled": bool,
+    },
+    total=False,
+)
+
+
+class ReceiptRuleOutputTypeDef(
+    _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredReceiptRuleTypeDef = TypedDict(
     "_RequiredReceiptRuleTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalReceiptRuleTypeDef = TypedDict(
@@ -1723,15 +1789,15 @@
     },
 )
 
 ListReceiptFiltersResponseTypeDef = TypedDict(
     "ListReceiptFiltersResponseTypeDef",
     {
         "Filters": List[ReceiptFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1755,34 +1821,35 @@
 
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
 
-CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "EventDestination": EventDestinationTypeDef,
-    },
-)
-
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
-        "EventDestinations": List[EventDestinationTypeDef],
+        "EventDestinations": List[EventDestinationOutputTypeDef],
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "EventDestination": EventDestinationTypeDef,
     },
 )
 
+EventDestinationUnionTypeDef = Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1808,14 +1875,40 @@
 
 class SendBounceRequestRequestTypeDef(
     _RequiredSendBounceRequestRequestTypeDef, _OptionalSendBounceRequestRequestTypeDef
 ):
     pass
 
 
+DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
+    "DescribeActiveReceiptRuleSetResponseTypeDef",
+    {
+        "Metadata": ReceiptRuleSetMetadataTypeDef,
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReceiptRuleResponseTypeDef = TypedDict(
+    "DescribeReceiptRuleResponseTypeDef",
+    {
+        "Rule": ReceiptRuleOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReceiptRuleSetResponseTypeDef = TypedDict(
+    "DescribeReceiptRuleSetResponseTypeDef",
+    {
+        "Metadata": ReceiptRuleSetMetadataTypeDef,
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
@@ -1830,40 +1923,15 @@
 
 class CreateReceiptRuleRequestRequestTypeDef(
     _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
 ):
     pass
 
 
-DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
-    "DescribeActiveReceiptRuleSetResponseTypeDef",
-    {
-        "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeReceiptRuleResponseTypeDef = TypedDict(
-    "DescribeReceiptRuleResponseTypeDef",
-    {
-        "Rule": ReceiptRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeReceiptRuleSetResponseTypeDef = TypedDict(
-    "DescribeReceiptRuleSetResponseTypeDef",
-    {
-        "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+ReceiptRuleUnionTypeDef = Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/type_defs.pyi` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ses.type_defs import AddHeaderActionTypeDef
 
-    data: AddHeaderActionTypeDef = {...}
+    data: AddHeaderActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -42,14 +42,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddHeaderActionTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
@@ -68,144 +69,151 @@
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
-    "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     "IdentityMailFromDomainAttributesTypeDef",
     "GetIdentityNotificationAttributesRequestRequestTypeDef",
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
-    "GetIdentityPoliciesResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
-    "GetSendQuotaResponseTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LambdaActionTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
-    "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
-    "ListIdentityPoliciesResponseTypeDef",
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    "PaginatorConfigTypeDef",
+    "TimestampTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
-    "RawMessageTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendBounceResponseTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "SendRawEmailResponseTypeDef",
-    "SendTemplatedEmailResponseTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
     "SetIdentityMailFromDomainRequestRequestTypeDef",
     "SetIdentityNotificationTopicRequestRequestTypeDef",
     "SetReceiptRulePositionRequestRequestTypeDef",
     "TestRenderTemplateRequestRequestTypeDef",
-    "TestRenderTemplateResponseTypeDef",
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
-    "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
-    "VerifyDomainIdentityResponseTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
-    "SendBulkTemplatedEmailResponseTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSendingEnabledResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetIdentityPoliciesResponseTypeDef",
+    "GetSendQuotaResponseTypeDef",
+    "GetTemplateResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    "ListIdentitiesResponseTypeDef",
+    "ListIdentityPoliciesResponseTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
-    "MessageDsnTypeDef",
-    "RecipientDsnFieldsTypeDef",
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    "SendBounceResponseTypeDef",
+    "SendBulkTemplatedEmailResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "SendRawEmailResponseTypeDef",
+    "SendTemplatedEmailResponseTypeDef",
+    "TestRenderTemplateResponseTypeDef",
+    "VerifyDomainDkimResponseTypeDef",
+    "VerifyDomainIdentityResponseTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
-    "SendRawEmailRequestRequestTypeDef",
+    "MessageDsnTypeDef",
+    "RecipientDsnFieldsTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
+    "SendRawEmailRequestRequestTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
+    "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
+    "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "EventDestinationUnionTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
-    "CreateReceiptRuleRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
+    "CreateReceiptRuleRequestRequestTypeDef",
+    "ReceiptRuleUnionTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
@@ -442,14 +450,25 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
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
 _RequiredDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -487,21 +506,14 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
         "DeliveryStreamARN": str,
     },
 )
@@ -517,42 +529,21 @@
     "ExtensionFieldTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-GetAccountSendingEnabledResponseTypeDef = TypedDict(
-    "GetAccountSendingEnabledResponseTypeDef",
-    {
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 GetIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -627,22 +618,14 @@
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
 
-GetIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
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
@@ -670,24 +653,14 @@
 )
 
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
-GetSendQuotaResponseTypeDef = TypedDict(
-    "GetSendQuotaResponseTypeDef",
-    {
-        "Max24HourSend": float,
-        "MaxSendRate": float,
-        "SentLast24Hours": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -717,115 +690,67 @@
     },
     total=False,
 )
 
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
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
 
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomVerificationEmailTemplatesRequestRequestTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    {
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIdentitiesRequestRequestTypeDef = TypedDict(
     "ListIdentitiesRequestRequestTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListIdentitiesResponseTypeDef = TypedDict(
-    "ListIdentitiesResponseTypeDef",
-    {
-        "Identities": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "ListIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
     },
 )
 
-ListIdentityPoliciesResponseTypeDef = TypedDict(
-    "ListIdentityPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReceiptRuleSetsRequestRequestTypeDef = TypedDict(
     "ListReceiptRuleSetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
@@ -836,48 +761,24 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    {
-        "VerifiedEmailAddresses": List[str],
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
+TimestampTypeDef = Union[datetime, str]
 PutIdentityPolicyRequestRequestTypeDef = TypedDict(
     "PutIdentityPolicyRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyName": str,
         "Policy": str,
     },
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -956,33 +857,14 @@
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleNames": Sequence[str],
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
-SendBounceResponseTypeDef = TypedDict(
-    "SendBounceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -996,46 +878,14 @@
 
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
-
-SendRawEmailResponseTypeDef = TypedDict(
-    "SendRawEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendTemplatedEmailResponseTypeDef = TypedDict(
-    "SendTemplatedEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -1132,22 +982,14 @@
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderTemplateResponseTypeDef = TypedDict(
-    "TestRenderTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSendingEnabledRequestRequestTypeDef = TypedDict(
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1195,68 +1037,51 @@
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainDkimResponseTypeDef = TypedDict(
-    "VerifyDomainDkimResponseTypeDef",
-    {
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyDomainIdentityRequestRequestTypeDef = TypedDict(
     "VerifyDomainIdentityRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainIdentityResponseTypeDef = TypedDict(
-    "VerifyDomainIdentityResponseTypeDef",
-    {
-        "VerificationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyEmailAddressRequestRequestTypeDef = TypedDict(
     "VerifyEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
 VerifyEmailIdentityRequestRequestTypeDef = TypedDict(
     "VerifyEmailIdentityRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
-SendBulkTemplatedEmailResponseTypeDef = TypedDict(
-    "SendBulkTemplatedEmailResponseTypeDef",
-    {
-        "Status": List[BulkEmailDestinationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredBulkEmailDestinationTypeDef = TypedDict(
     "_RequiredBulkEmailDestinationTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailDestinationTypeDef = TypedDict(
@@ -1298,37 +1123,35 @@
 
 class SendTemplatedEmailRequestRequestTypeDef(
     _RequiredSendTemplatedEmailRequestRequestTypeDef,
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
+    },
+)
+
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
     },
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[ConfigurationSetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
     },
 )
@@ -1344,38 +1167,21 @@
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    {
-        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
@@ -1388,86 +1194,213 @@
 
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSendingEnabledResponseTypeDef = TypedDict(
+    "GetAccountSendingEnabledResponseTypeDef",
+    {
+        "Enabled": bool,
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
+GetIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSendQuotaResponseTypeDef = TypedDict(
+    "GetSendQuotaResponseTypeDef",
+    {
+        "Max24HourSend": float,
+        "MaxSendRate": float,
+        "SentLast24Hours": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[ConfigurationSetTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    {
+        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentitiesResponseTypeDef = TypedDict(
+    "ListIdentitiesResponseTypeDef",
+    {
+        "Identities": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoliciesResponseTypeDef = TypedDict(
+    "ListIdentityPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListReceiptRuleSetsResponseTypeDef = TypedDict(
     "ListReceiptRuleSetsResponseTypeDef",
     {
         "RuleSets": List[ReceiptRuleSetMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMessageDsnTypeDef = TypedDict(
-    "_RequiredMessageDsnTypeDef",
+ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
+    "ListVerifiedEmailAddressesResponseTypeDef",
     {
-        "ReportingMta": str,
+        "VerifiedEmailAddresses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalMessageDsnTypeDef = TypedDict(
-    "_OptionalMessageDsnTypeDef",
+
+SendBounceResponseTypeDef = TypedDict(
+    "SendBounceResponseTypeDef",
     {
-        "ArrivalDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
-    pass
+SendBulkTemplatedEmailResponseTypeDef = TypedDict(
+    "SendBulkTemplatedEmailResponseTypeDef",
+    {
+        "Status": List[BulkEmailDestinationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredRecipientDsnFieldsTypeDef = TypedDict(
-    "_RequiredRecipientDsnFieldsTypeDef",
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
     {
-        "Action": DsnActionType,
-        "Status": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRecipientDsnFieldsTypeDef = TypedDict(
-    "_OptionalRecipientDsnFieldsTypeDef",
+
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
     {
-        "FinalRecipient": str,
-        "RemoteMta": str,
-        "DiagnosticCode": str,
-        "LastAttemptDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class RecipientDsnFieldsTypeDef(
-    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
-):
-    pass
+SendRawEmailResponseTypeDef = TypedDict(
+    "SendRawEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendTemplatedEmailResponseTypeDef = TypedDict(
+    "SendTemplatedEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderTemplateResponseTypeDef = TypedDict(
+    "TestRenderTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyDomainDkimResponseTypeDef = TypedDict(
+    "VerifyDomainDkimResponseTypeDef",
+    {
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyDomainIdentityResponseTypeDef = TypedDict(
+    "VerifyDomainIdentityResponseTypeDef",
+    {
+        "VerificationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityMailFromDomainAttributesResponseTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     {
         "MailFromDomainAttributes": Dict[str, IdentityMailFromDomainAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityNotificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityNotificationAttributesResponseTypeDef",
     {
         "NotificationAttributes": Dict[str, IdentityNotificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = TypedDict(
     "_RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "Identities": Sequence[str],
@@ -1487,57 +1420,115 @@
 ):
     pass
 
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSendStatisticsResponseTypeDef = TypedDict(
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    {
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_RequiredSendRawEmailRequestRequestTypeDef",
+_RequiredMessageDsnTypeDef = TypedDict(
+    "_RequiredMessageDsnTypeDef",
     {
-        "RawMessage": RawMessageTypeDef,
+        "ReportingMta": str,
     },
 )
-_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_OptionalSendRawEmailRequestRequestTypeDef",
+_OptionalMessageDsnTypeDef = TypedDict(
+    "_OptionalMessageDsnTypeDef",
     {
-        "Source": str,
-        "Destinations": Sequence[str],
-        "FromArn": str,
-        "SourceArn": str,
-        "ReturnPathArn": str,
-        "Tags": Sequence[MessageTagTypeDef],
-        "ConfigurationSetName": str,
+        "ArrivalDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
-class SendRawEmailRequestRequestTypeDef(
-    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
+    pass
+
+_RequiredRecipientDsnFieldsTypeDef = TypedDict(
+    "_RequiredRecipientDsnFieldsTypeDef",
+    {
+        "Action": DsnActionType,
+        "Status": str,
+    },
+)
+_OptionalRecipientDsnFieldsTypeDef = TypedDict(
+    "_OptionalRecipientDsnFieldsTypeDef",
+    {
+        "FinalRecipient": str,
+        "RemoteMta": str,
+        "DiagnosticCode": str,
+        "LastAttemptDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+    },
+    total=False,
+)
+
+class RecipientDsnFieldsTypeDef(
+    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
@@ -1555,14 +1546,39 @@
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
 
+_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_RequiredSendRawEmailRequestRequestTypeDef",
+    {
+        "RawMessage": RawMessageTypeDef,
+    },
+)
+_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_OptionalSendRawEmailRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Destinations": Sequence[str],
+        "FromArn": str,
+        "SourceArn": str,
+        "ReturnPathArn": str,
+        "Tags": Sequence[MessageTagTypeDef],
+        "ConfigurationSetName": str,
+    },
+    total=False,
+)
+
+class SendRawEmailRequestRequestTypeDef(
+    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+):
+    pass
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -1592,14 +1608,37 @@
 
 class SendBulkTemplatedEmailRequestRequestTypeDef(
     _RequiredSendBulkTemplatedEmailRequestRequestTypeDef,
     _OptionalSendBulkTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
+_RequiredEventDestinationOutputTypeDef = TypedDict(
+    "_RequiredEventDestinationOutputTypeDef",
+    {
+        "Name": str,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationOutputTypeDef = TypedDict(
+    "_OptionalEventDestinationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "SNSDestination": SNSDestinationTypeDef,
+    },
+    total=False,
+)
+
+class EventDestinationOutputTypeDef(
+    _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
+):
+    pass
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
 )
@@ -1634,14 +1673,37 @@
 )
 
 class BouncedRecipientInfoTypeDef(
     _RequiredBouncedRecipientInfoTypeDef, _OptionalBouncedRecipientInfoTypeDef
 ):
     pass
 
+_RequiredReceiptRuleOutputTypeDef = TypedDict(
+    "_RequiredReceiptRuleOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalReceiptRuleOutputTypeDef = TypedDict(
+    "_OptionalReceiptRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+        "TlsPolicy": TlsPolicyType,
+        "Recipients": List[str],
+        "Actions": List[ReceiptActionTypeDef],
+        "ScanEnabled": bool,
+    },
+    total=False,
+)
+
+class ReceiptRuleOutputTypeDef(
+    _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
+):
+    pass
+
 _RequiredReceiptRuleTypeDef = TypedDict(
     "_RequiredReceiptRuleTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalReceiptRuleTypeDef = TypedDict(
@@ -1666,15 +1728,15 @@
     },
 )
 
 ListReceiptFiltersResponseTypeDef = TypedDict(
     "ListReceiptFiltersResponseTypeDef",
     {
         "Filters": List[ReceiptFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1696,34 +1758,35 @@
 )
 
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
-CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "EventDestination": EventDestinationTypeDef,
-    },
-)
-
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
-        "EventDestinations": List[EventDestinationTypeDef],
+        "EventDestinations": List[EventDestinationOutputTypeDef],
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "EventDestination": EventDestinationTypeDef,
     },
 )
 
+EventDestinationUnionTypeDef = Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1747,60 +1810,61 @@
 )
 
 class SendBounceRequestRequestTypeDef(
     _RequiredSendBounceRequestRequestTypeDef, _OptionalSendBounceRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "RuleSetName": str,
-        "Rule": ReceiptRuleTypeDef,
-    },
-)
-_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "After": str,
-    },
-    total=False,
-)
-
-class CreateReceiptRuleRequestRequestTypeDef(
-    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
-):
-    pass
-
 DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleResponseTypeDef = TypedDict(
     "DescribeReceiptRuleResponseTypeDef",
     {
-        "Rule": ReceiptRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rule": ReceiptRuleOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "RuleSetName": str,
+        "Rule": ReceiptRuleTypeDef,
+    },
+)
+_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "After": str,
+    },
+    total=False,
+)
+
+class CreateReceiptRuleRequestRequestTypeDef(
+    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
+):
+    pass
+
+ReceiptRuleUnionTypeDef = Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/waiter.py` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses/waiter.pyi` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/PKG-INFO` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ses
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ses type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ses type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ses"></a>
 
 # types-aiobotocore-ses
 
 [![PyPI - types-aiobotocore-ses](https://img.shields.io/pypi/v/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ses.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ses)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ses?color=blue)](https://pypistats.org/packages/types-aiobotocore-ses)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ses)](https://pepy.tech/project/types-aiobotocore-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SES 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [types-aiobotocore-ses docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/).
 
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
@@ -364,24 +363,25 @@
 )
 
 
 def check_value(value: BehaviorOnMXFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ses.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ses.type_defs import (
     AddHeaderActionTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -400,138 +400,144 @@
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
-    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
     LambdaActionTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
-    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
-    RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
-    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
-    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesResponseTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
+    GetSendQuotaResponseTypeDef,
+    GetTemplateResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListCustomVerificationEmailTemplatesResponseTypeDef,
+    ListIdentitiesResponseTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
-    MessageDsnTypeDef,
-    RecipientDsnFieldsTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    SendBounceResponseTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
+    TestRenderTemplateResponseTypeDef,
+    VerifyDomainDkimResponseTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
-    SendRawEmailRequestRequestTypeDef,
+    MessageDsnTypeDef,
+    RecipientDsnFieldsTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
+    SendRawEmailRequestRequestTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
+    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
+    EventDestinationUnionTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
-    CreateReceiptRuleRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
+    CreateReceiptRuleRequestRequestTypeDef,
+    ReceiptRuleUnionTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_value() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ses-2.5.2/types_aiobotocore_ses.egg-info/SOURCES.txt` & `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

